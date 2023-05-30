# Guide de démarrage pour le projet Workshop Dating App React / Firebase
## Description et fonctionnalités

Le projet consiste à créer une application similaire à Tinder ou Fruitz en utilisant React pour la partie front-end et Firebase pour la partie back-end. L'application comprendra des fonctionnalités telles qu'une page de connexion, un menu de swipe et des conversations.
Prérequis

Avant de commencer, assurez-vous d'avoir npm (Node Package Manager) et Node.js installés sur votre machine. Si ce n'est pas le cas, suivez les étapes ci-dessous pour les installer :
#### Installation de Node.js
Ouvrer un terminal, exécutez les commandes suivantes :
```
sudo apt-get update
sudo apt-get install nodejs
```

Vérifiez que Node.js est installé en exécutant la commande suivante :
```
node -v
```

#### Installation de npm :

Ouvrer un terminal, exécutez les commandes suivantes :
```
sudo apt-get update
sudo apt-get install npm
```

Vérifiez que npm est installé en exécutant la commande suivante :
```
npm -v
```
## Configuration du projet

Créez un nouveau répertoire pour votre projet :

```
mkdir DatingApp
cd DatingApp
```

Initialisez un nouveau projet React en exécutant la commande suivante :
```
npx create-react-app dating-app
cd dating-app
```

Si vous souhaitez utiliser Tailwind CSS pour le style de votre application, installez-le en exécutant les commandes suivantes :
```
npm install tailwindcss@latest postcss@latest autoprefixer@latest
npx tailwindcss init
```
    
Vous aurez également besoin de Firebase pour la partie back-end du projet. Installez-le en exécutant la commande suivante :
```
npm install firebase
```

Maintenant que votre environnement de développement est configuré, vous pouvez passer à l'étape suivante.

### Création de la page de connexion

Dans le répertoire src, créez un dossier nommé components.
À l'intérieur du dossier components, créez un fichier nommé LoginPage.js.
Dans le fichier LoginPage.js, vous pouvez commencer à implémenter votre page de connexion en React.
Voici un exemple de code pour démarrer :
```
import React from 'react';

const LoginPage = () => {
  return (
    <div>
      <h1>Login Page</h1>
      {/* Ajoutez votre formulaire de connexion ici */}
    </div>
  );
};

export default LoginPage;
```

Dans le fichier App.js, importez le composant LoginPage en ajoutant la ligne suivante :

```
import LoginPage from './components/LoginPage';
```

Remplacez le contenu du composant App par le code suivant :

```
function App() {
  return (
    <Router>
      <Routes>
        <Route path="/" element={<LoginPage />} />
      </Routes>
    </Router>
  );
}
```

Maintenant, vous pouvez lancer votre application en exécutant la commande suivante :
```
npm start
```

Vous devriez voir la page de connexion s'afficher dans votre navigateur.

### Connexion à Firebase 

Rendez-vous sur la page Firebase (https://firebase.google.com/) et créez un compte si vous n'en avez pas déjà un.
Une fois connecté, créez un nouveau projet et donnez-lui un nom, par exemple "DatingApp".
Sur la page principale du projet Firebase, cliquez sur "Authentication" dans le menu de gauche.
Dans l'onglet "Sign-in Method", activez l'option "Email/Password".

À ce stade, vous avez configuré les bases du projet et vous pouvez continuer à développer les fonctionnalités nécessaires pour l'appli :) 
