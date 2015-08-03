# impact_mapping
var CaliOverlay;

function initialize(){

  var Cali = new google.maps.LatLng(37,-120);
  var imageBounds = new google.maps.LatLngBounds(
    new google.maps.LatLng(42.030941, -120.020349),
    new google.maps.LatLng(32.534939, -117.127079));
    
  var mapOptions = {
    zoom: 6
    center: Cali
  };

  var map = new.google.maps.Map(document.getElementById ('map-canvas'), mapOptions);
  
  CaliOverlay = new google.maps.GroundOverlay('http://i57.tinypic.com/2rz6w7n.jpg', imageBounds);
  CaliOverlay.setMap(map);
}

google.maps.event.addDomListener(windor, 'load', initialize);
