# impact_mapping


<!DOCTYPE html>
<html>
  <head>
    <meta name="viewport" content="initial-scale=1.0, user-scalable=no">
    <meta charset="utf-8">
    <title>Ground Overlays</title>
    <style>
      html, body, #map-canvas {
        height: 100%;
        margin: 0;
        padding: 0;
      }
    </style>
    <script src="https://maps.googleapis.com/maps/api/js?key=AIzaSyB1LUVeu649Y9tdgOuF9calGE-UY3Wn9Ik"></script>
    <script>
var CaliOverlay;

function initialize() {
  var Cali = new google.maps.LatLng(37,-120);
  var imageBounds = new google.maps.LatLngBounds(
      new google.maps.LatLng(42.030941, -120.020349),
      new google.maps.LatLng(32.534939, -117.127079));
  var mapOptions = {
    zoom: 6,
    center: Cali
  };
  
  car map = new google.maps.Map(document.getElementById('map-canvas'),
  mapOptions);
  CaliOverlay = new google.maps.GroundOverlay(
    'http://i57.tinypic.com/2rz6w7n.jpg',
    imageBounds);
  CaliOverlay.setMap(map);

}

google.maps.event.addDomListener(window, 'load', initialize);  

}
    </script>
  </head>
  <body>
    <div id="map-canvas"></div>
  </body>
</html>
