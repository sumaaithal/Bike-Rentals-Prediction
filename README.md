# Bike-Rentals-Prediction
The objective of the project is - using historical usage patterns and weather data, forecast(predict) bike rental demand (number of bike users (‘cnt’)) on hourly basis.

The dataset has following features:
<ol>
  <li>instant: record index</li>
  <li>dteday : date </li>
  <li>season: season (1: springer, 2: summer, 3: fall, 4: winter)</li>
  <li>yr: year (0: 2011, 1:2012)</li>
  <li>mnth: month (1 to 12)</li>
  <li>hr: hour (0 to 23)</li>
  <li>holiday: whether the day is a holiday or not</li>
  <li>weekday: day of the week</li>
  <li>workingday: if day is neither weekend nor holiday is 1, otherwise is 0.</li>
  <li>weathersit:
    1: Clear, Few clouds, Partly cloudy, Partly cloudy
    2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
    3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
    4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
  <li>temp: Normalized temperature in Celsius. The values are derived via (tt_min)/(t_maxt_min), t_min=*8, t_max=+39 (only in hourly scale) </li>
  <li>atemp: Normalized feeling temperature in Celsius. The values are derived via (tt_min)/(t_maxt_min), t_min=*16, t_max=+50 (only in hourly scale)</li>
  <li>hum: Normalized humidity. The values are divided to 100 (max)</li>
  <li>windspeed: Normalized wind speed. The values are divided to 67 (max)</li>
  <li>casual: count of casual users</li>
  <li>registered: count of registered users</li>
  <li>cnt: count of total rental bikes including both casual and registered users</li>
  The "target" data set ('y') should have only one 'label' i.e. 'cnt'.
</ol>

The methods followed to create the ML models are:
<ol>
  <li>perform EDA</li>
  <li>preprocess the data - to clean,scale using standardizer</li>
  <li>instantiate differnt model and use the cross validation to estimate the root mean squared errors</li>
  <li>train the final model obtained from step 4</li>
  <li>predict and evaluate the model</li>
  
</ol>
