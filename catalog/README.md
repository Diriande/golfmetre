# Catalogue des parcours de Golfmètre

Base de données des golfs de France utilisée par l'application Golfmètre, régénérée chaque semaine à partir d'OpenStreetMap.

- `index.json` : date des données OSM, source, licence, et pour chaque golf son identifiant, son nom, son centre, ses trous et son état (complet, partiel, contour seul).
- `courses/<id>.json` : le parcours au format interne de l'application (trous, greens, départs, obstacles, décor).

## Licence

Base de données dérivée d'OpenStreetMap, publiée sous [Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/).

© les contributeurs d'OpenStreetMap. Données : https://www.openstreetmap.org/copyright

Pour corriger un parcours (trous, pars, greens), le mieux est de l'éditer directement dans OpenStreetMap : la correction arrivera dans ce catalogue à la génération suivante.
