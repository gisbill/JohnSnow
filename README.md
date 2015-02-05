John Snow
========
Recreation of John Snow's famous 1854 London cholera map, for educational use. Intended for a [CartoDB](http://www.cartodb.com) map.
Data borrowed from [Robin Wilson](http://blog.rtwilson.com/john-snows-famous-cholera-analysis-data-in-modern-gis-formats/) and converted to web mercator [geojson](http://geojson.io).

I've also added a field to the cholera death points, showing distance from the infected well, which can be used for interesting, though made up, temporal visualizations using [torque](http://github.com/CartoDB/torque).
A georeferenced image can also be added from my mapbox account as a basemap in cartodb using gisbill.Snow.
If you want to play around with adding other custom basemaps, here are many provider [examples](http://leaflet-extras.github.io/leaflet-providers/preview/), or you can try modifying the url from Stamen's [Map Stack](http://mapstack.stamen.com/).

The [cartocss](http://www.mapbox.com/tilemill/docs/manual/carto/) code is for pumps data, and uses [maki](http://www.mapbox.com/maki/) icons.

The popups code is also for the pumps. Popups code is written with [Mustache](http://mustache.github.io/) templates. There is some built in logic (using mustache) forced into this code, but note that any javascript added to it would break the entire viz.
The cartodb 'description' field needs to be used, and an 'image' and 'link' text field needs to be added to pumps in order for some of the code here to work.

Also included is some code for a simple [Odyssey.js](http://cartodb.github.io/odyssey.js/) map (in [markdown](http://daringfireball.net/projects/markdown/)).
Be sure to change the vizjson line of code to match your own viz url.
