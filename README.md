# StuVe_rooms2020
GeoJson files (maps) for mapping public and quasi-public rooms of the StuVe@Uulm on an OSM-Type Map

The first version of this file was created with <umap.openstreetmap.de>
Worklink: <https://umap.openstreetmap.de/de/map/anonymous-edit/2550:XoHenbQpgNNkk1GtzKfr5f2edZc>

[comment]: <> (in  the output file unless you use it in)
[//]: <> (This is also a comment.)
[//]: # (This may be the most platform independent comment)

**documentation/help for umap**

- https://wiki.openstreetmap.org/wiki/UMap/Guide
- https://wiki.openstreetmap.org/wiki/UMap/Tips

**other**

Because different "OSM-Viewers" work different, testing was done on several other sites
- <https://geojson.net/#16/48.4236/9.9559>
- <http://geojson.tools/>
- <

---
# CODE (per dataset/node/point)
``` geojson
{
      "type": "Feature",
      "properties": {
```

## Optional Data
As mentioned above, these informations are only usefull via umap. For usage in other applications they may be ignored/deleted.

``` geojson
        "_umap_options": {
          "color": " ",
          "showLabel": null,
          "labelDirection": " "
        },
```
## Mandatory Data
``` geojson
{
      "type": "Feature",
      "properties": {
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
- `_umap_options` :: Because umap was used for the first version. These properties may be drafted
	 -  `color` :: color of the umap-marker (value =`"YellowGreen"` for Fachschaften; `"DeepSkyBlue"` for StuVe rooms)
	 -  `showLabel` :: determines that there will be a label in umap (value = `null`)
	 -  `labelDirection` :: direction of the umap label (value = `"right"` for Fachschaften; `"left"` for StuVe rooms)
- `name` :: name of the room
- `description` :: additional information
- `ref` :: reference = "room number"
- `website`(optional) :: website url
- `marker-color` :: (value = `"#a4ba2e"` for  Fachschaften; `"#4abbeb"` for StuVe rooms)
- `marker-size` :: (value = `medium`)
- `marker-symbol` :: OSM Node-Icon, (value= `"marker"` for open rooms; `"marker-stroked"` for only-StuVe-rooms). more can be found here: <https://map.michelstuyts.be/icons/>
- `LATITUDE` :: (~values for Ulm = (min `48.3800`; max `48.4200`))
- `LONGITUDE` :: (~values for Ulm = (min `9.9300`; max `9.9700`))
