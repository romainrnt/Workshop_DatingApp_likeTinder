# Workshop Dating App React / Firebase

## Description et Fonctionnalitées

Le projet consiste à créer une application comme Tinder, Fruitz de A à Z  (page de login, menu de swipe, conversations). Appli en React pour le front et Firebase pour le back.

## Pré-requis

Avant tout, vérifier que vous avez bien npm et node.js d'installé.

Si ce n'est pas le cas installez le comme suit,
Node.js :
```
sudo apt-get update
sudo apt-get install nodejs
node -v
```

npm :
```
sudo apt-get update
sudo apt-get install npm
npm -v
```

Setup le projet :
```
mkdir DatingApp
cd DatingApp
```

```
npx create-react-app dating-app
cd dating-app
```

Si vous souhaitez utiliser du style pour votre application je vous conseille d'utiliser Tailwind CSS.
```
npm install tailwindcss@latest postcss@latest autoprefixer@latest
npx tailwindcss init
```
Vous aurez également besoin de firebase pour la partie back du projet :
```
npm install firebase
```

Une fois que tout est bien installé, vous pouvez lancer votre IDE.

## Dev
Creez un dossier "components" et un fichier "LoginPage.js" dans src

Appeler le dans App.js en faisant
```
import LoginPage from './components/LoginPage';
```

Ajouter l'élement de la LoginPage
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

Vous pouvez mainteant implémenter votre page de login dans src/components/LoginPage.js
Pour lancer le projet :

```
npm start
```

Une fois que la page de login est faite.
Vous allez devoir la connecter à Firebase.

Rendez vous sur la page de firebase.
Créez votre compte et ajouter un nouveau projet :
Nommez votre projet DatingApp :

Rendez-vous sur la page principal ou vous aurez plusieurs informations.
Cliquez sur authentification et valider les options Adresse Mail / Mot de passe dans Sign-in Method.