<!-- page_number: true -->

# OSM - Présentation du projet (Sylvain)

<image src="images/logo_osmfr.png"></image>
<a href="https://www.openstreetmap.fr">OpenStreetMap.fr</a>
La carte libre et participative

---
- Présentation
- État des données
- Contribution
- Utilisation des données
- Réutilisations / "sous-projets"
- Ressources

---

OpenStreetMap (OSM) est un projet international fondé en 2004 dans le but de créer une carte libre du monde.
Nous collectons des données dans le monde entier sur les routes, voies ferrées, les rivières, les forêts, les bâtiments et bien plus encore !
 

- Octobre 2011 : Création de l'association OpenStreetMap France.
- Septembre 2012 : passage sous licence libre OdbL.

---
# Principes de base

Pas une carte mais une base de données !
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
# Pourquoi contribuer/utiliser  ?

OSM  : «  Vous êtes libre de copier, distribuer, transmettre et adapter nos données, à condition que vous créditiez, OpenStreetMap et ses contributeurs.  »

IGN  : « Toute reproduction ou adaptation sous quelque forme que ce soit, même partielle, interdite pour tous pays.  »
Mais quand même des jeux de données en opendata !

Google  : « Sauf dans le cas où vous avez reçu une autorisation écrite préalable de Google, vous n'êtes pas autorisé à : a) copier  ; b) redistribuer  ; c) extraire ; d) effectuer des téléchargements en nombre ; e) supprimer/masquer un lien qui apparaît  ; f) utiliser avec un gps / navigation routière  ; g) créer une base de données de lieux  ;  »

---
# Pourquoi contribuer/utiliser  ?

Avantages
- Construction collaborative = somme de petites contributions locales
- De nombreux outils permettent de réutiliser facilement les données selon ses propres besoins : GPS, impression d'atlas, carte en ligne, géocodage, …
- Mise à jour en temps réel  : on enregistre, et c'est disponible pour tout le monde !
- Accès à TOUTES les données

---
# Pourquoi contribuer/utiliser  ?

Données de meilleure qualité  !
- Fourvière

<image src="images/mc_fourviere.png"></image>

---
# Pourquoi contribuer/utiliser  ?

Données de meilleure qualité  !
- Fourvière
- Beauduc

Parce que c'est utile !
- Humanitarian OpenStreetMap Team

---
<image src="images/hot_contributed.png"></image>

---
# Pourquoi contribuer/utiliser  ?

Données de meilleure qualité  !
- Fourvière
- Beauduc

Parce que c'est utile !
- Humanitarian OpenStreetMap Team
- Réseau régional des SAMU Normandie

---
# Quelles données  ?

Tout ce qui est une donnée géographique stable et vérifiable

Mais :
- Pas de données nominatives
- Pas de données temporaires
- Pas de données « personnelles »
- Pas de données copiées d'autres cartes non-libres  !

---
# État des données (à mettre à jour)

Plus de 2,6 milliards de nœuds
Plus de 20 millions de groupes de modifications

En France environ 200-250 contributeurs actifs chaque jours

Projet suffisamment mature pour commencer à produire de la donnée de type référentiel.
Exemple avec les contours de communes en précision cadastrale, commencée en 2008 et terminée en décembre 2013 => mise à disposition sur le portail data.gouv.fr (23 jeux de données à l'heure actuelle).

Dernier en date : contours des cantons électoraux 2015


---
# Processus

<image src="images/processus_contribution.png"></image>

1 – Collecter : traces gps, cartopartie, imagerie aérienne, open data, «  field papers  »
2 – Charger dans l'éditeur
3 – Modifier les objets
4 – Ajouter les détails  : attributs, relations
5 – Export des données / Rendu


---
# Structure des données

- Noeud (node)  : un point identifié par ses coordonnées lat/lon. Seul objet qui porte l'information géographique  !
- Chemin (way)  : un ensemble de nœuds reliés en polyligne.
- Surface (way fermé) : une polyligne fermée, avec le tag « area=yes ». Tracer le chemin dans le sens trigonométrique (intérieur de la surface à gauche de la polyligne).
- Relation  : un ensemble d'objets.

---
# Attributs

Les attributs peuvent être placés sur n'importe quel type d'objet, de préférence celui de plus haut niveau.

Exemples :
- POI  : sur un nœud simple ou un nœud d'un chemin/surface
- route : sur le chemin
- bâtiment  : sur le chemin fermé
- nom de commune : sur la relation des chemins du contour communal

Pas de structure fixe, autant d'attributs que nécessaire !

---
# Les éditeurs  : ID

Nouvel éditeur en ligne
- Éditeur simple
- Support des navigateurs modernes
- Rendu des données avec d3.js
- Open-source

<image src="images/editeur_id.png"></image>

---
# Les éditeurs  : JOSM

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
# Contrôles de qualité

Sur http://openstreetmap.org : des « notes » pour signaler les bugs

---
<image src="images/osm_note.png"></image>

---
# Contrôles de qualité

Sur http://openstreetmap.org : des « notes » pour signaler les bugs
Sur http://osmose.openstreetmap.fr : analyses automatiques des données

---
<image src="images/osmose.png"></image>

---
# Contrôles de qualité

Sur http://openstreetmap.org : des « notes » pour signaler les bugs
Sur http://osmose.openstreetmap.fr : analyses automatiques des données
Sur http://tile.openstreetmap.fr : comparaisons avec des référentiels ouverts
- base routes 500
- BD Carthage
- données carroyées de l'INSEE
- référentiel FANTOIR

---
<image src="images/zones_a_mapper.png"></image>

---
# Contrôles de qualité

Sur http://openstreetmap.org : des « notes » pour signaler les bugs
Sur http://osmose.openstreetmap.fr : analyses automatiques des données
Sur http://tile.openstreetmap.fr : comparaisons avec des référentiels ouverts
- base routes 500
- BD Carthage
- données carroyées de l'INSEE
- référentiel FANTOIR

Des outils de travail en parallèle : pour ne pas se marcher sur les pieds et garantir l'exhaustivité du travail
- MapCraft : découper en plusieurs secteurs
- Maproulette : liste de tâches, vérification d'1 objet à la fois
- Task Manager de HOT : contribution en situation de crise humanitaire

---
# Utiliser  les  données

- Bouton « Partager » : lien avec marqueur, export d'une image à l'échelle
- Onglet « Exporter » : zone réduite, fichier .osm
- download.openstreetmap.fr et download.geofabrik.de : exports pays/région
- Overpass-Api : langage de requêtes, sélection de données
- Umap : création de cartes personnalisées

---
# Echo système - TagInfo
=> à basculer sur la partie 2 ?

---
# Exemples d'utilisations (à développer)

- app smartphone : osmand, maps.me
- OpenSolarMap
- géocoder base SIRENE
- Cincinati cycle map

---
# Ressources  en  lignes

- http://switch2osm.org
- http://wiki.openstreetmap.org/wiki/FR:Develop
- http://wiki.openstreetmap.org/wiki/FR:Map_Features
- http://wiki.openstreetmap.org/wiki/FR:Cartotheque

---
# Communauté française

http://openstreetmap.fr

http://wiki.openstreetmap.org/wiki/Lyon
- Rencontre mensuelle
- Liste de discussion

