# API OD Fortress

Ce document décrit l'API publique d'OD Fortress. Il est en cours de rédaction et sera enrichi au fur et à mesure du développement.

> **Statut** : Version préliminaire. Les endpoints, formats et authentification sont susceptibles d'évoluer.

---

## Introduction

L'API OD Fortress permet à l'application Android, au panel admin et aux systèmes de paiement d'interagir avec la plateforme. Elle repose sur une architecture RESTful avec authentification JWT.

---

## Authentification

> **À compléter** : méthode d'authentification détaillée.

```http
Authorization: Bearer {token}
```

---

## En-têtes communs

```http
Content-Type: application/json
Accept: application/json
Authorization: Bearer {token}
```

---

## Endpoints

### Authentification

| Méthode | Endpoint | Description |
| :--- | :--- | :--- |
| POST | `/api/v1/auth/register` | Créer un compte |
| POST | `/api/v1/auth/login` | Se connecter |
| POST | `/api/v1/auth/logout` | Se déconnecter |
| GET | `/api/v1/auth/me` | Profil connecté |

### Serveurs VPN

| Méthode | Endpoint | Description |
| :--- | :--- | :--- |
| GET | `/api/v1/servers` | Lister les serveurs disponibles |
| GET | `/api/v1/servers/{id}/config` | Obtenir la configuration VPN |

### Abonnements

| Méthode | Endpoint | Description |
| :--- | :--- | :--- |
| GET | `/api/v1/subscriptions` | Lister les plans |
| POST | `/api/v1/subscriptions` | Souscrire à un plan |
| GET | `/api/v1/subscriptions/current` | Abonnement actuel |

### Paiements

| Méthode | Endpoint | Description |
| :--- | :--- | :--- |
| POST | `/api/v1/payments/mobile-money` | Initier un paiement Mobile Money |
| POST | `/api/v1/payments/card` | Initier un paiement par carte |
| GET | `/api/v1/payments/history` | Historique des paiements |

---

## Codes de réponse

| Code | Signification |
| :--- | :--- |
| 200 | Succès |
| 201 | Ressource créée |
| 400 | Requête invalide |
| 401 | Non authentifié |
| 403 | Non autorisé |
| 404 | Ressource non trouvée |
| 422 | Erreur de validation |
| 500 | Erreur serveur |

---

## Prochaines étapes

- [ ] Définir les schémas complets de requête et réponse
- [ ] Rédiger les spécifications d'authentification
- [ ] Documenter les formats de configuration VPN
- [ ] Publier une collection Postman
