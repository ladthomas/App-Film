# APP FILM

Cette application permet aux utilisateurs de rechercher des séries télévisées en utilisant l'API de TVMaze et d'afficher les résultats sous forme de cartes interactives.

## Fonctionnalités

- **Recherche de séries** : Tapez le nom d'une série pour rechercher des résultats à partir de l'API TVMaze.
- **Affichage des résultats** : Les résultats s'affichent sous forme de cartes contenant le titre de la série, une image, et un résumé.
- **Cartes cliquables** : Chaque carte de série est entièrement cliquable, permettant une interaction fluide.

## Structure du projet

Le projet est constitué de trois fichiers principaux :

1. **index.html** : Fichier HTML principal qui définit la structure de base de l'application. Il contient un champ de recherche et une section pour les résultats.
2. **styles.css** : Fichier de style CSS pour la mise en page et le design de l'application.
3. **app.js** : Fichier JavaScript qui gère la logique de recherche via l'API TVMaze et l'affichage dynamique des résultats.

## Fichiers

### index.html

Ce fichier contient le squelette de l'application avec un champ de recherche et une section pour afficher les résultats. Il est lié au fichier CSS pour le style et au fichier JavaScript pour la logique de l'application.

Extrait du fichier `index.html` :
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>APP FILM</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div id="app">
        <header>
            <h1>Rechercher une Série</h1>
        </header>

        <main>
            <div class="search-box">
                <input type="text" id="searchInput" placeholder="Tapez le nom d'une série..." />
                <button id="searchButton">Rechercher</button>
            </div>
            <div id="results">
                <!-- Les résultats apparaîtront ici -->
            </div>
        </main>
    </div>

    <script src="app.js"></script>
</body>
</html>
