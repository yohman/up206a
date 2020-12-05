# Creating an interactive web map

Before you start your web mapping, make sure you have [set up your local web server](https://github.com/yohman/up206a/blob/master/Weeks/Week10/W10-01-Setting%20up%20a%20local%20server.md).

## Create a leaflet map
Open your text editor of choice, and enter the following code:
```html
<!-- leaflet css -->
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css" integrity="sha512-xodZBNTC5n17Xt2atTPuE1HxjVMSvLVW9ocqUKLsCC5CXdbqCmblAshOMAS6/keqq/sMZMZ19scR4PsZChSR7A==" crossorigin=""/>

<!-- leaflet js -->
<script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js" integrity="sha512-XQoYMqMTK8LvdxXYG3nZ448hOEQiglfqkJs1NOQV44cWnUrBc8PkAOcXy20w0vlaXaVUearIOBhiXZ5V3ynxwA==" crossorigin=""></script>

<!-- the map div -->
<div id='map' style='width:800px;height:600px;'></div>

<!-- javascript -->
<script type="text/javascript">

	// create the leaflet map
	var map = L.map('map').setView([34.1, -118.4], 10);

	// osm basemap
	L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
	    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
	}).addTo(map);

</script>
```

- Save the file as `map.html`
- Launch a browser window, and type http://localhost:8000/map.html

## Change the basemap

Go [here](https://leaflet-extras.github.io/leaflet-providers/preview/) for a list of freely available basemaps.

For high quality maps, you can use Mapbox tiles. You will need to create an account and obtain an [access token](https://account.mapbox.com/).

In the map.html file, swap the basemap by replacing the code for `//osm basemap` with the following:

```javascript
L.tileLayer('https://api.mapbox.com/styles/v1/{id}/tiles/{z}/{x}/{y}?access_token={accessToken}', {
    attribution: 'Map data &copy; <a href="https://www.openstreetmap.org/">OpenStreetMap</a> contributors, <a href="https://creativecommons.org/licenses/by-sa/2.0/">CC-BY-SA</a>, Imagery © <a href="https://www.mapbox.com/">Mapbox</a>',
    maxZoom: 18,
    id: 'mapbox/streets-v11',
    tileSize: 512,
    zoomOffset: -1,
    accessToken: 'your.mapbox.access.token'
}).addTo(map);
```

For satellite imagery, replace the id value of `mapbox/streets-v11` to `mapbox/satellite-streets-v11`. Full list of styles at the time of this writing:

- `light-v10`
- `dark-v10`
- `outdoors-v11`
- `streets-v11`
- `satellite-v11`
- `satellite-streets-v11`

## Add a geojson file

Download the following ![geojson file](arrests.js), which was created as part of the Week 8 Spatial Autocorrelation lab.
