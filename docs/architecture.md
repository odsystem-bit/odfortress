# Architecture OD Fortress

Ce document présente l'architecture générale d'OD Fortress. Il est destiné aux investisseurs, incubateurs et développeurs souhaitant comprendre les fondations techniques du projet.

> **Statut** : En cours de documentation. Certaines sections contiennent des placeholders qui seront complétées au fur et à mesure du développement.

---

## Vue d'ensemble

OD Fortress est une solution VPN client-serveur. L'application Android établit un tunnel chiffré vers les serveurs VPN, qui relaient le trafic internet de manière sécurisée.

```
┌─────────────────────────────────────────────────────────────┐
│                        Utilisateurs                         │
│  Particulier    Entreprise    Journaliste    Nomade        │
└──────────────────────┬────────────────────────────────────────┘
                       │
┌──────────────────────▼────────────────────────────────────────┐
│                     Client VPN Android                        │
│  Service VPN natif    WireGuard / OpenVPN / IKEv2           │
└──────────────────────┬────────────────────────────────────────┘
                       │ Tunnel chiffré
┌──────────────────────▼────────────────────────────────────────┐
│                     Serveurs VPN (Linux)                       │
│  Routage    No-logs    Firewall    Bandwidth monitoring       │
└──────────────────────┬────────────────────────────────────────┘
                       │
┌──────────────────────▼────────────────────────────────────────┐
│                     Backend API (Node.js)                     │
│  Auth · Abonnements · Serveurs · Paiements · Logs métriques │
└──────────────────────┬────────────────────────────────────────┘
                       │
        ┌──────────────┼──────────────┬──────────────┐
        │              │              │              │
┌───────▼──────┐ ┌────▼─────┐ ┌──────▼──────┐ ┌──────▼──────┐
│  PostgreSQL  │ │  Redis   │ │  Panel      │ │  Paiement   │
│              │ │ (cache)  │ │  Admin      │ │  Gateway    │
└──────────────┘ └──────────┘ └─────────────┘ └─────────────┘
```

---

## Couches applicatives

### 1. Client Android

- **Langage** : Kotlin
- **Service VPN natif** : VpnService Android
- **Protocoles** : WireGuard, OpenVPN, IKEv2
- **UI** : Jetpack Compose
- **Sécurité** : Android Keystore pour les clés

### 2. Serveurs VPN

- **OS** : Linux (Ubuntu/Debian)
- **Protocoles** : WireGuard, OpenVPN, IKEv2
- **Pare-feu** : nftables/iptables
- **Monitoring** : bande passante, latence, charge
- **No-logs** : politique stricte de non-conservation des logs de trafic

### 3. Backend API

- **Framework** : Node.js + Express
- **Base de données** : PostgreSQL
- **Cache** : Redis
- **Fonctionnalités** : authentification, gestion des abonnements, attribution des serveurs, paiements

### 4. Panel admin

- **Framework** : React ou Vue.js
- **Fonctionnalités** : gestion des serveurs, supervision des utilisateurs, rapports, support

### 5. Paiements

- **Mobile Money** : FedaPay, CinetPay
- **Cartes** : Stripe
- **Plans** : journalier, hebdomadaire, mensuel

---

## Modèle de sécurité

- Tunnels chiffrés avec les protocoles modernes (WireGuard, OpenVPN, IKEv2)
- Authentification JWT côté backend
- Politique no-logs pour le trafic utilisateur
- Kill switch pour éviter les fuites de connexion
- DNS sécurisé et anti-tracking
- Protection des clés et certificats sur les serveurs

---

## Scalabilité

- Ajout dynamique de serveurs VPN selon la charge
- Load balancing entre serveurs
- Mise en cache Redis pour les sessions et les métriques
- Déploiement conteneurisé avec Docker
- Monitoring continu et alertes

---

## Environnements

| Environnement | Usage | Statut |
| :--- | :--- | :--- |
| Local | Développement | Actif |
| Staging | Tests et recettes | À venir |
| Production | Déploiement public | À venir |

---

## Prochaines étapes documentaires

- [ ] Schéma détaillé de la base de données
- [ ] Diagrammes de séquence du flux de connexion VPN
- [ ] Spécification des endpoints API
- [ ] Matrice des rôles et permissions
- [ ] Plan de déploiement et de monitoring des serveurs
