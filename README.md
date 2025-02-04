# Isitech2425_NextJS


## NextJs

### Style Globaux

situé dans ```/app/ui/global.css```

il est appliqué à toute les route

il faut l'importer dans le ```/app/layout.tsx```

dans se fichier on vas avoir par exemple la palette de couleur pour notre site

### Intégration de Tailwind

objectif de Tailwind: gain de temps pas de performance.

plus lisible (il faut le pratiquer pour mieux le comprendre)

le + de Tailwind, les fichier CSS sont optimisé

### Bibliothèque clsx

permet de faire de l'affichage conditionné

### Optimisation des Polices 

impact sur les performance

Problème du CLS "Cumulative Layout Shift"

éviter le changment de mise en page lors du chargement
#### Dans NextJs

Les polices sont téléchargé au build et optimise automatiquement avec ```Next/font```

### Optimisation des Images 

Optimisation des performances
taille ajustable facilement
alt obligatoire

```className="hidden md:block"``` 

syntaxe pour savoir si l'image apparait suivant la taille de l'écran

### Routage

Fonctionne avec les fichiers et le ```page.tsx```

```layout.tsx``` Interace partagée entre plusieurs pages, contient les balises ```<html>``` et ```<body>```

### Navigation

normalement on utilise la balise ```<a>``` mais elle recharge complètement la page se qui impact fortement les performances et l'expérience utilisateur. On vas donc utiliser le composant ```<Link>``` 

partie préchargement, quand il le peut next vas précharger les éléments se qui améliore l'expérience utilisateur.

### base de données

remplir le fichier ```.env``` et bien le mettre dans le ```.gitignore```

On peut intéragir depuis un composant avec la bdd

### Streaming

technique de transfert de données par "Chunks", il vas séparer les parties static et dynamique

### Les composants

Rootlayout vien de typeScript

Les props : sont des paramètres qui vont permettre de transmettre des informations entre composants

la props children est