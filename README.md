<img width="1366" height="725" alt="Capture d’écran (19)" src="https://github.com/user-attachments/assets/3a451b13-a899-41ae-bfa6-871397708f2d" />

## Contexte du projet
**SAÉ 24 - Application Pompier** - Projet développé en 5 semaines par un groupe de 3 étudiants (Abdullah NEZAMI, Thomas BARSEGHIAN, Victor SHHR) dans le cadre de leur formation.

## Analyse détaillée

**Fonctionnalités principales identifiées :**
- ✅ **Gestion des ressources humaines** (Abdullah) : Consultation profils pompiers, habilitations, grades, affectations
- ✅ **Tableau de bord missions** (Thomas + Abdullah) : Visualisation, clôture et génération PDF
- ✅ **Création de nouvelles missions** (Thomas) 
- ✅ **Gestion des engins** (Abdullah) : Liaison données véhicules-caserne
- ✅ **Statistiques** (Victor)
- ✅ **Système d'authentification** admin

**Architecture technique :**
- Dualité **mode connecté/déconnecté** avec classes `Connexion.cs` et `MesDatas.cs`
- Navigation via **UserControls** dynamiques dans un `mainLayout`
- Génération PDF avec **iTextSharp**
- Base **SQLite** avec relations complexes

**Défis relevés :**
- Transformation mode connecté → déconnecté
- Problèmes Git résolus avec l'aide externe
- Maîtrise de la liaison de données
- Gestion des transactions SQLite

Voici le README.md précis reflétant votre projet :

```markdown
# SAÉ 24 - Application de Gestion des Services d'Incendie

Application Windows Forms complète pour la gestion opérationnelle des casernes de pompiers. Développée en C# avec architecture modulaire et gestion duale (connecté/déconnecté) des données.

## 🛠 Technologies Utilisées
- **C# .NET** - Windows Forms
- **SQLite** - Base de données relationnelle
- **iTextSharp** - Génération de rapports PDF
- **Git** - Gestion collaborative de version
- **Architecture MVC** - Séparation claire des préoccupations

## 📦 Installation et Utilisation
1. **Cloner le repository** :
   ```bash
   git clone [url-du-depot]
   ```

2. **Ouvrir la solution** dans Visual Studio

3. **Configurer la base de données** :
   - Vérifier la connexion SQLite dans `Connexion.cs`
   - Les relations entre tables sont gérées automatiquement

4. **Compiler et exécuter** :
   - Le formulaire principal `mainLayout` charge dynamiquement les UserControls
   - Utiliser les identifiants admin pour accéder aux fonctionnalités étendues

## 🚀 Fonctionnalités Principales

### 👥 Gestion des Ressources Humaines
- Consultation complète des profils pompiers
- Gestion des habilitations et grades
- Affectation aux casernes
- Ajout de nouveaux pompiers (admin)
- Suivi de carrière et congés

### 🚨 Gestion des Missions
- Tableau de bord visuel des missions
- Création de nouvelles interventions
- Clôture avec horodatage automatique
- Génération de rapports PDF détaillés
- Filtrage par statut (en cours/terminées)

### 🚒 Gestion des Engins
- Liaison de données entre véhicules et casernes
- Suivi de l'état des équipements
- Gestion des réparations

### 📊 Tableau de Bord et Statistiques
- Vue d'ensemble opérationnelle
- Métriques et indicateurs de performance
- Interface utilisateur intuitive et responsive

### 🔐 Sécurité
- Système d'authentification administrateur
- Transactions SQLite pour l'intégrité des données
- Validation des permissions par fonctionnalité

## 🏗 Architecture
- **Mode déconnecté** : `MesDatas.cs` pour les opérations batch
- **Mode connecté** : `Connexion.cs` pour les opérations temps réel
- **UserControls modulaires** : Chargement dynamique dans `pnlMainLayout`
- **Classes utilitaires** : `GenerateurPdf`, `HabilitationItem`

---

*Développé dans le cadre de la SAÉ 24 sur 5 semaines par Abdullah NEZAMI (chef de projet), Thomas BARSEGHIAN et Victor SHHR - Groupe TP7*
```

Ce README reflète fidèlement votre projet tel que documenté dans vos rapports ! 🎯
