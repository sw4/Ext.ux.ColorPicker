Ext.ux.ColorPicker
==================

Ext JS 4.2x Color Picker Field

**Licensed under [cc by-sa 3.0](http://creativecommons.org/licenses/by-sa/3.0/) with attribution required**

**Demo can be viewed here: http://sw4.github.io/Ext.ux.ColorPicker**

Requirements
=====

Requires canvas support and is based on a standard Ext triggerfield, so supports all native properties. Requires ExtJS JS and CSS to be referenced in your page.*

<sup>*Currently only tested in ExtJS 4.2x</sup>

Usage 
=======
Specify the location of the luminance and spectrum.png images, by setting the luminanceImg and spectrumImg properties on the object (or replacing the two related incidences in the main JS). E.g. 

```
Ext.create('Ext.ux.ColorPicker', {
  luminanceImg:'images/luminance.png',
  spectrumImg:'images/luminance.png'
});
```

Additionally, you can pass a HEX color to `value` to initialize the field with a color already selected.


Sample HTML Page
==================

```
<!doctype html>
<html lang="en">
    <head>
        <title>Ext.ux.ColorPicker</title>
        <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
        <meta charset="utf-8">
        <!-- Ext.ux.ColorPicker CSS -->
        <link href="https://rawgithub.com/sw4/Ext.ux.ColorPicker/master/Ext.ux.ColorPicker.css" rel="stylesheet">
    </head>
    <body>
        <h1>Ext.ux.ColorPicker</h1>
        <p>Note: This specific example will not work correctly due to the fact assets are loaded cross-domain (from rawgithub.com) which contravenes canvas security policy.</p>
        <div id="colorPicker"></div>
        <!-- Ext JS -->
        <script src="http://docs.sencha.com/extjs/4.2.1/extjs-build/examples/shared/include-ext.js"></script>        
        <!-- Ext.ux.ColorPicker JS -->
        <script src="https://rawgithub.com/sw4/Ext.ux.ColorPicker/master/Ext.ux.ColorPicker.js"></script>
        <script> 
        Ext.onReady(function() {
            var colorPicker = Ext.create('Ext.ux.ColorPicker', {
                luminanceImg:'https://rawgithub.com/sw4/Ext.ux.ColorPicker/master/luminance.png',
                spectrumImg:'https://rawgithub.com/sw4/Ext.ux.ColorPicker/master/spectrum.png',
                value:'#ff0000'
            });
            colorPicker.render('colorPicker');
        });        
        </script>
    </body>
</html>
```
