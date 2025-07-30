# 🚀 Gestion Agile - Planning Projet

> **Le planning qui fait rêver les chefs de projet ✨**

Une application web moderne et intuitive pour la gestion de projets agiles, avec planning automatique, suivi des développeurs, et génération de comptes rendus.

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-production-ready-brightgreen)

## 🌟 Fonctionnalités

### 📊 **Planning Automatique Intelligent**
- **Répartition automatique** des projets sur les sprints
- **Gestion des priorités** avec logique de répartition 80/20
- **Calcul de capacité** basé sur les statuts des développeurs
- **Gestion des absences** et indisponibilités
- **Marge de sécurité** automatique (1 sprint par projet)

### 👥 **Gestion des Équipes**
- **Profils développeurs** : Débutant, Junior, Confirmé, Senior
- **Points par sprint** automatiques selon le niveau
- **Gestion des absences** par date (congés, maladie, formation)
- **Affectation flexible** des développeurs aux projets

### 📋 **Gestion des Projets**
- **Workflow complet** : Conception → Développement → Test → Review → Déploiement
- **Priorités** : 1 (critique) à 3 (normal)
- **Estimation en points** (Story Points)
- **Dates de début** et suivi temporel
- **Statut automatique** en "Déploiement" à la livraison

### 📈 **Comptes Rendu Automatiques**
- **Génération automatique** lors de la livraison d'un projet
- **4 sections obligatoires** :
  - 📝 **Résumé du projet**
  - ✅ **Ce qui a marché**
  - ⚠️ **Ce qui a moins bien marché**
  - 🎯 **Améliorations à apporter**
- **Export PDF** professionnel
- **Historique complet** des comptes rendus

### 🎨 **Interface Moderne**
- **Design responsive** adapté à tous les écrans
- **Animations fluides** et transitions élégantes
- **Thème cohérent** avec couleurs personnalisées
- **UX optimisée** pour une utilisation intuitive

## 🛠️ Technologies

- **Frontend** : HTML5, CSS3, JavaScript (ES6+)
- **Framework** : React 18 (CDN)
- **Styling** : Tailwind CSS
- **PDF** : jsPDF
- **Icons** : Heroicons
- **Fonts** : Google Fonts (Montserrat, Inter)

## 🚀 Installation

### Prérequis
- Navigateur web moderne (Chrome, Firefox, Safari, Edge)
- Connexion internet (pour les CDN)

### Installation rapide
1. **Clonez le repository**
   ```bash
   git clone https://github.com/votre-username/velocity-of-a-city.git
   cd velocity-of-a-city
   ```

2. **Ouvrez l'application**
   ```bash
   # Ouvrez simplement le fichier index.html dans votre navigateur
   # Ou utilisez un serveur local
   python -m http.server 8000
   # Puis allez sur http://localhost:8000
   ```

3. **C'est tout !** 🎉

## 📖 Guide d'utilisation

### 1. **Configuration des Sprints**
- Ajoutez vos sprints avec dates de début et fin
- L'application utilise ces informations pour le planning

### 2. **Gestion de l'Équipe**
- **Ajoutez vos développeurs** avec leur niveau
- **Configurez les absences** par date
- Les points par sprint sont calculés automatiquement

### 3. **Création de Projets**
- **Définissez les projets** avec priorité et estimation
- **Affectez des développeurs** (optionnel)
- **Définissez une date de début** (optionnel)

### 4. **Planning Automatique**
- Le planning se génère automatiquement
- **Filtres** par priorité, état, développeur
- **Indicateurs visuels** pour les retards

### 5. **Livraison et Comptes Rendu**
- **Marquez un projet comme fini**
- **Remplissez le compte rendu** obligatoire
- **Téléchargez le PDF** quand vous voulez

## 🎯 Fonctionnalités Avancées

### 🔄 **Logique de Répartition**
- **Priorité 1 vs 3** : Séquentiel (priorité 1 d'abord)
- **Même priorité** : Répartition équitable
- **Plusieurs priorités** : Priorité la plus haute d'abord

### 📊 **Calculs Intelligents**
- **Capacité réelle** = Points de base × (1 - jours d'absence / 10)
- **Marge de sécurité** : +1 sprint par projet
- **Gestion des week-ends** : +2 jours par sprint

### 🎨 **Personnalisation**
- **Couleurs** : Violet (#7C3AED), Bleu (#38BDF8), Or (#FFD700)
- **Fonts** : Montserrat (titres), Inter (texte)
- **Animations** : Fade-in et transitions fluides

## 📱 Responsive Design

L'application s'adapte parfaitement à tous les écrans :

- **📱 Mobile** : Interface optimisée pour les petits écrans
- **💻 Desktop** : Utilisation complète de l'espace disponible
- **🖥️ Tablette** : Disposition intermédiaire optimale

## 🔧 Configuration

### Variables personnalisables
```javascript
// Dans le code, vous pouvez modifier :
const SPRINT_DAYS = 10; // Durée d'un sprint en jours ouvrés
const POINTS_PAR_STATUT = {
  'Débutant': 30,
  'Junior': 45,
  'Confirmé': 60,
  'Senior': 75,
};
```

### Couleurs du thème
```css
--primary: #7C3AED;    /* Violet */
--accent: #38BDF8;     /* Bleu */
--gold: #FFD700;       /* Or */
--dark: #18181B;       /* Noir */
```

## 📊 Exports et Rapports

### 📄 **Génération PDF**
- **Comptes rendus automatiques** lors de la livraison
- **Format professionnel** avec mise en page structurée
- **Nom de fichier** : `compte-rendu-[projet]-[date].pdf`

### 💾 **Sauvegarde Locale**
- **localStorage** pour la persistance des données
- **Sauvegarde automatique** à chaque modification
- **Pas de serveur requis** - tout fonctionne en local

## 🤝 Contribution

Les contributions sont les bienvenues ! 

1. **Fork** le projet
2. **Créez** une branche pour votre fonctionnalité
3. **Commitez** vos changements
4. **Poussez** vers la branche
5. **Ouvrez** une Pull Request

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

## 🙏 Remerciements

- **Tailwind CSS** pour le framework de styling
- **React** pour la réactivité
- **jsPDF** pour la génération de PDF
- **Heroicons** pour les icônes
- **Google Fonts** pour les polices

## 📞 Support

Si vous avez des questions ou des suggestions :

- **Issues** : [GitHub Issues](https://github.com/votre-username/velocity-of-a-city/issues)
- **Email** : contact@velocity-of-a-city.com
- **Documentation** : [Wiki du projet](https://github.com/votre-username/velocity-of-a-city/wiki)

---

**Fait avec ❤️ et beaucoup de ☕ par l'équipe Velocity of a City**

*Le planning qui fait rêver les chefs de projet ✨* 