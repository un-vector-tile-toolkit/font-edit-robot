# font-edit-robot
A repository to develop glyphs rendered as SDFs.  
I convert ttf fonts into pbf files using unvt/nanban and mapbox's node-fontnik.
Please note that Roboto fonts have their own license (Apache License).  

## background
I wanted to have PBF fonts for our web map. 

## install
```console
git clone https://github.com/un-vector-tile-toolkit/font-edit-robot
cd font-edit-robot
Docker run -it --rm -v ${PWD}:/data unvt/nanban
cd /data
git clone https://github.com/mapbox/node-fontnik
cd node-fontnik
npm install
make
cd ..
./node-fontnik/bin/build-glyphs Roboto/Roboto-(xxx).ttf (outputlocation)

```


## source
ttf fonts are donwnloaded from https://fonts.google.com/specimen/Roboto
