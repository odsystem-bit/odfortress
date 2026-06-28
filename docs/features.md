# Fonctionnalités OD Fortress

Ce document détaille les fonctionnalités principales d'OD Fortress, organisées par module et par plan d'abonnement.

> **Statut** : En cours de documentation. Les placeholders seront remplacés par des spécifications détaillées.

---

## 1. Module Connexion VPN

- Connexion en un clic
- Sélection automatique du serveur le plus proche
- Sélection manuelle du pays/du serveur
- Reconnexion automatique
- Indicateur de statut et de vitesse

## 2. Module Sécurité

- Chiffrement des tunnels (WireGuard, OpenVPN, IKEv2)
- Kill switch (coupure internet si VPN tombe)
- Split tunneling (sélection des applications VPN)
- DNS sécurisé
- Protection contre les fuites DNS, IPv6 et WebRTC

## 3. Module Vie privée

- Politique no-logs
- Anti-tracking
- Bloqueur de publicités et de traqueurs
- Mode furtif (roadmap)

## 4. Module Abonnements

| Plan | Durée | Fonctionnalités clés |
| :--- | :--- | :--- |
| Gratuit | Limité | 500 Mo/jour, 1 serveur |
| Journalier | 24h | Accès complet, tous les serveurs |
| Hebdomadaire | 7 jours | Accès complet, tous les serveurs |
| Mensuel | 30 jours | Accès complet, tous les serveurs, support |
| Entreprise | Sur devis | Multi-utilisateurs, IP dédiée, support prioritaire |

## 5. Module Paiement

- Paiement Mobile Money (MTN, Moov, Wave)
- Paiement par carte (Stripe)
- Renouvellement automatique
- Historique des paiements
- Gestion des remboursements

## 6. Module Dashboard

- Historique des connexions
- Consommation de données
- Gestion des appareils liés
- Gestion de l'abonnement
- Support client

## 7. Module Panel Admin

- Gestion des serveurs VPN
- Supervision des utilisateurs et abonnements
- Statistiques de bande passante
- Alertes et monitoring
- Support et tickets

---

## Matrice plans / fonctionnalités

| Fonctionnalité | Gratuit | Journalier/Hebdo/Mensuel | Entreprise |
| :--- | :--- | :--- | :--- |
| VPN de base | :white_check_mark: | :white_check_mark: | :white_check_mark: |
| Tous les serveurs | :x: | :white_check_mark: | :white_check_mark: |
| Kill switch | :x: | :white_check_mark: | :white_check_mark: |
| Split tunneling | :x: | :white_check_mark: | :white_check_mark: |
| Anti-tracking | :x: | :white_check_mark: | :white_check_mark: |
| Support prioritaire | :x: | :x: | :white_check_mark: |
| IP dédiée | :x: | :x: | :white_check_mark: |

---

## Prochaines étapes

- [ ] Spécifications détaillées de chaque module
- [ ] Maquettes et parcours utilisateurs
- [ ] Dictionnaire des données
- [ ] Tests d'acceptation par module
