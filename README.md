
<!-- README.md is generated from README.Rmd. Please edit that file -->
ESRI Leaflet bindings.
----------------------

ESRI bindings for the [leaflet](https://www.github.com/rstudio/leaflet) package, based on the [ESRI leaflet plugin](https://esri.github.io/esri-leaflet/). This package is part of the leaflet ecosystem of R packages for web mapping.

**Compatibility Matrix**

<table>
<colgroup>
<col width="19%" />
<col width="22%" />
<col width="33%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Leaflet JS ver.</th>
<th>R Leaflet pkg ver.</th>
<th>esri-leaflet JS Plugin ver.</th>
<th>R leaflet.esri pkg ver.</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><a href="https://github.com/Leaflet/Leaflet/releases/tag/v0.7.7">0.7.x</a></td>
<td><a href="https://github.com/rstudio/leaflet">1.1</a> <sup>1</sup></td>
<td><a href="https://github.com/Esri/esri-leaflet/releases/tag/v1.0.4">1.0.4</a></td>
<td>0.1.x</td>
</tr>
<tr class="even">
<td><a href="https://github.com/Leaflet/Leaflet/releases/tag/v1.0.1">1.x</a></td>
<td>? <sup>2</sup></td>
<td><a href="https://github.com/Esri/esri-leaflet/releases/tag/v2.0.4">2.x</a></td>
<td>?</td>
</tr>
</tbody>
</table>

-   1: Release 1.1 of the leaflet package should hit CRAN very soon, for now `devtools::install_github('rstudio/leaflet')`.
-   2: The R package has not yet been proted to Leaflet JS 1.x

### Features Tracking

**NOTE** It may not be possible to implement each and every feature and the documentation will be updated accordingly. Each feature which is implemented has a tick mark (✔️) next to it. Any description you find in this section is directly taken from the esri-leaflt [API reference](https://esri.github.io/esri-leaflet/api-reference/).

#### Layers

Layers provide visualization capabilities for data hosted in Feature Services, Map Services and Image Services.

-   [Basemap Layer](https://esri.github.io/esri-leaflet/api-reference/layers/basemap-layer.html) ✔️
-   [Dynamic Map Layer](https://esri.github.io/esri-leaflet/api-reference/layers/dynamic-map-layer.html)
-   [Image Map Layer](https://esri.github.io/esri-leaflet/api-reference/layers/image-map-layer.html)
-   [Raster Layer](https://esri.github.io/esri-leaflet/api-reference/layers/raster-layer.html)
-   [Tiled Map Layer](https://esri.github.io/esri-leaflet/api-reference/layers/tiled-map-layer.html)
-   [Feature Layer](https://esri.github.io/esri-leaflet/api-reference/layers/feature-layer.html)
-   [Cluster Feature Layer](https://esri.github.io/esri-leaflet/api-reference/layers/clustered-feature-layer.html)
-   [Heat Feature Layer](https://esri.github.io/esri-leaflet/api-reference/layers/heatmap-feature-layer.html)
-   ~~[Vector Basemap](https://esri.github.io/esri-leaflet/api-reference/layers/vector-basemap.html)~~ Cannot be supported for now as this requires leaflet 1.x.
-   ~~[Vector Layer](https://esri.github.io/esri-leaflet/api-reference/layers/vector-layer.html)~~ Cannot be supported for now as this requires leaflet 1.x.

#### Controls

-   [Geosearch](https://esri.github.io/esri-leaflet/api-reference/controls/geosearch.html)

#### Tasks

Tasks are wrappers for commonly used API methods on ArcGIS services. They expose commonly used parameters to make them more accessible to Leaflet.

-   [Query](https://esri.github.io/esri-leaflet/api-reference/tasks/query.html)
-   [Find](https://esri.github.io/esri-leaflet/api-reference/tasks/find.html)
-   [IdentifyFeatures](https://esri.github.io/esri-leaflet/api-reference/tasks/identify-features.html)
-   [IdentifyImage](https://esri.github.io/esri-leaflet/api-reference/tasks/identify-image.html)
-   [Geocode](https://esri.github.io/esri-leaflet/api-reference/tasks/geocode.html)
-   [Reverse Geocode](https://esri.github.io/esri-leaflet/api-reference/tasks/reverse-geocode.html)
-   [Suggest](https://esri.github.io/esri-leaflet/api-reference/tasks/suggest.html)
-   [Geoprocessing Task](https://esri.github.io/esri-leaflet/api-reference/tasks/gp-task.html)
-   [Query Related](https://esri.github.io/esri-leaflet/api-reference/tasks/query-related.html)

#### Events

[Event](https://esri.github.io/esri-leaflet/api-reference/events.html) types common across components of Esri Leaflet.

-   loading
-   load
-   createfeature
-   removefeature
-   addfeature
-   ???

### License

This package is released under [MIT](https://opensource.org/licenses/MIT).

### Known Issues

-   Basemap not displayed in RStudio Viewer (but they do show in external browser or when the viewer is opened in a separate window).