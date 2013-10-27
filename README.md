Ext.ux.ColorPicker
==================

Ext.ux.ColorPicker


Colorpicker field for Ext Js, an extension of similar functionality originally coded by Ryan Petrello in 2011. To use, simply add references to the JS and CSS scripts in your page. A color picker field can then be created using Ext.create('Ext.ux.ColorPicker'); You will need to also specify the location of the luminance and spectrum.png images, by setting the luminanceImg and spectrumImg properties on the object (or replacing the two related incidences in the main JS). E.g. 

('Ext.ux.ColorPicker', {
  luminanceImg:'images/luminance.png',
  spectrumImg:'images/luminance.png'
});


Requires <canvas> support.
