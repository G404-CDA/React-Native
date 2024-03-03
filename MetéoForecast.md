# MétéoForecast

### TP Réalisable en React et/ou ReactNative

## 🗼 API :

[OpenWeather - Weather forecasts, nowcasts and history in a fast and elegant way](https://openweathermap.org/)

- Créer un compte pour obtenir votre clé API

## 🌶️ Première étape : Création du projet

Créer un nouveau projet React ou React Native, installer l'ensemble des librairies nécessaires :

- Redux
- React Redux
- Redux Thunk
- Redux Dev Tools

et enfin créer l'arborescence du projet 

- components/
- actions/
- reducers/
- store.js

## 🌶️ Intégration

Vous allez devoir intégrer la maquette suivante [weather-app](https://xd.adobe.com/view/170a9627-134b-4fea-b115-d605c3d7e507-4259/), en respectant les problématiques de séparation des responsabilités

*il manque un petit bouton de validation de la ville pour lancer la recherche, ajoutez le*

#### On peut donc identifier les composants suivants :

- App
- Forecast
- ForecastTitle
- ForecastChoseCity
- ForecastResult
- ForecastForm

## 🌶️ Redux

Vous allez maintenant créer les fichiers de votre pattern Flux 😀

- reducers/forecast.js
    ```js
    let initialState = {
        forecast: {},
        loader: false
    };
    export const forecast = (state = initialState, action) => {
    /*TODO*/
    };
    ```

- actions/forecast.js
    ```js
    /*TODO*/
    export const updateForecast = (forecast) => {
    /*TODO*/
    };

    export const toggleLoader = (status) => {
    /*TODO*/
    };
    export const fetchForecast = city => {
        return async dispatch => {
            /*TODO*/
        }
    };
    ```

 - store.js (à faire vous même avec la fonction createStore et applyMidleware de redux)