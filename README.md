Tabletop Weather Station, with sound pressure sensor support 
============================================================

The Tabletop Weather Station is an open source touch-capable weather station.
It measures temperature, humidity, air pressure and air quality index with
high precision.

See `here <https://www.tinkerforge.com/en/doc/Kits/TabletopWeatherStation/TabletopWeatherStation.html>`__ for more details.

This fork adds suport for the tinkerforge sound pressure sensor and the RGB-Led

Currently I have added:

* display of current decibel value on the first screen in a new column
* storing the decibel value in the sqlite db, like all other values
* graphics screen like the other screens for temperature, humidity, etc.
* if the led-bricklet is connected, it changes the color according to the sound level:
    * green for less than 55 decibel, suitable for knowledge work
    * yellow for 55-70 db, suitable for simple work
    * orange for more than 70 db
    * red for more than 80 db

![The start screen of the weather station shows also the sound pressure in decibel](/demo/screenshots/weatherstation-start-320.jpg?raw=true)

![A graph that shows how the decibel values changes over time](/demo/screenshots/weatherstation-decibelgraph-320.jpg)
