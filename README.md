Ext.ux.ColorPicker
==================

Ext.ux.ColorPicker


Colorpicker field for Ext Js, an extension of similar functionality originally coded by Ryan Petrello in 2011. To use, simply add references to the JS and CSS scripts in your page. A color picker field can then be created using Ext.create('Ext.ux.ColorPicker'); You will need to also specify the location of the luminance and spectrum.png images, by setting the luminanceImg and spectrumImg properties on the object (or replacing the two related incidences in the main JS). E.g. 

Ext.create('Ext.ux.ColorPicker', {
  luminanceImg:'images/luminance.png',
  spectrumImg:'images/luminance.png'
});


Requires canvas support and is based on a standard Ext triggerfield, so supports all native properties.


Sample Use
==================


<!doctype html>
<html lang="en">
	<head>
		<meta charset="utf-8">	
		<!-- Link to EXT JS Theme -->
		<link rel="stylesheet" href="theme.css ">	
		<!-- Link to ExtJS library -->
		<script src="ext-all.js"></script>
		<!-- Link to Ext JS ColorPicker  -->
		<script src="Ext.ux.ColorPicker.min.js"></script>
		<link rel="stylesheet" href="Ext.ux.ColorPicker.min.css">
	</head>
	<body></body>
</html>


Sample Use Within your Ext JS Application
==========================================

Ext.create('Ext.ux.ColorPicker', {
  luminanceImg:'images/luminance.png',
  spectrumImg:'images/luminance.png',
  value:'#ff0000'
});
