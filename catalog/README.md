# Catalogue des parcours de Golfmètre

Base de données des golfs de France utilisée par l'application Golfmètre, régénérée chaque semaine à partir d'OpenStreetMap, complétée par des éléments estimés d'après les données de l'IGN.

- `index.json` : date des données OSM, source, licence, et pour chaque golf son identifiant, son nom, son centre, ses trous, son état (complet, partiel, contour seul) et s'il contient des éléments estimés (`estimated`).
- `courses/<id>.json` : le parcours au format interne de l'application (trous, greens, départs, obstacles, décor).

## Éléments estimés

Quand OpenStreetMap n'a pas les départs, le green ou les bunkers d'un trou, voire aucun trou, Golfmètre les estime d'après le relief LiDAR HD et les photos aériennes BD ORTHO de l'IGN. Ces éléments portent `"estimated": true`. Une donnée d'OpenStreetMap n'est jamais remplacée : dès qu'un élément y est cartographié, c'est lui qui est repris. Les trous reconstruits n'ont pas de par.

## Licence

Base de données dérivée d'OpenStreetMap, publiée sous [Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/).

© les contributeurs d'OpenStreetMap. Données : https://www.openstreetmap.org/copyright

Éléments estimés d'après IGN LiDAR HD et BD ORTHO, sous [Licence Ouverte 2.0](https://www.etalab.gouv.fr/licence-ouverte-open-licence/) (Etalab), compatible avec l'ODbL. Source : IGN, Géoplateforme.
