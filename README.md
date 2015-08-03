# impact_mapping
<!DOCTYPE html>
<html>
  <head>
    <style type="text/css">
      html, body, #map-canvas { height: 100%; margin: 0; padding: 0;}
    </style>
    <script tpye="text/javascript"
      src="https://maps.googleapis.com/maps/api/js?key=AIzaSyB1LUVeu649Y9tdgOuF9calGE-UY3Wn9Ik">
    </script>
    <script tpy="text/javascript">
      function initialize() {
          var mapOptions = {
            center: { lat: 37, lng: -120},
            zoom: 6
          };
          var map = new google.maps.Map(document.getElementById('map-canvas'),
          mapOptions) ;
      }
      google.maps.event.addDomListener(window, 'load', initialize) ;
    </script>
  </head>
  <body>
<div id="map-canvas"></div>
  </body>
 </html>
