# AngularPipes
My Collection of Custom Angular Pipes

Temperature Conversion Pipe
===============================================================
Use the pipe like this to convert from Celsius to Fahrenheit:
value | temperature: 'c' : 'f'
0 => 32°F

This will convert the value, do decimal pipe 1.0-1, and add the appropriate symbol 'F'


The pipe can also just add the unit for you if that is all you need:
value | temperature: 'f'
32°F

The pipe will convert Celcius, Fahrenheit, and Kelvin.
