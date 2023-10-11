# Tailwindcss

# Installation :

## **Étape 1 : Création d'un Projet**

Commencez par créer un projet web si vous n'en avez pas déjà un. Vous pouvez utiliser votre éditeur de texte préféré (comme Visual Studio Code) ou un générateur de projet comme Create React App, Vue CLI, ou simplement un dossier vide pour du HTML/CSS pur.

## **Étape 2 : Installation de Node.js et npm (si nécessaire)**

Si vous n'avez pas encore Node.js et npm installés sur votre ordinateur, vous devez les installer. Vous pouvez les télécharger à partir du site officiel de Node.js : **[https://nodejs.org/](https://nodejs.org/)**

Pour vérifier si Node.js et npm sont installés, ouvrez votre terminal et exécutez les commandes suivantes :

```bash
node -v
npm -v
```

Si ces commandes retournent des versions, c'est que Node.js et npm sont déjà installés.

## **Étape 3 : Initialisation du Projet**

Accédez au répertoire de votre projet dans le terminal. Vous pouvez utiliser la commande **`cd`** pour vous déplacer dans le répertoire de votre projet :

```bash
cd chemin/vers/votre/projet
```
Ou ouvrez votre projet sur VS Code et utilisez le terminal inclus.

Ensuite, initialisez votre projet en exécutant la commande suivante :

```bash
npm init -y
```

Cela créera un fichier **`package.json`** qui contiendra les informations sur votre projet.

## **Étape 4 : Installation de Tailwind CSS**

Maintenant, vous pouvez installer Tailwind CSS en utilisant npm. Exécutez la commande suivante dans votre terminal :

```bash
npm install tailwindcss
```

## **Étape 5 : Création d'un Fichier de Configuration Tailwind**

Générez un fichier de configuration Tailwind CSS en exécutant la commande suivante :

```bash
npx tailwindcss init
```

Cela créera un fichier **`tailwind.config.js`** à la racine de votre projet, que vous pourrez personnaliser pour ajuster les paramètres de Tailwind CSS selon vos besoins. Ajouter votre futur fichier "./index.html" à la section content pour test.

## **Étape 6 : Création d'un Fichier CSS**

Créez un fichier CSS où vous importerez les styles de Tailwind CSS. Par exemple, vous pouvez créer un fichier **`style.css`**.

Dans ce fichier, ajoutez l'instruction d'importation pour les styles Tailwind CSS :

```css
@import 'tailwindcss/base';
@import 'tailwindcss/components';
@import 'tailwindcss/utilities';
```

## **Étape 7 : Compilation des Styles**

Pour que Tailwind CSS soit pris en compte dans votre projet, vous devez compiler vos fichiers CSS. Vous pouvez utiliser des outils tels que Webpack, Parcel, ou simplement la ligne de commande pour cela.

Supposons que vous utilisez la ligne de commande. Créez une commande npm dans votre fichier **`package.json`** pour exécuter la compilation. Par exemple :

```json
"scripts": {
  "build:css": "tailwindcss build -i style.css -o output.css"
}
```

Exécutez ensuite la commande suivante pour compiler vos styles : 

```bash
npm run build:css
```

En cas de soucis de type 'Cannot find module xxx', vous pouvez réinstaller les dépendances :

```bash
rm -rf node_modules
npm install
```

## **Étape 8 : Intégration dans votre HTML**

Dans votre fichier HTML, liez le fichier CSS que vous avez compilé à votre projet :

```html
<link rel="stylesheet" href="output.css">
```

Vous pouvez maintenant utiliser les classes Tailwind CSS dans votre HTML pour styliser vos éléments.

Voilà, vous avez maintenant installé Tailwind CSS dans votre projet ! Vous pouvez commencer à créer des interfaces utilisateur magnifiques en utilisant les classes fournies par Tailwind CSS. Assurez-vous de consulter la documentation officielle de Tailwind CSS (**[https://tailwindcss.com/docs](https://tailwindcss.com/docs)**) pour en savoir plus sur les classes disponibles et comment les utiliser efficacement.

TIPS :

Vous venons de voir l’installation la plus performante et efficiente de Tailwindcss pour vos projets, cependant vous pouvez très bien installer tailwindcss plus simplement en utilisant le CDN :

```html
<script src="https://cdn.tailwindcss.com"></script>
```

TIPS 2 : 

Installez l’extension ***Tailwindcss Intellisense***, elle vous accompagnera dans votre apprentissage de tailwind et vous aidera à être plus rapide et efficace :)
