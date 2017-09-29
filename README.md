# Bokeh Bike Elevation Map
A visual representation of Austin's bike paths mapped to a color gradient to show elevation changes.


# Process
A .geoJSON file of line data is imported from <a href="https://mapzen.com/data/metroextracts/metro/austin_texas/">Mapzen</a> to supply the lines of the map.

The lines are aggregated my latitude and longitude then split into consecutive coordinates. These coordinates are averaged and fed into the Google Map API for it's elevation.

This is then mapped to an RGB value. Combined with the line segment this is plotted to reveal a color map gradient corresponding each line to its elevation.

### To-Do
This is in test mode right now so the color mapping is not complete right now
