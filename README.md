<div align="center">
  <img src="assets/banner.svg" alt="OD Fortress Banner" width="100%" />
</div>

<div align="center">
  <img src="assets/logo/logo-placeholder.svg" alt="OD Fortress Logo" width="120" height="120" />
  <h1>OD Fortress</h1>
  <p><strong>VPN et sécurité réseau pour l'Afrique francophone</strong></p>
  <p>
    <img src="https://img.shields.io/badge/Status-En%20développement-2A8A1A?style=flat-square" alt="Status" />
    <img src="https://img.shields.io/badge/Version-0.1.0-1D3C6E?style=flat-square" alt="Version" />
    <img src="https://img.shields.io/badge/License-MIT-F5A800?style=flat-square" alt="License" />
    <img src="https://img.shields.io/badge/Marché-Afrique%20francophone-1D3C6E?style=flat-square" alt="Marché" />
  </p>
</div>

---

## Table des matières

- [Présentation](#présentation)
- [Le problème](#le-problème)
- [La solution](#la-solution)
- [Fonctionnalités principales](#fonctionnalités-principales)
- [Architecture générale](#architecture-générale)
- [Technologies utilisées](#technologies-utilisées)
- [Feuille de route](#feuille-de-route)
- [Captures d'écran](#captures-décran)
- [Démo](#démo)
- [Liens officiels](#liens-officiels)
- [Contact](#contact)

---

## Présentation

**OD Fortress** est une solution de VPN et de sécurité réseau conçue pour le marché africain francophone. Elle permet aux utilisateurs de naviguer de manière sécurisée, de contourner les restrictions géographiques et de protéger leur vie privée sur les réseaux Wi-Fi publics et mobile data.

OD Fortress vise à offrir une alternative abordable, accessible en Mobile Money et adaptée aux infrastructures locales.

---

## Le problème

En Afrique francophone, les utilisateurs d'internet rencontrent plusieurs obstacles :
- Coût élevé des VPN internationaux et paiement inaccessible par carte bancaire.
- Restrictions d'accès à certains contenus et services en ligne.
- Risques élevés sur les réseaux Wi-Fi publics (vol de données, espionnage).
- Manque de solutions VPN locales avec support et paiement adaptés.
- Surveillance et limitation de la liberté d'accès à l'information.

---

## La solution

OD Fortress propose une application VPN sécurisée avec :

- **Application Android** : connexion VPN en un clic avec serveurs optimisés.
- **Serveurs VPN** : infrastructure dédiée avec chiffrement moderne.
- **Protocoles sécurisés** : WireGuard, OpenVPN, IKEv2.
- **Politique no-logs** : aucune trace de navigation conservée.
- **Kill switch** : coupure automatique de l'internet si le VPN tombe.
- **Paiement Mobile Money** : abonnements en FCFA via MTN, Moov, Wave.
- **Support local** : assistance en français et dans les langues locales.

---

## Fonctionnalités principales

- **VPN rapide et sécurisé** : connexion en un clic avec serveurs proches.
- **Chiffrement fort** : protection des données sur tous les réseaux.
- **No-logs** : aucune collecte de données de navigation.
- **Kill switch** : protection contre les fuites de connexion.
- **Split tunneling** : choix des applications utilisant le VPN.
- **DNS sécurisé** : protection contre le phishing et les malwares.
- **Anti-tracking** : blocage des traqueurs et publicités.
- **Multi-serveurs** : accès à plusieurs pays et régions.
- **Abonnements flexibles** : plans journalier, hebdomadaire, mensuel.
- **Paiement Mobile Money** : abonnement accessible sans carte bancaire.
- **Tableau de bord** : suivi de la consommation, de l'abonnement et des appareils.

---

## Architecture générale

OD Fortress repose sur une architecture VPN client-serveur sécurisée :

- **Application Android** : Kotlin avec service VPN natif, UI moderne.
- **Serveurs VPN** : infrastructure Linux avec WireGuard, OpenVPN et IKEv2.
- **Backend API** : Node.js avec gestion des utilisateurs, abonnements et serveurs.
- **Paiement** : intégration Mobile Money et cartes bancaires.
- **Panel admin** : supervision des serveurs, utilisateurs et abonnements.
- **Monitoring** : surveillance des serveurs et de la bande passante.

Pour plus de détails, consulter :
- [`docs/architecture.md`](docs/architecture.md)
- [`docs/features.md`](docs/features.md)
- [`docs/business-model.md`](docs/business-model.md)
- [`docs/api.md`](docs/api.md)
- [`docs/faq.md`](docs/faq.md)

---

## Technologies utilisées

### Mobile
![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)

### Serveurs VPN
![WireGuard](https://img.shields.io/badge/WireGuard-88171A?style=for-the-badge&logo=wireguard&logoColor=white)
![OpenVPN](https://img.shields.io/badge/OpenVPN-EA7E20?style=for-the-badge&logo=openvpn&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)

### Backend
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)

### Outils
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

---

## Feuille de route

| Phase | Objectif | Statut |
| :--- | :--- | :--- |
| **Phase 1** | Application Android VPN de base avec WireGuard | En cours |
| **Phase 2** | Backend API, authentification et abonnements | À venir |
| **Phase 3** | Paiement Mobile Money et gestion des plans | À venir |
| **Phase 4** | Kill switch, split tunneling, DNS sécurisé | À venir |
| **Phase 5** | Panel admin, monitoring et support client | À venir |
| **Phase 6** | Expansion régionale et partenariats opérateurs | À venir |

Consulter [`ROADMAP.md`](ROADMAP.md) pour le détail.

---

## Captures d'écran

> Les captures d'écran seront ajoutées progressivement dans le dossier [`assets/screenshots/`](assets/screenshots/).

<div align="center">
  <img src="assets/screenshots/placeholder.svg" alt="Application OD Fortress placeholder" width="80%" />
  <p><em>Application OD Fortress — placeholder</em></p>
</div>

---

## Démo

Une démo publique sera disponible prochainement dans le dossier [`demo/`](demo/).

---

## Liens officiels

- **Site web** : [À compléter](https://)
- **Documentation** : [`docs/`](docs/)
- **Portfolio** : [stanislas-nouemou](https://github.com/odsystem-bit/stanislas-nouemou)
- **GitHub** : [odfortress](https://github.com/odsystem-bit/odfortress)

---

## Contact

Pour toute question, partenariat ou opportunité d'investissement :

- **Email** : [À compléter](mailto:)
- **LinkedIn** : [À compléter](https://linkedin.com/in/)
- **GitHub** : [@odsystem-bit](https://github.com/odsystem-bit)

---

<div align="center">
  <sub>OD Fortress — Votre accès internet, sécurisé et libre.</sub>
</div>
