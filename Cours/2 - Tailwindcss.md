# **Introduction :**

Comparons d’abord Tailwindcss et Bootstrap que vous connaissez déjà beaucoup plus. 

Tailwind CSS et Bootstrap sont deux frameworks CSS populaires pour la conception web, mais ils suivent des approches différentes. Bootstrap offre une série de composants prêts à l'emploi avec des classes prédéfinies, ce qui facilite la création rapide de sites web. Cependant, Tailwind CSS se distingue par sa flexibilité. Au lieu de fournir des composants préconstruits, il offre un ensemble de classes utilitaires que vous pouvez utiliser pour construire des designs personnalisés. Cela signifie que Tailwind CSS vous donne un contrôle total sur le style de votre site, sans avoir à surcharger ou à écraser des styles existants. De plus, Tailwind CSS est plus léger en termes de taille de fichier, ce qui se traduit par des temps de chargement plus rapides pour votre site. En fin de compte, si vous recherchez une approche plus flexible et légère pour la conception web et que vous préférez un contrôle granulaire sur le style, Tailwind CSS pourrait être le choix idéal.

Imagine que tu es un artiste et que Tailwind CSS est ta boîte de peinture. Avec cette boîte, tu peux créer des sites web super cool, tout comme un artiste crée de magnifiques tableaux. 

Tailwind CSS est une sorte de "boîte à outils" pour les développeurs web. Il te donne une tonne de petites classes CSS que tu peux utiliser pour construire ton site web. C'est comme avoir une boîte pleine de Legos de différentes formes et couleurs, et tu peux les assembler comme tu veux pour créer ce que tu veux.

Par exemple, si tu veux faire un bouton, tu peux utiliser des classes comme

```
bg-blue-500
```

pour le rendre bleu,

```
text-white
```

pour rendre le texte blanc, et

```
p-2
```

pour lui donner un peu de rembourrage. C'est comme si tu prenais un Lego bleu, un Lego blanc et un Lego un peu plus gros pour faire un bouton.

Et le meilleur dans tout ça ? Tu n'as pas besoin d'écrire une tonne de CSS toi-même. Tailwind s'en occupe pour toi. C'est comme si tu avais un assistant qui prépare toutes tes couleurs et formes pour toi, afin que tu puisses te concentrer sur la création de ton chef-d'œuvre.

Alors, prêt à commencer ton voyage avec Tailwind CSS ? Attrape ta souris et ton clavier, et prépare-toi à créer quelque chose d'incroyable !

## **Les Bases de Tailwind CSS**

Tailwind CSS est basé sur l'utilisation de classes CSS directement dans votre code HTML. Imaginez ces classes comme des blocs de construction que vous pouvez assembler pour créer votre site Web.

Voici quelques-unes des classes les plus courantes que vous pouvez utiliser :

### **Couleurs**

- **`bg-red-500`** : Change l'arrière-plan en rouge.
- **`text-blue-700`** : Change la couleur du texte en bleu.

( On définit l’intensité avec les nombres, par exemple *text-blue-200* sera bien moins foncé que *text-blue-700*)

### **Tailles**

- **`w-64`** : Définit une largeur de 16rem (taille fixe).
- **`h-32`** : Définit une hauteur de 8rem (taille fixe).
- **`w-[50px]`** : Définit une largeur de 50 pixels (taille personnalisée en pixels).
- **`h-[170px]`** : Définit une hauteur de 170 pixels (taille personnalisée en pixels).
- **`w-1/2`** : Définit une largeur de 50% (largeur proportionnelle).
- **`w-1/4`** : Définit une largeur de 25% (largeur proportionnelle).
- **`w-full`** : Définit une largeur de 100%.
- **`w-[50%]`** : Définit une largeur de 50% (taille personnalisée en pourcentage).
- **`w-[75vw]`** : Définit une largeur de 75% de la largeur de la fenêtre (viewport width).
- **`h-[50vh]]`** : Définit une hauteur de 50% de la hauteur de la fenêtre (viewport height).

### **Flexibilité**

- **`flex`** : Permet aux éléments de se comporter de manière flexible.
- **`justify-center`** : Centre le contenu horizontalement.

### **Marges et Espacements**

- **`m-4`** : Ajoute une marge de 1rem autour de l'élément.
- **`p-6`** : Ajoute un espace de 1,5rem à l'intérieur de l'élément.
- **`mt-4`** : Ajoute une marge top de 1rem autour de l'élément. On peut aussi ajouter t à p pour faire un padding top.
- **`mb-4`** : Pour une marge bottom.
- **`ms-4`** : Pour une marge à gauche (s pour start).
- **`me-4`** : Pour une marge à droite (e pour end).
- **`mx-4`** : Pour une marge à gauche ET à droite (x est l'axe des abscisses).
- **`my-4`** : Pour une marge en haut et en bas (y est l'axe des ordonnées).

### **Breakpoints de Tailwind CSS** (pour le responsive !)
- **`sm (small) : ≥ 640px`** : Utilisé pour les écrans de petite taille, comme les smartphones.

- **`md (medium) : ≥ 768px`** : Utilisé pour les écrans de taille moyenne, comme les tablettes.

- **`lg (large) : ≥ 1024px`** : Utilisé pour les écrans de grande taille, comme les ordinateurs portables.

- **`xl (extra-large) : ≥ 1280px`** : Utilisé pour les écrans très larges, comme les moniteurs de bureau.

- **`2xl (double extra-large) : ≥ 1536px`** : Utilisé pour les écrans ultra-larges.

#### **Utilisation des Breakpoints**
Vous pouvez utiliser ces breakpoints pour appliquer des styles spécifiques à chaque taille d'écran. Par exemple :

- **`sm:bg-red-500`** : Change le fond en rouge pour les écrans de petite taille et plus.
- **`md:bg-blue-500`** : Change le fond en bleu pour les écrans de taille moyenne et plus.
  
Ces breakpoints permettent de créer des designs responsives adaptés à différents dispositifs !

## **Exemples Pratiques**

### **Créons une Boîte Colorée**

```php
<div class="bg-green-300 w-48 h-48 flex justify-center items-center">
  <p class="text-white">Ma Boîte Colorée</p>
</div>
```

Dans cet exemple, nous avons créé une boîte verte de 48x48 pixels avec du texte blanc au centre. Magique, non ?

**Une Liste d'Amis**

```php
<ul>
  <li class="mb-2">Ami 1</li>
  <li class="mb-2">Ami 2</li>
  <li class="mb-2">Ami 3</li>
</ul>
```

Vous pouvez utiliser les classes pour espacer vos éléments et les rendre plus jolis.

## **Personnalisation**

Le meilleur dans Tailwind CSS, c'est que vous pouvez personnaliser vos couleurs, tailles et plus encore ! Vous pouvez créer vos propres classes CSS dans le fichier de configuration.

## **Conclusion**

Félicitations ! Vous avez appris les bases de Tailwind CSS. Il y a tellement plus à découvrir, alors n'hésitez pas à explorer davantage. Avec un peu de pratique, vous serez capable de créer des sites Web incroyables en un rien de temps.

Continuez à apprendre et à explorer le monde du design Web. Qui sait, vous pourriez être la prochaine superstar du développement Web !

Amusez-vous bien et à bientôt pour de nouvelles aventures dans le monde du codage ! 😃
