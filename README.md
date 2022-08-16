# Forge Viewer on GEO MAP

Display forge viewer model on Geo Map.

![](GEOMAP_forge_viewer.gif)

## Have your model on GEO MAP

1. Make sure that you already have your simple forge viewer, if not, checkout out how to [create simple viewer](https://petrbroz.github.io/forge-samples-docs/tutorials/simple-viewer/).
2. Create a new file under the `wwwroot` folder and name it `geo-three.ext.js`. Replace it's content with the following [snippet of code](https://github.com/wallabyway/geo-three-ext/blob/main/docs/geo-three.ext.js).
3. Replace all the instances of the `viewer` with `this.viewer` in your `geo-three.ext.js`.
4. Add the `GeoThreeExtension` extension to the viewer by updating the `viewer.js` as follows;

    (i). Start by importing your extension at the top of `viewer.js`

        import './geo-three.ext.js';

    (ii). Then add your extension to the viewer by updating the function `initViewer` with the following configurations.

        ...
        const config = {
            extensions: ['Autodesk.DocumentBrowser', 'GeoThreeExtension']
        };
        ...
5. Finally add the extension script to the `index.html`.

        ...
        <script type="text/javascript" src="./geo-three.ext.js"></script>
        ...













# Contributors

    Michael | Senior Software Engineer

# Author

    Harun G. G. | Forge Developer Advocate

