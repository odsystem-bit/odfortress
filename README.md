<div align="center">
  <img src="assets/banner.svg" alt="OD Fortress Banner" width="100%" />
</div>

<div align="center">

<img src="assets/logo/logo-placeholder.svg" alt="OD Fortress Logo" width="120" height="120" style="border-radius:50%;border:4px solid #14C7B5;" />

# OD Fortress

### VPN et sécurité réseau pour l'Afrique francophone

<img src="https://img.shields.io/badge/Statut-En_développement-14C7B5?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/Version-0.1.0-0E8E82?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/Licence-MIT-1AB8AB?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/Marché-Afrique_francophone-0E8E82?style=flat-square&logoColor=white" />

</div>

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=14C7B5&height=120&section=header" width="100%"/>

## Table des matières

[![Présentation](https://img.shields.io/badge/Présentation-14C7B5?style=flat-square&logoColor=white)](#présentation)
[![Le problème](https://img.shields.io/badge/Le_problème-14C7B5?style=flat-square&logoColor=white)](#le-problème)
[![La solution](https://img.shields.io/badge/La_solution-14C7B5?style=flat-square&logoColor=white)](#la-solution)
[![Fonctionnalités](https://img.shields.io/badge/Fonctionnalités-14C7B5?style=flat-square&logoColor=white)](#fonctionnalités-principales)
[![Architecture](https://img.shields.io/badge/Architecture-14C7B5?style=flat-square&logoColor=white)](#architecture-générale)
[![Technologies](https://img.shields.io/badge/Technologies-14C7B5?style=flat-square&logoColor=white)](#technologies-utilisées)
[![Feuille de route](https://img.shields.io/badge/Feuille_de_route-14C7B5?style=flat-square&logoColor=white)](#feuille-de-route)
[![Captures d'écran](https://img.shields.io/badge/Captures_d'écran-14C7B5?style=flat-square&logoColor=white)](#captures-décran)
[![Démo](https://img.shields.io/badge/Démo-14C7B5?style=flat-square&logoColor=white)](#démo)
[![Liens officiels](https://img.shields.io/badge/Liens_officiels-14C7B5?style=flat-square&logoColor=white)](#liens-officiels)
[![Contact](https://img.shields.io/badge/Contact-14C7B5?style=flat-square&logoColor=white)](#contact)

<br/>

## Présentation

**OD Fortress** est une solution de VPN et de sécurité réseau conçue pour le marché africain francophone. Elle permet aux utilisateurs de naviguer de manière sécurisée, de contourner les restrictions géographiques et de protéger leur vie privée sur les réseaux Wi-Fi publics et en mobile data.

OD Fortress vise à offrir une alternative abordable, accessible en Mobile Money et adaptée aux infrastructures locales.

<br/>

## Le problème

<table>
<tr>
<td width="50%" valign="top">

### Accès et coût

Les VPN internationaux restent coûteux et leur paiement par carte bancaire est souvent inaccessible localement. Les utilisateurs font également face à des restrictions d'accès à certains contenus et services en ligne.

</td>
<td width="50%" valign="top">

### Sécurité et liberté

Les risques sur les réseaux Wi-Fi publics, vol de données et espionnage, restent élevés, tandis que le manque de solutions VPN locales avec support et paiement adaptés limite la liberté d'accès à l'information.

</td>
</tr>
</table>

<br/>

## La solution

OD Fortress propose une application VPN sécurisée pensée pour le contexte local.

Une application Android permet une connexion VPN en un clic avec des serveurs optimisés, appuyée sur une infrastructure dédiée au chiffrement moderne. Les protocoles sécurisés WireGuard, OpenVPN et IKEv2 garantissent la robustesse des connexions, sous une politique stricte de no-logs qui ne conserve aucune trace de navigation. Un kill switch coupe automatiquement internet si le VPN tombe, et le paiement se fait en Mobile Money, en FCFA, via MTN, Moov ou Wave. Un support local en français et dans les langues locales complète l'ensemble.

<br/>

## Fonctionnalités principales

<table>
<tr>
<td width="50%" valign="top">

### 🔐 Sécurité et confidentialité

Connexion VPN rapide en un clic avec serveurs proches, chiffrement fort sur tous les réseaux et politique no-logs garantissant l'absence de collecte des données de navigation. Le kill switch protège contre les fuites de connexion, et un DNS sécurisé bloque le phishing et les malwares, complété par un anti-tracking contre les traqueurs et publicités.

</td>
<td width="50%" valign="top">

### ⚙️ Flexibilité et contrôle

Split tunneling pour choisir précisément quelles applications passent par le VPN, accès multi-serveurs à plusieurs pays et régions, et abonnements flexibles en plans journalier, hebdomadaire ou mensuel. Le paiement Mobile Money rend l'abonnement accessible sans carte bancaire, avec un tableau de bord pour suivre consommation, abonnement et appareils connectés.

</td>
</tr>
</table>

Pour plus de détails, consulter la documentation complète :

<p>
<img src="https://img.shields.io/badge/docs/architecture.md-0E8E82?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/docs/features.md-0E8E82?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/docs/business_model.md-0E8E82?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/docs/api.md-0E8E82?style=flat-square&logoColor=white" />
<img src="https://img.shields.io/badge/docs/faq.md-0E8E82?style=flat-square&logoColor=white" />
</p>

<br/>

## Architecture générale

OD Fortress repose sur une architecture VPN client-serveur sécurisée, pensée pour la fiabilité et la simplicité d'usage.

L'application Android est développée en Kotlin avec un service VPN natif et une interface moderne. Les serveurs VPN tournent sur une infrastructure Linux avec WireGuard, OpenVPN et IKEv2. Le backend API en Node.js gère les utilisateurs, les abonnements et les serveurs, tandis que le paiement intègre à la fois le Mobile Money et les cartes bancaires. Un panel admin supervise serveurs, utilisateurs et abonnements, complété par un monitoring continu des serveurs et de la bande passante.

[![Documentation architecture](https://img.shields.io/badge/Documentation_complète-14C7B5?style=flat-square&logo=readthedocs&logoColor=white)](docs/architecture.md)

<br/>

## Technologies utilisées

<div align="center">

**Mobile**

<img src="https://img.shields.io/badge/Kotlin-14C7B5?style=for-the-badge&logo=kotlin&logoColor=white" />
<img src="https://img.shields.io/badge/Android-14C7B5?style=for-the-badge&logo=android&logoColor=white" />

**Serveurs VPN**

<img src="https://img.shields.io/badge/WireGuard-0E8E82?style=for-the-badge&logo=wireguard&logoColor=white" />
<img src="https://img.shields.io/badge/OpenVPN-0E8E82?style=for-the-badge&logo=openvpn&logoColor=white" />
<img src="https://img.shields.io/badge/Linux-0E8E82?style=for-the-badge&logo=linux&logoColor=white" />

**Backend**

<img src="https://img.shields.io/badge/Node.js-1AB8AB?style=for-the-badge&logo=node.js&logoColor=white" />
<img src="https://img.shields.io/badge/Express-1AB8AB?style=for-the-badge&logo=express&logoColor=white" />
<img src="https://img.shields.io/badge/PostgreSQL-1AB8AB?style=for-the-badge&logo=postgresql&logoColor=white" />

**Outils**

<img src="https://img.shields.io/badge/Docker-0A6B61?style=for-the-badge&logo=docker&logoColor=white" />
<img src="https://img.shields.io/badge/Git-0A6B61?style=for-the-badge&logo=git&logoColor=white" />
<img src="https://img.shields.io/badge/GitHub-0A6B61?style=for-the-badge&logo=github&logoColor=white" />

</div>

<br/>

## Feuille de route

<table>
<tr>
<td width="15%"><strong>Phase 1</strong></td>
<td width="65%">Application Android VPN de base avec WireGuard</td>
<td width="20%"><img src="https://img.shields.io/badge/En_cours-14C7B5?style=flat-square&logoColor=white" /></td>
</tr>
<tr>
<td><strong>Phase 2</strong></td>
<td>Backend API, authentification et abonnements</td>
<td><img src="https://img.shields.io/badge/À_venir-1AB8AB?style=flat-square&logoColor=white" /></td>
</tr>
<tr>
<td><strong>Phase 3</strong></td>
<td>Paiement Mobile Money et gestion des plans</td>
<td><img src="https://img.shields.io/badge/À_venir-1AB8AB?style=flat-square&logoColor=white" /></td>
</tr>
<tr>
<td><strong>Phase 4</strong></td>
<td>Kill switch, split tunneling, DNS sécurisé</td>
<td><img src="https://img.shields.io/badge/À_venir-1AB8AB?style=flat-square&logoColor=white" /></td>
</tr>
<tr>
<td><strong>Phase 5</strong></td>
<td>Panel admin, monitoring et support client</td>
<td><img src="https://img.shields.io/badge/À_venir-1AB8AB?style=flat-square&logoColor=white" /></td>
</tr>
<tr>
<td><strong>Phase 6</strong></td>
<td>Expansion régionale et partenariats opérateurs</td>
<td><img src="https://img.shields.io/badge/À_venir-1AB8AB?style=flat-square&logoColor=white" /></td>
</tr>
</table>

<p>
<img src="https://img.shields.io/badge/ROADMAP.md-14C7B5?style=flat-square&logoColor=white" />
</p>

<br/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=14C7B5&height=2&section=header" width="100%"/>

## Captures d'écran

<div align="center">

<sub>Les captures d'écran sont ajoutées progressivement dans le dossier <code>assets/screenshots/</code>.</sub>

<br/><br/>

<img src="assets/screenshots/placeholder.svg" alt="Application OD Fortress" width="80%" />

<p><em>Application OD Fortress</em></p>

</div>

<br/>

## Démo

Une démo publique sera disponible prochainement dans le dossier `demo/`.

<br/>

## Liens officiels

<div align="center">

[![Site web](https://img.shields.io/badge/Site_web-À_compléter-14C7B5?style=for-the-badge&logo=googlechrome&logoColor=white)](#)
[![Documentation](https://img.shields.io/badge/Documentation-14C7B5?style=for-the-badge&logo=readthedocs&logoColor=white)](docs/)
[![Portfolio](https://img.shields.io/badge/Portfolio-14C7B5?style=for-the-badge&logo=github&logoColor=white)](https://github.com/odsystem-bit/stanislas-nouemou)
[![Dépôt GitHub](https://img.shields.io/badge/Dépôt_GitHub-14C7B5?style=for-the-badge&logo=github&logoColor=white)](https://github.com/odsystem-bit/odfortress)

</div>

<br/>

<img src="https://capsule-render.vercel.app/api?type=rect&color=14C7B5&height=2&section=header" width="100%"/>

## Contact

<div align="center">

Pour toute question, partenariat ou opportunité d'investissement.

<br/>

[![Email](https://img.shields.io/badge/Email-À_compléter-14C7B5?style=for-the-badge&logo=gmail&logoColor=white)](mailto:)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-14C7B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/)
[![GitHub](https://img.shields.io/badge/@odsystem--bit-14C7B5?style=for-the-badge&logo=github&logoColor=white)](https://github.com/odsystem-bit)

<br/><br/>

<sub>OD Fortress · Votre accès internet, sécurisé et libre</sub>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=14C7B5&height=100&section=footer" width="100%"/>
