## Weather Fun

### \*\*City input is not hooked up atm\**
### TODOS

- get rid of jQuery function and make everything angular
- button for update function and on city change
- cache id's for already fetched cities
- display current conditions, etc. as "cards"
    - add the rest of the current cond. info
- allow multiple cards on screen at once
- allow drag'n'drop to reorder cards
- set a home city
- still need to display forecast
- add history (i think there is another openweathermap.org nodel library that does this)
- graphing of history
    - yesterday
    - this day last week/month/year
    - statistics like mean, sd, mode, median
- use more icons
- show trends in current cond. like rising and falling temp, hum, pressure, etc
    - changes in wind direction
- buttons to show forecast, history, charts



#### Usage (from weather.js readme)

At the moment you can access the current weather conditions and the
forecast for any city. By default it will use the closest match as
returned by Open Weather Map.

```javascript
Weather.getCurrent("Kansas City", function(current) {
  console.log(
    ["currently:",current.temperature(),"and",current.conditions()].join(" ")
  );
});

Weather.getForecast("Kansas City", function(forecast) {
  console.log("forecast high: " + forecast.high());
  console.log("forecast low: " + forecast.low());
});
```

[openweathermap.org]: http://openweathermap.org
[Weather.js]: http://github.com/noazark/weather
[Sugar.js]: http://sugarjs.com/
[jQuery]: http://jquery.com/