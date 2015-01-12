John Snow
========
Recreation of John Snow's famous 1854 London cholera map. 
Data borrowed from Robin Wilson and converted to WGS84 geojson.
http://blog.rtwilson.com/john-snows-famous-cholera-analysis-data-in-modern-gis-formats/

I've also added a field to the cholera death points, showing distance from the infected well, which can be used for interesting made up temporal visualizations. 
A georeferenced image can also be added from my mapbox account as a basemap in cartodb using gisbill.Snow.

The cartocss code is for pumps data. See more here: https://www.mapbox.com/tilemill/docs/manual/carto/

The popups code is also for the pumps. Popups code is written in Mustache templates. See more here: http://mustache.github.io/ There is some built in logic in this code, but note that any <script> tags in this code would break the entire viz.

Also included is some code for a simple Odyssey.js map (in markdown), detailed below. Be sure to change the viz code to match your own viz url.
http://cartodb.github.io/odyssey.js/
