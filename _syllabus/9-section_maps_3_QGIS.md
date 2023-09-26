---
class: 9
day: Tuesday, October 26
title: QGIS
tags: 
---

## Assignment due: 
- Create a map by using the csv code we wrote in last class. Import it on QGIS, export a .jpg, and upload it on GitHub


## Before Class 
- Download and install [QGIS Standalone Installer](https://qgis.org/en/site/forusers/download.html) (Long term release (most stable)) 

## Reading 
- Foote, K. E., Lynch, M. (1995) “Geographic Information Systems as an Integrating Technology: Context, Concepts, and Definitions, in The Geographer’s Craft <http://gisweb.massey.ac.nz/topic/webreferencesites/whatisgis/texaswhatisgis/texas/intro.htm>
- Tsiafakis, D., Evangelidis, V. (2006) “GIS as an Interpretative Tool in Greek Archaeological Research,” in G. Priestnall - P. Aplin (eds.) Proceedings of the GIS Research UK. 14th Annual Conference. GISRUK 2006. 5-7 April 2006, Nottingam: 328-333.

## Extra readings
- Watch [this video](https://www.youtube.com/watch?v=hVuPAAAAoso&ab_channel=SarahE.Bond) on Pleiades and Antiquity À-la-carte by Tom Elliott and Sarah Bond (the video is a bit old so some features may have slightly changed).
- Use OpenRefine and Geocollider: [OpenRefine](https://openrefine.org/) is a tool that helps you work with tabular data and  [Geocollider](https://pleiades.stoa.org/news/blog/introducing-geocollider) is a tool that helps you collate a list of places locations against the Pleiades gazetteer. See Tom Elliott, “[An example workflow for geography in an ancient studies project: the Vicarello cups](https://www.youtube.com/watch?v=KMZZSVhQwXo&ab_channel=TomElliott),” who goes through step by step how you can form a text as a comma-separated values (CSV) file and how to use OpenRefine and Geocollider (after 17:08). Check also his blog post “[Using OpenRefine With Pleiades](http://horothesia.blogspot.com/2017/10/using-openrefine-with-pleiades.html),” in Horothesia, October 13, 2017.

## Notes 

#### Helpfull websites
- [EarthExplorer](https://earthexplorer.usgs.gov/). It requires registration. [Watch Obtaining + Loading Landsat Imagery in QGIS 3.10](https://www.youtube.com/watch?v=mBk2VIMawRE&ab_channel=MiddleburyRemoteSensing) for a step-by-step guide on how to use the data from EarthExplorer.
- [Mapping the Ancient Mediterranean with QGIS: A Quick Guide](https://sites.temple.edu/tudsc/2017/01/31/mapping-the-ancient-mediterranean-with-qgis-a-quick-gude/). From where you can download data on mapping data for the ancient world:
  - [Coastline](http://awmc.unc.edu/awmc/map_data/shapefiles/physical_data/coastline/)
  - [River](http://awmc.unc.edu/awmc/map_data/shapefiles/physical_data/ba_merge/)
  - [Inland water](http://awmc.unc.edu/awmc/map_data/shapefiles/physical_data/inlandwater/)
  - [Open water](http://awmc.unc.edu/awmc/map_data/shapefiles/physical_data/openwater/)
  - [Roman Road](http://awmc.unc.edu/awmc/map_data/shapefiles/ba_roads/)
- [ArcGIS REST Services Directory](https://server.arcgisonline.com/arcgis/rest/services). You can check the different MapServers. In order to download them
  - navigate to one MapServer and copy the link. E.g., https://server.arcgisonline.com/arcgis/rest/services/NatGeo_World_Map/MapServer
  - Go to QGIS. Right click on XYZ Tiles and Add Connection.
  - In Name, put a representative name.
  - In URL, paste the link you copied and add `/tile/{z}/{y}/{x}`.
  - Press OK. Then you will able to drap  and drop it in Layers.
  - [OpenDem](https://www.opendem.info/opendem_client.html). You can download contour datasets in shape format.
- [Ancient World Mapping Center](http://awmc.unc.edu/wordpress/), that provides different resources for diggital mapping of the ancient world. You may want to check the Spapefiles in [Resources](http://awmc.unc.edu/wordpress/map-files/).