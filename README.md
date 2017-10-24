# Weath-app
  Simple weather app
  
# JQuery  
  https://cdnjs.cloudflare.com/ajax/libs/jquery/3.2.1/jquery.min.js
        
  
# Weather Api 
  http://simpleweatherjs.com/
  
# Code 
        $(document).ready(function() {
              $.simpleWeather({
                      location:781008,
                      woeid: '',
                      unit: 'C',
                      success: function(weather) {
                      html = '<h1>Weather App</h1><br><h3> '+weather.temp+'&deg;'+weather.units.temp+'</h3>';

                      html += '<span>'+weather.city+', '+weather.region+'</span></br>';
                      $("#weather").html(html);
                      },
                      error: function(error) {
                      $("#weather").html('<p>'+error+'</p>');
                      }
              });
      });
# Structure

  <li> JQuery </li>
  <li> Weather Api  </li>
  <li> Code </li>


# Demo
  <br>
     https://manashio.github.io/Weather-app/
  
