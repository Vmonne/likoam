# LIKOAM — Système de Gestion des Archives / Records Management System

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/VMONNE/likoam)
[![Licence](https://img.shields.io/badge/licence-GPL%20v3-green.svg)](LICENSE)
[![Plateforme](https://img.shields.io/badge/plateforme-Google%20Apps%20Script-yellow.svg)](https://script.google.com)
[![Statut](https://img.shields.io/badge/statut-bêta-orange.svg)]()

---

🇫🇷 [Français](#-français) | 🇬🇧 [English](#-english)

---

## 🇫🇷 Français

### 📋 Qu'est-ce que LIKOAM ?

LIKOAM est un système de gestion des archives courantes et intermédiaires, conçu pour les institutions qui veulent digitaliser la gestion de leurs documents tout en préparant la migration vers un SAE définitif. Likoam convient à toute sorte d’organisation : Ministères, collectivités, ONG, entreprises et organisations communautaires. Il fonctionne entièrement sur l'infrastructure Google Workspace (Google Sheets + Google Drive), ce qui le rend léger, accessible et facile à déployer sans installation de serveur.

---

### ✨ Fonctionnalités principales

#### 📊 Tableau de bord
- Statistiques en temps réel sur le statut des documents
- Alertes pour les documents approchant de leur échéance de conservation
- Accès rapide aux documents en attente de validation

#### 📤 Versement documentaire
- Versement de documents avec métadonnées (titre, catégorie, service/département)
- Upload automatique du fichier vers Google Drive organisé par service et catégorie de documents
- Génération instantanée d'un bordereau de versement

#### 🔍 Recherche et consultation
- Recherche avancée
- Consultation directe du document via prévisualisation Google Drive
- Résultats filtrés selon le service de l'agent (contrôle d'accès par rôle)

#### 🗄️ Coffre-fort des archives
- Documents validés avec application des règles de conservation (DUA)
- Calcul automatique des dates d'élimination
- Suivi du sort final : Destruction (D), Tri (T), Conservation permanente (C)
- Filtres par catégorie, service, sort final et échéance

#### 📋 Registre des bordereaux
- Génération automatique des bordereaux de versement
- Génération automatique des bordereaux d'élimination
- Documents imprimables prêts pour impression PDF
- Registre complet avec recherche et filtres

#### ⚙️ Panneau d'administration
- Gestion des agents (création, activation/désactivation, attribution des rôles)
- Configuration des services et départements
- Gestion des catégories avec durées de conservation (DUA) et sorts finaux
- Contrôle d'accès par rôle (Admin / Utilisateur)

---

### 🏗️ Architecture technique

| Composant | Technologie |
|-----------|-------------|
| Backend | Google Apps Script |
| Base de données | Google Sheets |
| Stockage fichiers | Google Drive |
| Frontend | HTML5 / CSS3 / Bootstrap 5 / Vanilla JS |
| Authentification | Système de code agent interne |
| Déploiement | Google Apps Script Web App |
  
---

### 📁 Structure du dépôt

```
likoam/
├── Code.gs              # Backend — Google Apps Script
├── Index.html           # Frontend — Application monopage
├── appsscript.json      # Manifeste Apps Script
├── README.md            # Ce fichier
└── LICENSE              # GPL v3
```

### 👩🏽‍💻 Auteure

**Victorine Monné Loua**
Archiviste digitale

- 🌐 Site web : [victorinemonne.com](https://victorinemonne.com)
- 💼 LinkedIn : [linkedin.com/in/victorine-monné](https://ci.linkedin.com/in/victorine-monn%C3%A9-0a3247b9)
- 🐙 GitHub : [github.com/VMONNE](https://github.com/VMONNE)
- 📧 Contact : likoamarchives@gmail.com

---

### 📄 Licence

Ce projet est sous licence **GNU General Public License v3.0** — voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

---

## 🇬🇧 English

### 📋 What is LIKOAM?

LIKOAM is a web-based current and semi-current records management system built for institutions seeking to digitize their records management practices while preparing for eventual transfer to a permanent archival repository. It is suitable for organizations of all types and sizes — government ministries, local authorities, NGOs, corporations, and community organizations.
LIKOAM runs entirely on Google Workspace infrastructure (Google Sheets + Google Drive), making it lightweight, cost-effective, and straightforward to deploy — no server, no IT department required.

---
✨ Core Features
📊 Dashboard

Live overview of records status across the institution
Automated alerts for records approaching end of retention period
Quick access to records pending appraisal and validation

📤 Accession

Register incoming records with full descriptive metadata (title, category, creating department)
Automatic upload and filing to Google Drive, organized by department and record series
Instant generation of a transfer form upon accession

🔍 Search & Retrieval

Advanced search across multiple fields (title, creator, department, record series, status)
Direct document access via Google Drive preview
Access restricted by department and user role

🗄️ Archival Repository

Validated records managed according to approved retention schedules
Automatic calculation of disposal dates based on retention periods
Disposition tracking: Destruction (D), Review (T), Permanent Preservation (C)
Filtering by record series, department, disposition action, and disposal date

📋 Records Registers

Automatic generation of transfer forms
Automatic generation of disposal authorization forms
Print-ready documents for official records
Searchable and filterable register of all transfers and disposals

⚙️ Administration

User management (registration, activation/deactivation, role assignment)
Department and service configuration
Record series management with retention periods and disposition actions
Role-based access control (Administrator / User)

---

### 🏗️ Technical Architecture

| Component | Technology |
|-----------|-----------|
| Backend | Google Apps Script |
| Database | Google Sheets |
| File Storage | Google Drive |
| Frontend | HTML5 / CSS3 / Bootstrap 5 / Vanilla JS |
| Authentication | Internal agent code system |
| Deployment | Google Apps Script Web App |


### 📁 Repository Structure

```
likoam/
├── Code.gs              # Backend — Google Apps Script
├── Index.html           # Frontend — Single page application
├── appsscript.json      # Apps Script manifest
├── README.md            # This file
└── LICENSE              # GPL v3
```

---

### 👩🏽‍💻 Author

**Victorine Monné Loua**
Digital Archivist

- 🌐 Website: [victorinemonne.com](https://victorinemonne.com)
- 💼 LinkedIn: [linkedin.com/in/victorine-monné](https://ci.linkedin.com/in/victorine-monn%C3%A9-0a3247b9)
- 🐙 GitHub: [github.com/VMONNE](https://github.com/VMONNE)
- 📧 Contact: likoamarchives@gmail.com

---

### 📄 License

This project is licensed under the **GNU General Public License v3.0** — see the [LICENSE](LICENSE) file for details.

---

