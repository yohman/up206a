# Creating an interactive web map

Make sure you have set up your local web server.

## Create a leaflet map
Open your text editor of choice, and enter the following code:
```javascript
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
