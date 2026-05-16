# LIKOAM — Système de Gestion des Archives / Records Management System

> **L**ogiciel **I**ntégré de gestion des archives **C**ourantes et intermédiaires **O**pérationnelles et **A**dministratives **M**odernes

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/VMONNE/likoam)
[![Licence](https://img.shields.io/badge/licence-GPL%20v3-green.svg)](LICENSE)
[![Plateforme](https://img.shields.io/badge/plateforme-Google%20Apps%20Script-yellow.svg)](https://script.google.com)
[![Statut](https://img.shields.io/badge/statut-bêta-orange.svg)]()

---

🇫🇷 [Français](#-français) | 🇬🇧 [English](#-english)

---

## 🇫🇷 Français

### 📋 Qu'est-ce que LIKOAM ?

LIKOAM est un système de gestion des archives courantes et intermédiaires accessible via le web, conçu pour les institutions de toute taille — ministères, collectivités locales, ONG, entreprises et organisations communautaires. Il fonctionne entièrement sur l'infrastructure Google Workspace (Google Sheets + Google Drive), ce qui le rend léger, accessible et facile à déployer sans aucune installation de serveur.

LIKOAM a été conçu par une archiviste, pour les archivistes — avec une compréhension approfondie des normes archivistiques et des réalités du travail en environnement à ressources limitées.

---

### ✨ Fonctionnalités principales

#### 📊 Tableau de bord
- Statistiques en temps réel sur le statut des documents
- Alertes pour les documents approchant de leur échéance de conservation
- Accès rapide aux documents en attente de validation

#### 📤 Versement documentaire
- Versement de documents avec métadonnées (titre, catégorie, service/département)
- Upload automatique du fichier vers Google Drive
- Génération instantanée d'un bordereau de versement

#### 🔍 Recherche et consultation
- Recherche multicritères (titre, agent, service, catégorie, statut)
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

**Aucun serveur requis. Aucune installation. Aucun coût de maintenance.**

---

### 🚀 Démarrage rapide

#### Prérequis
- Un compte Google
- Accès à Google Sheets et Google Drive
- Notions de base sur le déploiement Google Apps Script

#### Étapes de déploiement

1. **Créer le Google Sheet**
   - Créer un nouveau Google Sheet avec les onglets suivants :
     - `Sheet1` (feuille principale des documents)
     - `Agents`
     - `SERVICES`
     - `Référence DUA`
     - `BORDEREAUX`

2. **Configurer Apps Script**
   - Ouvrir le Google Sheet → Extensions → Apps Script
   - Créer un fichier `Code.gs` et coller le code backend
   - Créer un fichier `Index.html` et coller le code frontend

3. **Configurer le manifeste**
   - Activer le fichier `appsscript.json` dans les Paramètres du projet
   - Ajouter les scopes OAuth nécessaires

4. **Déployer en tant qu'application Web**
   - Cliquer sur Déployer → Nouveau déploiement
   - Type : Application Web
   - Exécuter en tant que : Moi
   - Accès : Tout le monde
   - Copier l'URL de déploiement

5. **Créer votre premier agent Admin**
   - Ouvrir la feuille `Agents`
   - Ajouter une ligne : Nom, CodeAgent, Actif, Service, Email, Admin

6. **Accéder à l'application**
   - Ouvrir l'URL de déploiement
   - Saisir votre code agent
   - Cliquer sur SE CONNECTER

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

---

### 🌍 Internationalisation

LIKOAM v1.0 est disponible en **français**.

Traductions prévues :
- 🇬🇧 Anglais — en cours
- 🇧🇷 Portugais — en cours

Les contributions pour les traductions sont les bienvenues !

---

### 🗺️ Feuille de route

#### V1.0 (Version actuelle)
- [x] Workflow de versement et validation des documents
- [x] Recherche multicritères
- [x] Gestion des règles de conservation (DUA)
- [x] Bordereaux d'élimination et de versement
- [x] Contrôle d'accès par rôle
- [x] Interface responsive mobile

#### V2.0 (En développement)
- [ ] Stack Python / Flask / SQLite
- [ ] Fonctionnement entièrement hors ligne
- [ ] Déploiement en réseau local (sans internet)
- [ ] Indexation OCR des documents
- [ ] Classification assistée par IA (RAG)
- [ ] Support multi-institutions
- [ ] API REST

---

### 🤝 Contribuer

LIKOAM est un projet open source né d'une pratique archivistique réelle. Les contributions sont les bienvenues !

1. Forker le dépôt
2. Créer une branche (`git checkout -b feature/NouvelleFonctionnalite`)
3. Commiter vos modifications (`git commit -m 'Ajout nouvelle fonctionnalité'`)
4. Pousser la branche (`git push origin feature/NouvelleFonctionnalite`)
5. Ouvrir une Pull Request

---

### 👩🏽‍💻 Auteure

**Victorine Monné Kpan**
Conservateur d'Archives | Gestionnaire de documents | Développeuse

- 🌐 Site web : [victorinemonne.com](https://victorinemonne.com)
- 💼 LinkedIn : [linkedin.com/in/victorine-monné](https://ci.linkedin.com/in/victorine-monn%C3%A9-0a3247b9)
- 🐙 GitHub : [github.com/VMONNE](https://github.com/VMONNE)
- 📧 Contact : likoamarchives@gmail.com

---

### 📄 Licence

Ce projet est sous licence **GNU General Public License v3.0** — voir le fichier [LICENSE](LICENSE) pour plus de détails.

---

*LIKOAM — Parce que chaque document mérite d'être correctement géré.*

---
---

## 🇬🇧 English

### 📋 What is LIKOAM?

LIKOAM is a web-based **records and archives management system** designed for institutions of all sizes — ministries, local authorities, NGOs, companies, and community organizations. It runs entirely on Google Workspace infrastructure (Google Sheets + Google Drive), making it lightweight, accessible, and easy to deploy without any server installation.

LIKOAM was designed by an archivist, for archivists — with a deep understanding of archival science standards and the realities of working in under-resourced environments.

---

### ✨ Key Features

#### 📊 Dashboard
- Real-time statistics on document status
- Alerts for documents nearing their retention deadline
- Quick access to documents pending validation

#### 📤 Document Submission
- Submit documents with metadata (title, category, service/department)
- Automatic file upload to Google Drive
- Instant generation of a submission receipt

#### 🔍 Search & Retrieval
- Multi-criteria search (title, agent, service, category, status)
- Direct document consultation via Google Drive preview
- Results limited to the agent's own service (role-based access)

#### 🗄️ Archives Vault
- Validated documents with applied retention rules (DUA)
- Automatic calculation of elimination dates
- Final disposition tracking: Destruction (D), Sorting (T), Permanent Conservation (C)
- Filters by category, service, disposition, and deadline

#### 📋 Registers
- Automatic generation of submission records
- Automatic generation of elimination records
- Printable PDF-ready documents
- Complete register with search and filter capabilities

#### ⚙️ Administration Panel
- Agent management (create, activate/deactivate, role assignment)
- Service and department configuration
- Category management with retention periods (DUA) and final disposition
- Role-based access control (Admin / User)

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

**No server required. No installation. No maintenance costs.**

---

### 🚀 Getting Started

#### Prerequisites
- A Google account
- Access to Google Sheets and Google Drive
- Basic knowledge of Google Apps Script deployment

#### Deployment Steps

1. **Create the Google Sheet**
   - Create a new Google Sheet with the following tabs:
     - `Sheet1` (main documents sheet)
     - `Agents`
     - `SERVICES`
     - `Référence DUA`
     - `BORDEREAUX`

2. **Set up Apps Script**
   - Open your Google Sheet → Extensions → Apps Script
   - Create a new file `Code.gs` and paste the backend code
   - Create a new file `Index.html` and paste the frontend code

3. **Configure the manifest**
   - Enable the `appsscript.json` manifest file in Project Settings
   - Add the required OAuth scopes

4. **Deploy as Web App**
   - Click Deploy → New Deployment
   - Type: Web App
   - Execute as: Me
   - Who has access: Anyone
   - Copy the deployment URL

5. **Create your first Admin agent**
   - Open your `Agents` sheet
   - Add a row with: Name, AgentCode, Actif, Service, Email, Admin

6. **Access the application**
   - Open the deployment URL
   - Enter your agent code
   - Click SE CONNECTER

---

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

### 🌍 Internationalization

LIKOAM v1.0 is available in **French**.

Planned translations:
- 🇬🇧 English — in progress
- 🇧🇷 Portuguese — in progress

Contributions for translations are welcome!

---

### 🗺️ Roadmap

#### V1.0 (Current)
- [x] Document submission and validation workflow
- [x] Multi-criteria search
- [x] Retention rules (DUA) management
- [x] Elimination and submission records
- [x] Role-based access control
- [x] Mobile responsive interface

#### V2.0 (In Development)
- [ ] Python / Flask / SQLite stack
- [ ] Full offline capability
- [ ] Local network deployment (no internet required)
- [ ] OCR document indexing
- [ ] AI-assisted classification (RAG)
- [ ] Multi-institution support
- [ ] REST API

---

### 🤝 Contributing

LIKOAM is an open-source project born from real archival practice. Contributions are welcome!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

### 👩🏽‍💻 Author

**Victorine Monné Kpan**
Conservateur d'Archives | Records Manager | Developer

- 🌐 Website: [victorinemonne.com](https://victorinemonne.com)
- 💼 LinkedIn: [linkedin.com/in/victorine-monné](https://ci.linkedin.com/in/victorine-monn%C3%A9-0a3247b9)
- 🐙 GitHub: [github.com/VMONNE](https://github.com/VMONNE)
- 📧 Contact: likoamarchives@gmail.com

---

### 📄 License

This project is licensed under the **GNU General Public License v3.0** — see the [LICENSE](LICENSE) file for details.

---

*LIKOAM — Because every document deserves to be properly managed.*
