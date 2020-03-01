# StuVe_rooms2020
GeoJson files (maps) for mapping public and quasi-public rooms of the StuVe@Uulm on an OSM-Type Map

The first version of this file was created with <umap.openstreetmap.de>
Worklink: <https://umap.openstreetmap.de/de/map/anonymous-edit/2550:XoHenbQpgNNkk1GtzKfr5f2edZc>

Because different "OSM-Viewers" work different, testing was done on several other sites
- <https://geojson.net/#16/48.4236/9.9559>
- <http://geojson.tools/>
- <

---
## Mandatory Properties
``` geojson
{
      "type": "Feature",
      "properties": {
        "_umap_options": {
          "color": " ",
          "showLabel": null,
          "labelDirection": " "
        },
        "name": " ",
        "description": "",
        "ref": " ",
        "marker-color": " ",
        "marker-size": "medium",
        "marker-symbol": " "
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          LATITUDE,
          LONGITUDE
        ]
      }
}
```
----
## Notes
- _umap_options :: Because umap was used for the first version. These properties may be drafted
-  color :: color of the umap-marker (value = "YellowGreen" for Fachschaften; "DeepSkyBlue" for StuVe rooms)
-  showLabel :: determines that there will be a label in umap (value = null)
-  labelDirection :: direction of the umap label (value = "right" for Fachschaften; "left" for StuVe rooms)
 
- marker-symbol :: OSM Node-Icon, (value= "marker" for open rooms; "marker-stroked" for only-StuVe-rooms. more can be found here: <https://map.michelstuyts.be/icons/>
- marker-color :: "#a4ba2e" for  Fachschaften; "#4abbeb" for StuVe rooms
