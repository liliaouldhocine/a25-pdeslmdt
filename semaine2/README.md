# **ÉNONCÉ DU RAPPORT - SEMAINE 2**

## **STREAMFLEX - RAPPORT D'AVANCEMENT SEMAINE 2**

### **Objectif :** Mettre en place les fondations sécurité et réseau

---

## **CE QUI EST ATTENDU CETTE SEMAINE**

### **Objectifs Principaux :**

```bash
1. "Maîtriser IAM et la sécurité AWS"
2. "Comprendre et créer une architecture réseau VPC"
3. "Mettre en place les premières politiques de sécurité"
```

---

## **CONTENU DU RAPPORT À REMETTRE**

### **1. RAPPORT DE SÉCURITÉ IAM**

**Format :** Document PDF détaillant votre structure IAM

```markdown
## NOTRE ARCHITECTURE IAM

### Utilisateurs Créés :

- [ ] `streamflex-admin` - Compte administrateur sécurisé
- [ ] `streamflex-dev` - Compte développeur avec permissions limitées

### Groupes IAM :

- [ ] `StreamFlex-Admins` - Accès complet au projet
- [ ] `StreamFlex-Developers` - Permissions de développement
- [ ] `StreamFlex-Viewers` - Accès lecture seule

### Politiques Personnalisées :

- [ ] Politique "StreamFlex-EC2-Limited" → seulement t2.micro/t3.micro
- [ ] Politique "StreamFlex-S3-VideosOnly" → accès limité aux buckets vidéos

### Sécurité Renforcée :

- [ ] MFA activée sur tous les comptes
- [ ] Politique de mot de passe robuste configurée
- [ ] Clés d'accès sécurisées et stockées safe
```

### **2. DIAGRAMME RÉSEAU VPC**

**Format :** Image + explications (draw.io/Lucidchart)

```markdown
## NOTRE ARCHITECTURE RÉSEAU

### VPC Configuration :

- **Nom :** `streamflex-vpc`
- **CIDR :** `10.0.0.0/16`
- **Région :** Canada Central (ca-central-1)

### Sous-réseaux Créés :

- [ ] `public-subnet-1a` (10.0.1.0/24) - Zone ca-central-1a
- [ ] `public-subnet-1b` (10.0.2.0/24) - Zone ca-central-1b
- [ ] `private-subnet-1a` (10.0.3.0/24) - Zone ca-central-1a
- [ ] `private-subnet-1b` (10.0.4.0/24) - Zone ca-central-1b

### Éléments Clés :

- [ ] Internet Gateway attaché
- [ ] Tables de routage configurées
- [ ] Groupes de sécurité définis
```

### **3. JOURNAL DE BORD ÉQUIPE**

**Format :** Tableau des réalisations et défis

```markdown
## NOTRE SEMAINE EN BREF

### Répartition des Tâches :

| Membre | Rôle Principal   | Tâches Accomplies                      |
| ------ | ---------------- | -------------------------------------- |
| [Nom]  | Sécurité IAM     | Création utilisateurs, MFA, politiques |
| [Nom]  | Architecture VPC | Diagramme, création VPC, sous-réseaux  |
| [Nom]  | Documentation    | Rédaction rapport, captures d'écran    |
| [Nom]  | Coordination     | Réunions, suivi planning               |

### Défis Rencontrés :

- [ ] "Problème avec [décrire le défi technique]"
- [ ] "Solution apportée : [expliquer la solution]"
- [ ] "Leçon apprise : [partager l'apprentissage]"

### Réunions d'Équipe :

- [ ] Lundi [date] - Planning semaine (30 min)
- [ ] Mercredi [date] - Point technique (45 min)
- [ ] Vendredi [date] - Finalisation rapport (60 min)
```

### **4. CAPTURES D'ÉCRAN**

**Format :** Images annotées des réalisations

```bash
"Capture 1" → Console IAM montrant vos utilisateurs/groups
"Capture 2" → Console VPC montrant votre architecture
"Capture 3" → Console EC2 montrant la région Canada Central
"Capture 4" → Page de connexion MFA active
```

---

## **FORMAT DE REMISE**

### **Structure du Dossier :**

```
StreamFlex-Semaine2-GroupeX/
├── Rapport-Semaine2-GroupeX.pdf
├── Architecture-VPC-GroupeX.png
├── Politiques-IAM-GroupeX.pdf
├── Journal-Bord-GroupeX.md
└── Captures/
    ├── iam-structure.png
    ├── vpc-console.png
    ├── mfa-active.png
    └── region-canada.png
```

### **Modalités :**

```bash
"Format : Archive ZIP sur Moodle"
"Nommage : StreamFlex-Semaine2-GroupeX.zip"
"Date limite : Vendredi 18h00"
```

---

## **CONSEILS POUR RÉUSSIR**

### **Sécurité IAM :**

```bash
"Activez TOUJOURS MFA sur les comptes admin"
"Utilisez le principe du moindre privilège"
"Nommez clairement utilisateurs et groupes"
```

### **Réseau VPC :**

```bash
"Commencez simple : 1 subnet public, 1 subnet privé"
"Configurez les groupes de sécurité restrictifs"
"Utilisez draw.io pour des diagrammes professionnels"
```

### **Travail d'Équipe :**

```bash
"Répartissez les rôles selon les forces de chacun"
"Communiquez régulièrement sur l'avancement"
"Demandez de l'aide si vous bloquez plus de 30 minutes"
```

---

## **BONUS POUR LES ÉQUIPES AMBITIEUSES**

### **Éléments Optionnels :**

```bash
"Script de déploiement automatique du VPC"
"Politique IAM avancée avec conditions"
"Architecture multi-AZ complète"
"Documentation de procédures de sécurité"
```

---

## **RESSOURCES UTILES**

### **Documentation AWS :**

```bash
"IAM Getting Started : https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started.html"
"VPC Guide : https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html"
```

### **Outils Recommandés :**

```bash
"draw.io - pour les diagrammes d'architecture"
"Google Docs - collaboration en équipe"
"GitHub - versioning de la documentation"
```
