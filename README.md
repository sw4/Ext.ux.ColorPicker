Ext.ux.ColorPicker
==================

HTML5 colorpicker field for Ext JS, extending functionality originally coded by Ryan Petrello in 2011. 

Specify the location of the luminance and spectrum.png images, by setting the luminanceImg and spectrumImg properties on the object (or replacing the two related incidences in the main JS). E.g. 

```
Ext.create('Ext.ux.ColorPicker', {
  luminanceImg:'images/luminance.png',
  spectrumImg:'images/luminance.png'
});
```

Requires canvas support and is based on a standard Ext triggerfield, so supports all native properties.


Sample Use
==================

```
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
```

```
Ext.create('Ext.ux.ColorPicker', {
  luminanceImg:'images/luminance.png',
  spectrumImg:'images/luminance.png',
  value:'#ff0000'
});
```
