# **ÉNONCÉ DU RAPPORT - SEMAINE 4**

## **STREAMFLEX - RAPPORT D'AVANCEMENT SEMAINE 4**

### **Objectif :** Implémenter la persistance des données et l'authentification

---

## **INTRODUCTION**

**Chers équipes StreamFlex,**

Félicitations pour le déploiement de votre première version ! Cette semaine, nous ajoutons deux composants **essentiels** à toute application moderne : **la base de données et l'authentification**. Votre mission : donner une mémoire à StreamFlex !

---

## **CE QUI EST ATTENDU CETTE SEMAINE**

### **Objectifs Principaux :**

```bash
1. "Maîtriser RDS et les bases de données cloud"
2. "Implémenter l'authentification utilisateur"
3. "Créer les modèles de données pour StreamFlex"
```

---

## **CONTENU DU RAPPORT À REMETTRE**

### **1. RAPPORT BASE DE DONNÉES RDS**

**Format :** Document PDF détaillant votre architecture données

```markdown
## NOTRE BASE DE DONNÉES STREAMFLEX

### Instance RDS Créée :

- [ ] `streamflex-db` - Instance RDS PostgreSQL/MySQL
- [ ] **Type :** db.t3.micro (Free Tier)
- [ ] **Moteur :** PostgreSQL ou MySQL
- [ ] **Région :** Canada Central (ca-central-1)

### Configuration Base de Données :

- [ ] Base créée avec nom : `streamflex_db`
- [ ] Utilisateur DB créé : `streamflex_user`
- [ ] Connexion sécurisée depuis l'EC2
- [ ] Sauvegardes automatiques configurées

### Modèle de Données :

- [ ] Table `users` : id, email, password_hash, created_at
- [ ] Table `videos` : id, user_id, title, description, s3_key, created_at
- [ ] Au moins 2 tables avec relations définies
```

### **2. SYSTÈME D'AUTHENTIFICATION**

**Format :** Code + démonstration

```markdown
## NOTRE AUTHENTIFICATION STREAMFLEX

### Fonctionnalités Implémentées :

- [ ] Inscription utilisateur (email/mot de passe)
- [ ] Connexion utilisateur
- [ ] Sessions utilisateur
- [ ] Déconnexion
- [ ] Middleware de protection des routes

### Sécurité :

- [ ] Mots de passe hashés (bcrypt)
- [ ] JWT ou sessions sécurisées
- [ ] Validation des inputs
- [ ] Protection contre les injections SQL

### Routes API :

- [ ] `POST /api/auth/register` - Inscription
- [ ] `POST /api/auth/login` - Connexion
- [ ] `POST /api/auth/logout` - Déconnexion
- [ ] `GET /api/auth/me` - Profil utilisateur
```

### **3. INTÉGRATION APPLICATION**

**Format :** Code + captures d'écran

```markdown
## NOTRE APPLICATION AVEC DONNÉES

### Pages Protégées :

- [ ] Tableau de bord utilisateur (après connexion)
- [ ] Page de profil utilisateur
- [ ] Interface d'upload vidéo (connexion requise)

### Fonctionnalités Liées :

- [ ] Les vidéos sont associées à l'utilisateur connecté
- [ ] Chaque utilisateur voit seulement ses vidéos
- [ ] Persistance des données entre les sessions

### Test de Fonctionnement :

- [ ] Création de compte fonctionnelle
- [ ] Connexion/déconnexion opérationnelle
- [ ] Données persistées en base
```

### **4. JOURNAL DE BORD ÉQUIPE**

**Format :** Tableau des réalisations et défis

```markdown
## NOTRE SEMAINE EN BREF

### Répartition des Tâches :

| Membre | Rôle Principal      | Tâches Accomplies                         |
| ------ | ------------------- | ----------------------------------------- |
| [Nom]  | Database Architect  | Configuration RDS, modèles de données     |
| [Nom]  | Backend Auth        | Implémentation authentification, sécurité |
| [Nom]  | Frontend            | Interfaces connexion, gestion sessions    |
| [Nom]  | Integration & Tests | Tests end-to-end, documentation           |

### Défis Techniques Rencontrés :

- [ ] "Problème avec [décrire le défi technique]"
- [ ] "Solution apportée : [expliquer la solution]"
- [ ] "Leçon apprise : [partager l'apprentissage]"

### Réunions d'Équipe :

- [ ] Lundi [date] - Modélisation données (60 min)
- [ ] Mercredi [date] - Intégration auth (60 min)
- [ ] Vendredi [date] - Tests et finalisation (45 min)
```

---

## **CAPTURES D'ÉCRAN OBLIGATOIRES**

**Format :** Images annotées des réalisations

```bash
"Capture 1" → Console RDS montrant votre instance running
"Capture 2" → Page d'inscription StreamFlex
"Capture 3" → Page de connexion fonctionnelle
"Capture 4" → Tableau de bord utilisateur connecté
"Capture 5" → Données en base (via pgAdmin ou autre)
"Capture 6" → Code des modèles de données
```

---

## **FORMAT DE REMISE**

### **Structure du Dossier :**

```
StreamFlex-Semaine4-GroupeX/
├── Rapport-Semaine4-GroupeX.pdf
├── Database/
│   ├── schema.sql (structure des tables)
│   ├── seed-data.sql (données de test)
│   └── README.md (instructions connexion)
├── Auth/
│   ├── auth-routes.js
│   ├── middleware-auth.js
│   └── password-utils.js
├── Screenshots/
│   ├── rds-instance.png
│   ├── signup-page.png
│   ├── login-page.png
│   ├── user-dashboard.png
│   └── database-tables.png
└── Journal-Bord-GroupeX.md
```

### **Modalités :**

```bash
"Format : Archive ZIP sur Moodle"
"Nommage : StreamFlex-Semaine4-GroupeX.zip"
"Date limite : Vendredi 18h00"
```

---

## **CONSEILS POUR RÉUSSIR**

### **Base de Données RDS :**

```bash
"Commencez avec PostgreSQL (meilleur support JSON)"
"Configurez le Security Group pour autoriser seulement votre EC2"
"Utilisez db.t3.micro pour rester dans le Free Tier"
```

### **Authentification :**

```bash
"Utilisez bcrypt pour le hashage des mots de passe"
"JWT pour les tokens ou sessions express"
"Validez TOUS les inputs utilisateur"
```

### **Sécurité :**

```bash
"Ne stockez JAMAIS de mots de passe en clair"
"Utilisez des variables d'environnement pour les secrets"
"Préparez vos requêtes SQL (anti-injection)"
```

---

## **RESSOURCES UTILES**

### **Documentation AWS :**

```bash
"RDS Getting Started : https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_GettingStarted.html"
"PostgreSQL on RDS : https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/CHAP_PostgreSQL.html"
```
