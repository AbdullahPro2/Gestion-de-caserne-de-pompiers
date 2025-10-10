# Gestion de caserne de pompiers

<img width="1366" height="725" alt="Capture d’écran (19)" src="https://github.com/user-attachments/assets/3a451b13-a899-41ae-bfa6-871397708f2d" />

Projet développé en 5 semaines par un groupe de 3 étudiants dans le cadre de leur formation.

## Fonctionnalités
- **Gestion des ressources humaines** : Consultation profils pompiers, habilitations, grades, affectations
- **Tableau de bord missions** : Visualisation, clôture et génération PDF
- **Création de nouvelles missions** 
- **Gestion des engins** : Liaison données véhicules-caserne
- **Statistiques**
- **Système d'authentification** : admin

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


## 🛠 Technologies Utilisées
- **C# .NET** - Windows Forms
- **SQLite** - Base de données relationnelle
- **iTextSharp** - Génération de rapports PDF
- **Git** - Gestion collaborative de version

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


## 🏗 Architecture
- **Mode déconnecté** : `MesDatas.cs` pour les opérations batch
- **Mode connecté** : `Connexion.cs` pour les opérations temps réel
- **UserControls modulaires** : Chargement dynamique dans `pnlMainLayout`
- **Classes utilitaires** : `GenerateurPdf`, `HabilitationItem`

---


Ce README reflète fidèlement votre projet tel que documenté dans vos rapports ! 🎯
