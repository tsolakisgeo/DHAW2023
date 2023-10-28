---
class: 9
day: Tuesday, October 26
title: QGIS (1/2)
tags: 
---

## Assignments due:

### Response Paper
- Based on your readings, please provide a short (max. 200 words) response on what GIS is and how it informs the archaeological research.

Upload your response paper on GitHub in the directory <username>/CLCV22123/9 and paste a link to the file on Canvas.
  
### Critique of two digital tool
- [The Homer Multitext project](https://www.homermultitext.org/)
- [The Digital Dead Sea Scrolls](http://dss.collections.imj.org.il/)

Upload your critiquie on GitHub in the directory <username>/CLCV22123/9 and paste a link to the file on Canvas.

### Weekly assignment
### 1. Python and JSON
Write a function `def export_coordinates(input_list, filename)` that takes a list of PleiadesIDs as an input and creates an csv file with four columns (named `'title', 'pleiadesID', 'longitude', 'latitude'`). The function should:
- test if a particular path (e.g., `['features'][0]['geometry']['coordinates']`) exists in the JSON file. If such a path does not exist, the function should handle the error/exception. Hint: do not use `if statements`.
- make requests to the Pleiades and return the respective fields for the mentioned columns
- export the results to a csv file, whose name will be passed as an argument.

Finally:
- Upload the Jupyter Notebook and the csv file on Github `(<username>/CLCV22123/9/)`.
- Post a link to the folder on Canvas.

### 2. Peripleo
Use the csv file you submitted for Exercise 4. 

- Rename the titles of your headers to "title", "longitude", "latitude", and "url". 
- Add another column named "depictions" and populate that column with links to images you have found online for each respective place.
- Upload the csv file to [Locolligo](https://docuracy.github.io/Locolligo/).
- Download your input as a JSON file.
- Open the JSON file in a text editor. Search for jpg and change the respective field as seen below

__Original__:

```      
 "depictions": [

    {

      "@id": "https://s3.geograph.org.uk/geophotos/06/22/64/6226459_9ac04c4d.jpg"

    }

  ]
```

__Final__:

```      
 "depictions": [

    {

      "@id": "https://s3.geograph.org.uk/geophotos/06/22/64/6226459_9ac04c4d.jpg",

      "title": "The Acropolis Museum as seen from the top of the Acropolis of Athens",

      "thumbnail": "https://s3.geograph.org.uk/geophotos/04/63/93/4639399_bde13bd4_120x120.jpg"

    }

  ]
```

- Upload your file to your Peripleo repository. 
- Make the necessary changes so that your new JSON file will be the source of Peripleo.
- Post a link to your Peripleo map (e.g., https://britishlibrary.github.io/peripleo) on Canvas.
- If you have successfully followed the previous steps, your map will show your places. If you chick on each place an image should appear.

## Before Class 
- Download and install [QGIS Standalone Installer](https://qgis.org/en/site/forusers/download.html) (Long term release (most stable)) 

## Readings 
- Foote, K. E., Lynch, M. (1995) “Geographic Information Systems as an Integrating Technology: Context, Concepts, and Definitions, in The Geographer’s Craft <http://gisweb.massey.ac.nz/topic/webreferencesites/whatisgis/texaswhatisgis/texas/intro.htm>
- Graml, C., Hunziker, M., Vukadin, K. (2019) “Cult and Crisis: A GIS Approach to the Sacred Landscape of Hellenistic Attica,” _Open Archaeology_, 5; 1, p. 383-395.

## Extra readings
- Watch [this video](https://www.youtube.com/watch?v=hVuPAAAAoso&ab_channel=SarahE.Bond) on Pleiades and Antiquity À-la-carte by Tom Elliott and Sarah Bond (the video is a bit old so some features may have slightly changed).
- Use OpenRefine and Geocollider: [OpenRefine](https://openrefine.org/) is a tool that helps you work with tabular data and  [Geocollider](https://pleiades.stoa.org/news/blog/introducing-geocollider) is a tool that helps you collate a list of places locations against the Pleiades gazetteer. See Tom Elliott, “[An example workflow for geography in an ancient studies project: the Vicarello cups](https://www.youtube.com/watch?v=KMZZSVhQwXo&ab_channel=TomElliott),” who goes through step by step how you can form a text as a comma-separated values (CSV) file and how to use OpenRefine and Geocollider (after 17:08). Check also his blog post “[Using OpenRefine With Pleiades](http://horothesia.blogspot.com/2017/10/using-openrefine-with-pleiades.html),” in Horothesia, October 13, 2017.

## Notes 

#### Helpfull websites
- Google Maps Satellite Imagery
  - `https://mt1.google.com/vt/lyrs=y&x={x}&y={y}&z={z}`.
- [Ancient World Mapping Center](http://awmc.unc.edu/wordpress/), that provides different resources for diggital mapping of the ancient world. You may want to check the Spapefiles in [Resources](http://awmc.unc.edu/wordpress/map-files/).
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
- [EarthExplorer](https://earthexplorer.usgs.gov/). It requires registration. [Watch Obtaining + Loading Landsat Imagery in QGIS 3.10](https://www.youtube.com/watch?v=mBk2VIMawRE&ab_channel=MiddleburyRemoteSensing) for a step-by-step guide on how to use the data from EarthExplorer.
- [Natural Earth](https://www.naturalearthdata.com/downloads/10m-raster-data/10m-natural-earth-2/).

