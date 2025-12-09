# SchreinSchedule - Le cerveau de votre automatisation

**Minuteur intelligent tout-en-un pour applications .NET Windows Forms**

SchreinSchedule - Minuteur intelligent .NET pour l'automatisation d'applications. Planification multi-tâches avancée avec déclencheurs conditionnels, commandes configurables et stratégies d'exécution flexibles. Parfait pour l'automatisation métier et le contrôle de processus.  #dotnet #automation #timer #scheduler #winforms

## 🌟 Fonctionnalités Principales

### ⏰ Planification Avancée
- **Déclencheurs multiples** : Dates programmées, heures spécifiques, récurrences
- **Fenêtres horaires** : Exécution uniquement dans des plages horaires définies
- **Calendrier intelligent** : Jours de semaine, patterns mensuels, exclusions de dates
- **Stratégies flexibles** : Récurrente, Calendrier, TimeWindow, Mixte

### 🤖 Automatisation Conditionnelle
- **Commandes intelligentes** : Exécution basée sur l'état de l'interface
- **Conditions complexes** : Support des opérateurs logiques ET/OU et parenthèses
- **Monitoring temps réel** : Réaction aux changements des valeurs des contrôles
- **Priorités configurables** : Ordre d'exécution personnalisable

### ⚡ Gestion Professionnelle
- **Collection Editor intégré** : Configuration visuelle sans code
- **Gestion d'état** : Suivi des exécutions, réussites/échecs
- **Limitations** : Nombre max d'exécutions, cooldown entre événements
- **Déclenchement manuel** : Contrôle à la volée via API

## 💡 Cas d'Usage

- **Industrie** : Surveillance de processus, contrôle d'équipements
- **Métier** : Automatisation de rapports, sauvegardes planifiées
- **Domotique** : Gestion d'éclairage, contrôle climatique
- **Monitoring** : Vérifications périodiques, alertes conditionnelles

# Documentation SchreinSchedule

## Vue d'ensemble
SchreinSchedule est un composant .NET Windows Forms qui transforme n'importe quelle application en système automatisé professionnel. Il combine la puissance d'un planificateur de tâches avancé avec la flexibilité d'un moteur de règles conditionnelles.

## Architecture du Composant

### 🎮 Contrôle Visuel
- Interface utilisateur compacte (64x64 pixels)
- Indicateur visuel d'état (Actif/Inactif)
- Zones cliquables pour démarrage/arrêt et configuration
- Mise à jour automatique de l'heure

### ⚙️ Système de Tâches
Chaque tâche peut être configurée avec :
- **Déclencheurs** : Heure unique, dates multiples, récurrence
- **Arrêts** : Auto-stop, durée limite, nombre d'exécutions
- **Stratégie** : Récurrente, Calendrier, Fenêtre horaire, Mixte
- **Exclusions** : Dates spécifiques, jours fériés

### 🎯 Commandes Intelligentes
Les commandes s'exécutent selon :
- **Type de déclenchement** : Initial, Récurrent, Calendrier, Manuel, Arrêt
- **Conditions** : Expressions basées sur les valeurs des contrôles UI
- **Priorité** : Ordre d'exécution de 1 (élevé) à 10 (faible)
- **Limitations** : Nombre maximum d'exécutions

## Exemples de Configuration

### Surveillance de Température
```csharp
// Si température1 > 25°C ET ventilateur éteint → Activer ventilateur
Condition: "schreinTemperature1.Valeur > 25 && schreinVentilateur.Etat == false"
```

### Rapport Quotidien
```csharp
// 9h00 du lundi au vendredi, si base de données connectée
Condition: "labelDBStatus.Text == 'Connected'"
Déclencheur: Récurrent, jours ouvrables 9:00
```

### Sécurité
```csharp
// Alarme si pression > 100 OU température > 80
Condition: "capteurPression.Valeur > 100 || capteurTemperature.Valeur > 80"
```

### Sécurité
```csharp
// Alarme si pression > 100 OU température > 80
Condition: "capteurPression.Valeur > 100 || capteurTemperature.Valeur > 80"
```

### Sécurité
```csharp
// Alarme si pression > 100 OU température > 80
Condition: "capteurPression.Valeur > 100 || capteurTemperature.Valeur > 80"
```
## 🎯 Conditions Avancées

Le moteur de conditions supporte :

### 🔍 **Comparaisons**
`==`, `!=`, `>`, `<`, `>=`, `<=`

### 🧠 **Logique** 
`&&` (ET), `||` (OU)

### 📐 **Parenthèses**
Priorité des opérations

### 📊 **Types**
Nombres, strings, booléens

### 🔗 **Références**
`Control.Propriété`

### 💡 **Exemple**
```csharp
(temp1 > 30 && switch1 == true) || override.Actif
```

## Mots-clés recommandés
### Catégorie principale :
Timer, Scheduler, Automation, Planning

### Fonctionnalités :
Conditional, Trigger, Task, Command

### Technologie :
Windows Forms, .NET, Component

### Usage :
Control, Monitoring, Scheduling

### Secteurs :
Business Automation, Process Control

### 📝 Résumé pour Toolbox

```text
SchreinSchedule - Minuteur Automatisation
• Planification multi-tâches avancée
• Commandes conditionnelles intelligentes  
• Interface de configuration intégrée
• Déclencheurs multiples et stratégies flexibles
• Parfait pour l'automatisation métier
```
