# Aloghides AngularPipes
My collection of custom Angular Pipes

## Temperature Units and Conversion Pipe
The temperature pipe will convert the value, do decimal pipe 1.0-1, and add the appropriate unit symbol.
The pipe will convert Celcius, Fahrenheit, and Kelvin. 
- Accepted units are 'C', 'F', and 'K' and not case sensitive.

### Usage 1 - Conversions


```angular
{{ value | temperature: 'input unit' : 'output unit' }}
```
##### Convert Celsius to Fahrenheit:
```angular
{{ 0 | temperature: 'c' : 'f' }}

32°F
```

### Usage 2 - Append Units

##### Append the unit symbol to your value:
```angular
{{ 32 | temperature: 'f' }}

32°F
```

## Wind Direction - Degrees to Cardinal Direction Conversion Pipe
The windDirection pipe will convert the value of degrees to a cardinal direction.
- Ouput values are 'calm', 'NNE', 'NE', 'ENE', 'E', 'ESE', 'SE', 'SSE', 'S', 'SSW', 'SW', 'WSW', 'W', 'WNW', 'NW', 'NNW', 'N'
- Per NWS Glossary:
  The true direction from which the wind is blowing at a given location (i.e., wind blowing from the north to the south is a north wind).
  It is normally measured in tens of degrees from 10 degrees clockwise through 360 degrees. North is 360 degrees.
  A wind direction of 0 degrees is only used when wind is calm. 

### Usage 1 - Conversions


```angular
{{ value | windDirection }}
```
##### Convert Degrees to Cardinal Direction:
```angular
{{ 135 | windDirection }}

SE
```

## Wind Speed - Common Wind Speed Unit Conversion Pipe
The windSpeed pipe will convert units commonly used for measuring wind speed.  It will convert, do decimalPipe 1.0-1, and add the unit symbol.
- Accepted units are 'mph', 'kph', 'ms', and 'kts'.  The pipe can convert between any two of these units.
- That is miles per hour, kilometers per hour, meters per second, and knots.

### Usage 1 - Conversions


```angular
{{ value | windSpeed: 'input unit' : 'output unit' }}
```
##### Convert kilometers per hour to miles per hour:
```angular
{{ 10 | windSpeed: 'kph' : 'mph' }}

6.2mph
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
