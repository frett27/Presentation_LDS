<!-- page_number: true -->
# Travailler avec les geométries 

- Modèles :
	- Points
	- Ligne (multi)
	- Polygones (multi)

- Coordonnées X/Y/Z - M

- OGC - ST_Geometry

<p align="right"><image src="images/geometries.png" height="300"></image></p>

---
@@@ exemple définition geometries

WKT

GeoJSON

WKB

Shape

---
# Operateurs

- Tests booleen
	- intersection, touche, à l'intérieur, ont des frontières communes, ...  
- Modifications / Création
	- union / différence / intersection
<p align="center"><image src="images/union.jpg" height="100"></image></p>

- Rasterisation / Buffer / Delaunay / ... 

<p align="center"><image src="images/ex_rasterisation.png" height="150"></image>
<image src="images/buffer.jpg" height="150"></image></p>

---

# Bibliotheques Geometriques
	
- [OGR / GDAL (C++ / Wrappers)](http://gdal.org/)
- [ESRI-Geometry-API (JVM)](https://github.com/Esri/geometry-api-java)
- [JTS (JVM)](https://github.com/locationtech/jts)
- [GEOS (C++)](https://trac.osgeo.org/geos)
... 

---

@@@ Exemple manipulation geometries


---

# Problématiques associées à la cartographie

- Système de coordonnées (WGS 84/ WebMercator)
	- Bibliotheques de reprojection
- Computational Geometry / Précision des nombres
- Indexation / Volumes

---

# Indexation / Sharding

- Tuiles
- GeoHash
- QuadTree - RTree
- ...

---

@@@ Exemples - scala geohash

---

# En environnement BigData

- Points d'attention
	- Temps de parsing
	- Taille des éléments stockés

---

# Utilisation des données OSM

@@@ Exemples

---

# Framework

Vertica
Geomesa
ESRI-UDF 
...
@@@@

