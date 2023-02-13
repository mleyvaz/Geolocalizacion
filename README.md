
    <script>
      if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(function(position) {
          var latitude = position.coords.latitude;
          var longitude = position.coords.longitude;
          document.getElementById("location").innerHTML =
            "Latitud: " + latitude + "<br>Longitud: " + longitude;
        });
      } else {
        document.getElementById("location").innerHTML =
          "Lo siento, tu navegador no soporta la ubicación GPS.";
      }
    </script>


