
<image src="images/osm_logo.png"></image>
[OpenStreetMap](https://www.openstreetmap.fr)
La carte libre et participative

---
<!-- page_number: true -->

- Présentation
- État des données
- Contribution
- Utilisation des données
- Réutilisations / "sous-projets"
- Ressources

---
# Historique

OpenStreetMap (OSM) est un projet international fondé en 2004 dans le but de créer une carte libre du monde.
Nous collectons des données dans le monde entier sur les routes, voies ferrées, les rivières, les forêts, les bâtiments et bien plus encore !
 
- Octobre 2011 : Création de l'association OpenStreetMap France.
- Septembre 2012 : passage sous licence libre OdbL.

---
# Principes de base

Pas une __carte__ mais une __base de données__ !
 => la donnée est constituée d'objets géographiques

Plus uniquement les rues …
- Bâtiments
- Points d'intérêts
- Pistes cyclables
- Pistes de ski
- Occupation des sols
- Adresses
- ...

---
# Pourquoi contribuer/utiliser ?

__OSM__ : « Vous êtes libre de copier, distribuer, transmettre et adapter nos données, à condition que vous créditiez, OpenStreetMap et ses contributeurs. »

__IGN__ : « Toute reproduction ou adaptation sous quelque forme que ce soit, même partielle, interdite pour tous pays. »
Mais quand même des jeux de données en opendata !

__Google__ : « Sauf dans le cas où vous avez reçu une autorisation écrite préalable de Google, vous n'êtes pas autorisé à : a) copier ; b) redistribuer ; c) extraire ; d) effectuer des téléchargements en nombre ; e) supprimer/masquer un lien qui apparaît ; f) utiliser avec un gps / navigation routière ; g) créer une base de données de lieux ; »

---
# Pourquoi contribuer/utiliser ?

Avantages
- Construction collaborative = somme de petites contributions locales
- De nombreux outils permettent de réutiliser facilement les données selon ses propres besoins : [GPS](http://garmin.openstreetmap.fr/garmin-lann/), [impression d'atlas](http://maposmatic.org), [carte en ligne](https://umap.openstreetmap.fr/fr/), [géocodage](https://adresse.data.gouv.fr/), …
- Mise à jour en temps réel : on enregistre, et c'est disponible pour tout le monde !
- Accès à TOUTES les données

---
# Pourquoi contribuer/utiliser ?

Données de meilleure qualité !
- [Fourvière](https://tools.geofabrik.de/mc/#16/45.7602/4.8208&num=3&mt0=mapnik&mt1=google-satellite&mt2=google-map)

---
# Pourquoi contribuer/utiliser ?

<image src="images/mc_fourviere.png"></image>

---
# Pourquoi contribuer/utiliser ?

Données de meilleure qualité !
- [Fourvière](https://tools.geofabrik.de/mc/#16/45.7602/4.8208&num=3&mt0=mapnik&mt1=google-satellite&mt2=google-map)
- [Beauduc](https://tools.geofabrik.de/mc/#15/43.3995/4.5943&num=3&mt0=mapnik&mt1=google-satellite&mt2=google-map)

Parce que c'est utile !
- [Humanitarian OpenStreetMap Team](https://www.hotosm.org)

---
# Pourquoi contribuer/utiliser ?

<image src="images/hot_contributed.png"></image>

---
# Pourquoi contribuer/utiliser ?

Données de meilleure qualité !
- [Fourvière](https://tools.geofabrik.de/mc/#16/45.7602/4.8208&num=3&mt0=mapnik&mt1=google-satellite&mt2=google-map)
- [Beauduc](https://tools.geofabrik.de/mc/#15/43.3995/4.5943&num=3&mt0=mapnik&mt1=google-satellite&mt2=google-map)

Parce que c'est utile !
- [Humanitarian OpenStreetMap Team](https://www.hotosm.org)
- [Réseau régional des SAMU Normandie](https://www.dailymotion.com/video/x1u2iq7)

---
# Quelles données ?

Tout ce qui est une donnée géographique stable et vérifiable

Mais :
- Pas de données nominatives
- Pas de données temporaires
- Pas de données « personnelles »
- Pas de données copiées d'autres cartes non-libres !

---
# État des données

- Plus de 4 milliards de nœuds
- Plus de 50 millions de groupes de modifications

En France environ 200-250 contributeurs actifs chaque jours

Projet suffisamment mature pour commencer à produire de la donnée de type référentiel!
Exemple avec les contours de communes en précision cadastrale, commencée en 2008 et terminée en décembre 2013 => mise à disposition sur le portail [data.gouv.fr](https://www.data.gouv.fr/fr/organizations/openstreetmap/) (24 jeux de données à l'heure actuelle).

Derniers en date : [bornes de recyclage Trilib'](https://www.data.gouv.fr/fr/datasets/bornes-trilib/), [Zones Touristiques Internationales à Paris](https://www.data.gouv.fr/fr/datasets/zones-touristiques-internationales-a-paris/)

---
# Processus

<image src="images/processus_contribution.png"></image>

1. Collecter : [traces gps](https://www.openstreetmap.org/traces), cartopartie, imagerie aérienne, open data, « [field papers](http://fieldpapers.org) »
2. Charger dans l'éditeur
3. Modifier les objets
4. Ajouter les détails : attributs, relations
5. Export des données / Rendu

---
# Structure des données

- **Noeud** (node) : un point identifié par ses coordonnées lat/lon. Seul objet qui porte l'information géographique !
- **Chemin** (way) : un ensemble de nœuds reliés en polyligne.
- Surface (way fermé) : une polyligne fermée, avec le tag « area=yes ». Tracer le chemin dans le sens trigonométrique (intérieur de la surface à gauche de la polyligne).
- **Relation** : un ensemble d'objets.

---
# Attributs

Les attributs peuvent être placés sur n'importe quel type d'objet, de préférence celui de plus haut niveau.

Exemples :
- POI : sur un nœud simple ou un nœud d'un chemin/surface
- route : sur le chemin
- bâtiment : sur le chemin fermé
- nom de commune : sur la relation des chemins du contour communal

Pas de structure fixe, __autant d'attributs que nécessaire__ !

---
# [TagInfo](https://taginfo.openstreetmap.org)

Visualiser les nombres d'occurences, valeurs, combinaisons de mots-clefs

<image src="images/taginfo.png"></image>

---
# Les éditeurs : ID

Nouvel éditeur en ligne
- Éditeur simple
- Support des navigateurs modernes
- Rendu des données avec d3.js
- Open-source

<image src="images/id_ini.png"></image>

---
# Les éditeurs : ID

<image src="images/id.png"></image>

---
# Les éditeurs : JOSM

L'outil le plus complet et le plus souple : http://josm.openstreetmap.de

Nombreuses extensions :
- adresses
- cadastre
- validation des données
- filtres
- télécommande
- imagerie
- ...

---
# Les éditeurs : JOSM

<image src="images/josm.png"></image>

---
# Contrôles de qualité

Sur [openstreetmap.org](https://www.openstreetmap.org/#map=15/45.7510/4.8600&layers=N) : des « notes » pour signaler les bugs

---
# Contrôles de qualité

<image src="images/osm_notes.png"></image>

---
# Contrôles de qualité

Sur [openstreetmap.org](https://www.openstreetmap.org/#map=15/45.7510/4.8600&layers=N) : des « notes » pour signaler les bugs
Sur [osmose.openstreetmap.fr](https://osmose.openstreetmap.fr/fr/map/#zoom=18&lat=45.75442&lon=4.860092&layer=Mapnik&overlays=FFFFFFFFFFFFFFFFFFFFT&item=xxxx&level=1%2C2%2C3&tags=&fixable=) : analyses automatiques des données

---
# Contrôles de qualité

<image src="images/osmose.png"></image>

---
# Contrôles de qualité

Sur [openstreetmap.org](https://www.openstreetmap.org/#map=15/45.7510/4.8600&layers=N) : des « notes » pour signaler les bugs
Sur [osmose.openstreetmap.fr](https://osmose.openstreetmap.fr/fr/map/#zoom=18&lat=45.75442&lon=4.860092&layer=Mapnik&overlays=FFFFFFFFFFFFFFFFFFFFT&item=xxxx&level=1%2C2%2C3&tags=&fixable=) : analyses automatiques des données
Sur [tile.openstreetmap.fr](http://tile.openstreetmap.fr/?zoom=12&lat=45.75424&lon=4.8404&layers=B000000FFFFTF) : comparaisons avec des référentiels ouverts
- base routes 500
- BD Carthage
- données carroyées de l'INSEE
- référentiel FANTOIR

---
# Contrôles de qualité

<image src="images/zones_a_mapper.png"></image>

---
# Contrôles de qualité

Sur [openstreetmap.org](https://www.openstreetmap.org/#map=15/45.7510/4.8600&layers=N) : des « notes » pour signaler les bugs
Sur [osmose.openstreetmap.fr](https://osmose.openstreetmap.fr/fr/map/#zoom=18&lat=45.75442&lon=4.860092&layer=Mapnik&overlays=FFFFFFFFFFFFFFFFFFFFT&item=xxxx&level=1%2C2%2C3&tags=&fixable=) : analyses automatiques des données
Sur [tile.openstreetmap.fr](http://tile.openstreetmap.fr/?zoom=12&lat=45.75424&lon=4.8404&layers=B000000FFFFTF) : comparaisons avec des référentiels ouverts

Des outils de travail en parallèle : pour ne pas se marcher sur les pieds et garantir l'exhaustivité du travail
- [MapCraft](https://mapcraft.nanodesu.ru) : découper en plusieurs secteurs
- [Maproulette](http://maproulette.org) : liste de tâches, vérification d'1 objet à la fois
- [Task Manager de HOT](http://tasks.hotosm.org) : contribution en situation de crise humanitaire

---
# Utiliser les données

- Bouton « Partager » : lien avec marqueur, export d'une image à l'échelle
- Onglet « [Exporter](https://www.openstreetmap.org/export#map=18/45.75449/4.85960) » : zone réduite, fichier .osm
- [download.openstreetmap.fr](http://download.openstreetmap.fr/extracts/) et [download.geofabrik.de](http://download.geofabrik.de) : exports pays/région
- [Overpass-Api](https://overpass-turbo.eu) : langage de requêtes, sélection de données

---
# Utiliser les données

<image src="images/overpass.png"></image>

---
# Utiliser les données

- Bouton « Partager » : lien avec marqueur, export d'une image à l'échelle
- Onglet « [Exporter](https://www.openstreetmap.org/export#map=18/45.75449/4.85960) » : zone réduite, fichier .osm
- [download.openstreetmap.fr](http://download.openstreetmap.fr/extracts/) et [download.geofabrik.de](http://download.geofabrik.de) : exports pays/région
- [Overpass-Api](https://overpass-turbo.eu) : langage de requêtes, sélection de données
- [Umap](https://umap.openstreetmap.fr) : création de cartes personnalisées

---
# Utiliser les données

<image src="images/umap_edition.png"></image>

---
# Utiliser les données

<image src="images/umap_primevere.png"></image>

---
# Utiliser les données

- Bouton « Partager » : lien avec marqueur, export d'une image à l'échelle
- Onglet « [Exporter](https://www.openstreetmap.org/export#map=18/45.75449/4.85960) » : zone réduite, fichier .osm
- [download.openstreetmap.fr](http://download.openstreetmap.fr/extracts/) et [download.geofabrik.de](http://download.geofabrik.de) : exports pays/région
- [Overpass-Api](https://overpass-turbo.eu) : langage de requêtes, sélection de données
- [Umap](https://umap.openstreetmap.fr) : création de cartes personnalisées
- [PostGIS](https://wiki.openstreetmap.org/wiki/PostGIS) : import de données complètes / mise à jour / traitements géographiques

---
# Exemples d'utilisations

- app smartphone : [osmand](https://osmand.net), [maps.me](https://maps.me)
- [OpenSolarMap](http://opensolarmap.org)

---
# Exemples d'utilisations

<image src="images/opensolarmap.png"></image>

---
# Exemples d'utilisations

- app smartphone : [osmand](https://osmand.net), [maps.me](https://maps.me)
- [OpenSolarMap](http://opensolarmap.org)
- [géocoder base SIRENE](https://github.com/cquest/geocodage-spd/tree/master/insee-sirene)
- [Cincinnati bike map](http://cincymap.org/about/)

---
# Exemples d'utilisations

<image src="images/Cincinnati_Bike_Map.png"></image>

---
# Ressources en lignes

- Basculer sur OSM : http://switch2osm.org
- Ressources pour les développeurs : http://wiki.openstreetmap.org/wiki/FR:Develop
- Principaux mots-clef/valeurs : http://wiki.openstreetmap.org/wiki/FR:Map_Features

---
# Ressources en lignes

<image src="images/map_feature.png"></image>

---
# Ressources en lignes

- Basculer sur OSM : http://switch2osm.org
- Ressources pour les développeurs : http://wiki.openstreetmap.org/wiki/FR:Develop
- Principaux mots-clef/valeurs : http://wiki.openstreetmap.org/wiki/FR:Map_Features
- Exemples de réalisations : http://wiki.openstreetmap.org/wiki/FR:Cartotheque

---
# Communauté

**Française**
http://openstreetmap.fr

**Lyonnaise**
http://wiki.openstreetmap.org/wiki/Lyon
- Rencontre mensuelle
- Liste de discussion

