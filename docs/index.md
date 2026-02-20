#  Fiche Technique Complète : IGN France (V2)

> **Référentiel :** Information géographique, forestière et aménagement du territoire.
> **Usage :** Documentation projet, intégration SIG, Big Data.

---

##  Identité de l'Organisme
* **Nom Officiel :** Institut national de l'information géographique et forestière (IGN).
* **Statut :** Établissement public (EPA) sous tutelle des ministères de l'Écologie et de l'Agriculture.
* **Missions :** Géodésie, Topographie, Photogrammétrie, Inventaire forestier national (IFN).

---

## Standards Techniques & Géodésie
Pour éviter les décalages de cartes, voici les normes utilisées par l'IGN :

* **Système de projection (Métropole) :** Lambert-93 (`EPSG:2154`).
* **Système de projection (Mondial/Web) :** WGS 84 / Pseudo-Mercator (`EPSG:3857`).
* **Système d'altitude :** NGF-IGN69 (Nivellement Général de la France).
* **Précision :** Métrique (BD TOPO) à centimétrique (Réseau Géodésique Permanent).

---

##  Ressources Open Data & API
La majorité des données sont sous **Licence Ouverte Etalab 2.0**.

### 1. Flux de données (Web Services)
Accessibles via QGIS, ArcGIS ou des bibliothèques JS (Leaflet/OpenLayers) :
* **WMTS :** Flux de tuiles pré-rendues (Cartes, Orthophotos).
* **WMS/WFS :** Flux de données vecteurs (Bâtiments, routes, parcelles).
* **TMS :** Pour les intégrations mobiles spécifiques.

### 2. Catalogues de Données Phares
| Nom | Format type | Description |
| :--- | :--- | :--- |
| **BD TOPO®** | GeoPackage / SQL | La base la plus complète (Bâti, réseaux, hydro). |
| **BD ORTHO®** | JPEG2000 / GeoTIFF | Photos aériennes haute résolution (20cm). |
| **Lidar HD** | .LAZ (Nuage points) | Scan laser du relief (10 pts/m² en moyenne). |
| **BD FORÊT®** | Vecteur | Occupation du sol forestier et essences d'arbres. |
| **RGE Alti®** | Pas de 1m à 5m | Modèle Numérique de Terrain (MNT) précis. |

---

##  Projets Innovants & Futur
* **Jumeau Numérique de la France :** Modélisation 3D intégrale du pays pour simuler les inondations ou l'étalement urbain.
* **IA & Occupation du Sol :** Utilisation du Deep Learning pour détecter automatiquement les changements (piscines non déclarées, nouvelles constructions) via les photos aériennes.
* **Géocommuns :** Démarche collaborative (inspirée d'OpenStreetMap) pour enrichir les bases de données publiques.

---

## Outils pour le Développeur
* **Géoportail API :** Accès programmatique aux services de recherche d'adresse et de calcul d'itinéraire.
* **Calcul d'altimétrie :** API REST pour récupérer l'altitude d'un point `(lat, lon)`.
* **Remonter le temps :** Comparaison historique (1950 vs Aujourd'hui) via API.

---

## Liens Utiles
* 📥 [Géoservices (Téléchargement)](https://geoservices.ign.fr/)
* 🌐 [Géoportail (Visualisation)](https://www.geoportail.gouv.fr/)
* 📖 [Documentation Technique (Wiki)](https://geoservices.ign.fr/documentation)

---
*Dernière mise à jour : 2024 - Documentation technique*