## Starter Project

- css fourni (styles globaux, composants stylisés)
- dossiers/fichiers déjà configurés
- toutes les importations sont incluses (avertissements)
- index.js pour faciliter les importations

## Styled Components

[Styled-Components - Main Docs](https://styled-components.com/)

```jsx
import styled from "styled-components";

const ReactComponent = () => {
 // logique ici
 return <Wrapper>
 {some content}
 </Wrapper>
}


const Wrapper = styled.htmlElement`
écrivez vos styles ici
`
export default ReactComponent
```

## React Icons

[React Icons - Main Docs](https://react-icons.github.io/react-icons/)

```jsx
import { FiUsers, FiUserPlus } from "react-icons/fi";
<FiUsers className='nameOfTheClass'> </FiUsers>;
```

## React Router Dom

version utilisée - "react-router-dom": "^5.2.0",

- [react-router-dom - Main Docs](https://reactrouter.com/web/guides/quick-start)

- <Switch> rend le premier <Route> enfant qui correspond.
- Une <Route path="*"> correspond toujours.

## Gihthub API

- [Root Endpoint](https://api.github.com)
- [Get User](https://api.github.com/users/glebngouma)
- [Repos](https://api.github.com/users/glebngouma/repos?per_page=100)
- [Followers](https://api.github.com/users/glebngouma/followers)
- [Rate Limit](https://api.github.com/rate_limit)

Pour les demandes non authentifiées, la limite de débit est de 60 demandes par heure. Les demandes non authentifiées sont associées à l'adresse IP d'origine et non à l'utilisateur qui fait la demande.

## Fusion Charts

- [Fusion Charts - Main Docs](https://www.fusioncharts.com/)
- [First React Chart](https://www.fusioncharts.com/dev/getting-started/react/your-first-chart-using-react)
- [List Of Charts](https://www.fusioncharts.com/dev/chart-guide/list-of-charts)
- [Themes](https://www.fusioncharts.com/dev/themes/introduction-to-themes)

## Auth0

- [Auth0 - Main Docs](https://auth0.com/)

- Créer une application
- Choisir : Applications Web à page unique
- Choisir : React
- Aller à l'onglet Paramètres
- Copier/coller Domaine, ID client - peut être public (ou utiliser .env)
- Ajouter un domaine -
  pour l'instant http://localhost:3000 (NE PAS COPIER COLLER DE LA BARRE D'URL)

  - URL de rappel autorisés
  - URL de déconnexion autorisés
  - Origines Web autorisées
  - ENREGISTRER LES MODIFICATIONS !!!!!!!!!!!!!!!

- Connexions
  email,social

- [React SDK Docs](https://auth0.com/docs/libraries/auth0-react)
- [REACT SDK API Docs](https://auth0.github.io/auth0-react/)

## Deployment

[Netlify](https://www.netlify.com/)

## Additional Info

#### Redirects with react-router-dom

Pour que le routage fonctionne sur netlify, les redirections ont été ajoutées au dossier public

- \_redirige le fichier dans le public

```

/*    /index.html   200

```

[Redirects Blog Post](https://dev.to/dance2die/page-not-found-on-netlify-with-react-router-58mc)

#### Warnings and create-react-app

package.json

```js
"build": "CI= react-scripts build",
```

[create-react-app Warning Fix Blog Post](https://community.netlify.com/t/how-to-fix-build-failures-with-create-react-app-in-production/17752)
