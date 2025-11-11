# **ÉNONCÉ DU RAPPORT - SEMAINE 3**

## **STREAMFLEX - RAPPORT D'AVANCEMENT SEMAINE 3**

### **Objectif :** Déployer l'infrastructure de base et la première version de l'application

---

## **INTRODUCTION**

**Chers équipes StreamFlex,**

Félicitations pour la mise en place de vos fondations sécurité ! Cette semaine, nous passons à la **création de l'infrastructure de base** et au **déploiement de la première version de votre application**. Votre mission : faire vivre StreamFlex !

---

## **CE QUI EST ATTENDU CETTE SEMAINE**

### **Objectifs Principaux :**

```bash
1. "Maîtriser EC2 et le déploiement d'applications"
2. "Comprendre et utiliser S3 pour le stockage"
3. "Déployer la première version fonctionnelle de StreamFlex"
```

---

## **CONTENU DU RAPPORT À REMETTRE**

### **1. RAPPORT TECHNIQUE EC2 & APPLICATION**

**Format :** Document PDF détaillant votre infrastructure

```markdown
## NOTRE INFRASTRUCTURE EC2

### Instance Créée :

- [ ] `streamflex-app-server` - Instance EC2 pour l'application
- [ ] **Type :** t3.micro (Free Tier)
- [ ] **AMI :** Amazon Linux 2023 ou Ubuntu
- [ ] **Région :** Canada Central (ca-central-1)

### Configuration Serveur :

- [ ] Serveur web installé (Apache, Nginx ou Node.js)
- [ ] Application StreamFlex déployée
- [ ] Port d'écoute configuré (3000, 8080, ou 80)

### Accès et Sécurité :

- [ ] Connexion SSH fonctionnelle
- [ ] Security Group configuré pour HTTP/HTTPS
- [ ] Application accessible via IP publique
```

### **2. PREMIÈRE VERSION DE L'APPLICATION**

**Format :** Code + captures d'écran

```markdown
## NOTRE APPLICATION STREAMFLEX V1

### Fonctionnalités Implémentées :

- [ ] Page d'accueil avec présentation StreamFlex
- [ ] Interface basique de navigation
- [ ] Page "À propos" ou "Contact"
- [ ] Structure prête pour les vidéos

### Stack Technique :

- [ ] **Backend :** Node.js/Express ou autre
- [ ] **Frontend :** HTML/CSS/JS ou framework
- [ ] **Port :** [3000/8080/80] - spécifier lequel

### Accès à l'Application :

- **URL :** http://[VOTRE-IP-EC2]:[PORT]
- **Statut :** Application accessible publiquement
```

### **3. CONFIGURATION STOCKAGE S3**

**Format :** Description + captures console AWS

```markdown
## NOTRE ARCHITECTURE STOCKAGE S3

### Buckets Créés :

- [ ] `streamflex-videos-[équipe]` - Pour le stockage vidéo
- [ ] `streamflex-assets-[équipe]` - Pour les assets statiques

### Configuration Buckets :

- [ ] **Région :** Canada Central (ca-central-1)
- [ ] **Permissions :** Configurées sécuritairement
- [ ] **Versioning :** Activé ou désactivé

### Intégration Application :

- [ ] SDK AWS configuré dans l'application
- [ ] \*\*Test d'upload/download fonctionnel
```

### **4. JOURNAL DE BORD ÉQUIPE (10%)**

**Format :** Tableau des réalisations et défis

```markdown
## NOTRE SEMAINE EN BREF

### Répartition des Tâches :

| Membre | Rôle Principal | Tâches Accomplies                      |
| ------ | -------------- | -------------------------------------- |
| [Nom]  | Backend EC2    | Configuration serveur, déploiement app |
| [Nom]  | Frontend       | Développement interface StreamFlex     |
| [Nom]  | Storage S3     | Configuration buckets, intégration     |
| [Nom]  | Documentation  | Tests, rapport, captures d'écran       |

### Défis Techniques Rencontrés :

- [ ] "Problème avec [décrire le défi technique]"
- [ ] "Solution apportée : [expliquer la solution]"
- [ ] "Leçon apprise : [partager l'apprentissage]"

### Réunions d'Équipe :

- [ ] Lundi [date] - Planning développement (45 min)
- [ ] Mercredi [date] - Intégration et tests (60 min)
- [ ] Vendredi [date] - Finalisation rapport (45 min)
```

---

## **CAPTURES D'ÉCRAN OBLIGATOIRES**

**Format :** Images annotées des réalisations

```bash
"Capture 1" → Console EC2 montrant votre instance running
"Capture 2" → Application StreamFlex accessible via navigateur
"Capture 3" → Console S3 montrant vos buckets
"Capture 4" → Connexion SSH à votre instance
"Capture 5" → Code de votre application (au moins 1 fichier)
```

---

## **FORMAT DE REMISE**

### **Structure du Dossier (pas besoin d'avoir la même sructure d'application) :**

```
StreamFlex-Semaine3-GroupeX/
├── Rapport-Semaine3-GroupeX.pdf
├── Application/
│   ├── server.js (ou fichier principal)
│   ├── package.json
│   └── README.md (instructions déploiement)
├── Screenshots/
│   ├── ec2-instance.png
│   ├── app-browser.png
│   ├── s3-buckets.png
│   └── ssh-connection.png
└── Journal-Bord-GroupeX.md
```

### **Modalités :**

```bash
"Format : Archive ZIP sur Moodle"
"Nommage : StreamFlex-Semaine3-GroupeX.zip"
"Date limite : Vendredi 18h00"
```

---

## **CONSEILS POUR RÉUSSIR**

### **Déploiement EC2 :**

```bash
"Commencez simple : application 'Hello World' d'abord"
"Testez localement avant de déployer sur EC2"
"Utilisez PM2 pour garder l'application active"
```

### **Application StreamFlex :**

```bash
"Priorisez les fonctionnalités core : accueil, navigation"
"Interface simple mais professionnelle"
"Pensez responsive design"
```

### **Stockage S3 :**

```bash
"Créez des buckets avec des noms uniques"
"Configurez les permissions minimales nécessaires"
"Testez l'upload d'un fichier simple"
```

---

## **RESSOURCES UTILES**

### **Documentation AWS :**

```bash
"EC2 User Guide : https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html"
"S3 Getting Started : https://docs.aws.amazon.com/AmazonS3/latest/userguide/GetStartedWithS3.html"
"Node.js on EC2 : https://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/setting-up-node-on-ec2-instance.html"
```

### **Tutoriels Recommandés :**

```bash
"Déployer une app Node.js sur EC2"
"Configurer S3 avec SDK JavaScript"
"Sécuriser une instance EC2"
```
