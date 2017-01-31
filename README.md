Leaflet.markercluster.webpack
=====================

Leaflet markercluster (https://github.com/Leaflet/Leaflet.markercluster) structured with webpack.

### Install

Install with npm: `npm install --save leaflet.markercluster.webpack`

### Usage

```javascript
require('leaflet.markercluster.webpack');
```

### Notes
This module already requires 'leaflet', so don't require it again.
Also, the css files from leaflet and markercluster are already required too. 

Also, the L object is exposed:

```javascript
var L = require('leaflet.markercluster.webpack');
```
### Build Notes
As this module requires some css files, you have to install a css loader.

Installing:
```bash
npm install --save-dev css-loader style-loader  
```

And configure the loader in webpack.config:
```javascript
{ 
    test: /\.css$/, loader: "style-loader!css-loader" 
}
```