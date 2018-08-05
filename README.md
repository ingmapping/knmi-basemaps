# KNMI Basemaps
An overview of tiled basemaps and tools developed for the KNMI geospatial infrastructure

This repository gives an overview of raster tiled basemaps and tools that were developed for the KNMI geospatial infrastructure during an internship project from March 2018 until August 2018. 

The purpose of the internship at the [KNMI](https://www.knmi.nl/over-het-knmi/about) was twofold: on the one hand, the development of tools to produce and reproduce tiled basemaps was central, while on the other hand, the goal was to create tiled basemaps for the KNMI geospatial infrastructure that meet the organization's use and user requirements. The internship project resulted into tiled basemaps for [KNMI GeoWeb](https://github.com/KNMI/GeoWeb-FrontEnd/)  that are: (1) reproducible by means of open-source solutions and tools, and (2) better suited for the overlay of geospatial (weather) data as a result of proper basemap styles and relevant custom cartographic projections. 

## Why this internship project?
As an operational organization, the KNMI needed to be independent of external basemap services. For this reason, KNMI wished to have their own basemaps and tools to produce and reproduce them. Furthermore, the former default OpenStreetMap remote basemap in KNMI GeoWeb contained a lot of overly detailed information. Because weather forecasters need to focus on weather model visualization, they should not be hindered by overly detailed background maps. The new basemaps respond to this problem.

## What was researched?
First, a literature research was performed on several cartographic topics (Web Mapping trends and standards & cartographic map design, generalization and projections) to understand what makes an effective basemap for use in KNMI GeoWeb. Afterwards, a use and user requirement analysis was conducted in order to understand the wishes and needs of (potential) KNMI GeoWeb users regarding basemaps.
By taking into account findings from the literature research as well as the use and user requirement analysis, it became clear that the KNMI needed basemaps that are (1) reproducible, (2) interactive (i.e. ability to zoom-in and out), and (3) well-designed in order to match with the main function of basemaps in KNMI GeoWeb which is to serve as a background for the overlay of geospatial data and weather visualizations.

## What are the results?
The deliverables give the [KNMI GeoWeb](https://github.com/KNMI/GeoWeb-FrontEnd/) developers a set of tools and solutions to generate tiled basemaps that give the KNMI, as an operational organization, independence of remote basemap services. Furthermore, the end-users of KNMI GeoWeb are provided with a set of pre-defined basemap styles and projections for which they can choose from for different purposes. There are basemaps with a lot of detail and basemaps that can be used for overview.

The developed tiled basemaps respond well to the advantages of interactive maps that enable to have additional 'hidden' information which can be accessed by the map user through interaction (e.g zooming). For this internship project, a “less-is-more approach” was applied for the cartographic design and generalization process while creating new basemaps for [KNMI GeoWeb](https://github.com/KNMI/GeoWeb-FrontEnd/). The ability to have different information on different zoom levels and to have more balanced, clear and legible basemap styles stimulates the effective use of [KNMI GeoWeb](https://github.com/KNMI/GeoWeb-FrontEnd/) and contributes to a better user experience of [KNMI GeoWeb](https://github.com/KNMI/GeoWeb-FrontEnd/).

## An overview of the new basemaps for KNMI GeoWeb
* KNMI GeoWeb WorldMap - *A simple basemap of the World for overview, data overlay and use with custom projections.* 
* KNMI GeoWeb WorldMap Light Grey Canvas - *A simple greyscale basemap of the World for overview and data overlay.*
* KNMI GeoWeb OpenStreetMap NL - *An extensive basemap for the extent of the Netherlands for when a lot of detail is needed when zooming in. Not recommended for data overlay. Recommended for users that are used to the standard OpenStreetMap style.*
* KNMI GeoWeb OSM Blossom NL - *A custom styled basemap for the extent of the Netherlands for when balanced detail is needed when zooming in. Recommended for users that need buildings in high zoom levels.*
* KNMI GeoWeb OpenStreets NL - *A custom styled basemap for the extent of the Netherlands for when balanced detail is needed when zooming in. Recommended for general purposes and for when Rijksdriehoekstel projection ([EPSG:28992](https://epsg.io/28992)) is needed.*
* KNMI GeoWeb OSM Antarctica - *A simple basemap of the Antarctica region in Polar projection ([EPSG:3412](https://epsg.io/3412)) for overview or data overlay.*
* KNMI GeoWeb Positron NL - A custom styled basemap for the extent of the Kingdom of the Netherlands for balanced overview, data overlay and some detail when zooming in.  Recommended for data overlay.*
* KNMI GeoWeb Positron NL No Labels - *A custom styled basemap without labels for the extent of the Kingdom of the Netherlands for balanced overview, data overlay and some detail when zooming in. Recommended for data overlay.*
* KNMI GeoWeb Klokantech Basic NL - *A custom styled basemap for the extent of the Kingdom of the Netherlands for balanced overview, data overlay and some detail when zooming in. Recommended for users that are used to the Google Maps style.*
* KNMI GeoWeb Klokantech Basic NL No Labels - *A custom styled basemap without labels for the extent of the Kingdom of the Netherlands for balanced overview, data overlay and some detail when zooming in. Recommended for users that are used to the Google Maps style.*

## An overview of the tools and GitHub repositories to reproduce the new KNMI GeoWeb basemaps
* KNMI GeoWeb WorldMap - [https://www.github.com/ingmaping/Basemaps_QTiles](https://www.github.com/ingmaping/Basemaps_QTiles).
* KNMI GeoWeb WorldMap Light Grey Canvas - [https://www.github.com/ingmapping/custom-projections-tilemill](https://www.github.com/ingmapping/custom-projections-tilemill).
* KNMI GeoWeb OpenStreetMap NL - [https://www.github.com/ingmapping/docker-mapnik-osm-tiles](https://www.github.com/ingmapping/docker-mapnik-osm-tiles).
* KNMI GeoWeb OSM Blossom NL - [https://www.github.com/ingmapping/docker-osm-blossom](https://www.github.com/ingmapping/docker-osm-blossom) or [https://www.github.com/ingmapping/osm-blossom-tilemill](https://www.github.com/ingmapping/osm-blossom-tilemill).
* KNMI GeoWeb OpenStreets NL - [https://www.github.com/ingmapping/openstreets-nl-tilemill](https://www.github.com/ingmapping/openstreets-nl-tilemill ) or [https://www.github.com/ingmapping/docker-openstreets-nl](https://www.github.com/ingmapping/docker-openstreets-nl) or [https://www.github.com/ingmapping/docker-openstreets-nl-rd](https://www.github.com/ingmapping/docker-openstreets-nl-rd) or [https://www.github.com/ingmapping/docker-mapnik-osm-tiles](https://www.github.com/ingmapping/docker-mapnik-osm-tiles).
* KNMI GeoWeb OSM Antarctica - [https://www.github.com/ingmapping/docker-mapnik-polar](https://www.github.com/ingmapping/docker-mapnik-polar ).
* KNMI GeoWeb Positron NL - [https://www.github.com/ingmapping/tile-generation](https://www.github.com/ingmapping/tile-generation).
* KNMI GeoWeb Positron NL No Labels - [https://www.github.com/ingmapping/tile-generation](https://www.github.com/ingmapping/tile-generation).
* KNMI GeoWeb Klokantech Basic NL - [https://www.github.com/ingmapping/tile-generation](https://www.github.com/ingmapping/tile-generation).
* KNMI GeoWeb Klokantech Basic NL No Labels - [https://www.github.com/ingmapping/tile-generation](https://www.github.com/ingmapping/tile-generation).
