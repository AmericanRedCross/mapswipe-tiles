
https://github.com/mapbox/tippecanoe
https://github.com/mapbox/mbutil
https://github.com/klokantech/mapbox-gl-js-offline-example


```
tippecanoe -o results.mbtiles -z18 results.json

mb-util --image_format=pbf results.mbtiles results
cd results
gzip -d -r -S .pbf *
find . -type f -exec mv '{}' '{}'.pbf \;
```
