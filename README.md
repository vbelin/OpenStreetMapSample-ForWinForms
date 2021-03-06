# Open Street Map Sample for WinForms

### Description
OpenStreetMap (OSM) is a collaborative project to create free geographic data for the entire world. It can be thought of as a "Free Wiki World Map". The latest version of MapSuite now supports this.  

Please refer to [Wiki](http://wiki.thinkgeo.com/wiki/map_suite_desktop_for_winforms) for the details.

![Screenshot](https://github.com/ThinkGeo/OpenStreetMapSample-ForWinForms/blob/master/ScreenShot.png)

### Requirements
This sample makes use of the following NuGet Packages

[MapSuite 10.0.0](https://www.nuget.org/packages?q=ThinkGeo)

### About the Code

**The preceeding code is added to the load event for your application.**

The first step is to set `winformsMap.MapUnit` to `GeographyUnit.Meters`. 
You'll then be able to add the OpenStreetMap overlay with the following code:
```csharp
OpenStreetMapOverlay osmOvelerlay = new OpenStreetMapOverlay();
winformsMap.Overlays.Add(osmOvelerlay);
```
Once the overlay is added, be sure to call `winformsMap.Refresh()` to get the map to draw the new layer. 

### Getting Help

[Map Suite Desktop for Winforms Wiki Resources](http://wiki.thinkgeo.com/wiki/map_suite_desktop_for_winforms)

[Map Suite Desktop for Winforms Product Description](https://thinkgeo.com/ui-controls#desktop-platforms)

[ThinkGeo Community Site](http://community.thinkgeo.com/)

[ThinkGeo Web Site](http://www.thinkgeo.com)

### Key APIs
This example makes use of the following APIs:

- [ThinkGeo.MapSuite.WinForms.OpenStreetMapOverlay](http://wiki.thinkgeo.com/wiki/api/thinkgeo.mapsuite.winforms.openstreetmapoverlay)

### About Map Suite
Map Suite is a set of powerful development components and services for the .Net Framework.

### About ThinkGeo
ThinkGeo is a GIS (Geographic Information Systems) company founded in 2004 and located in Frisco, TX. Our clients are in more than 40 industries including agriculture, energy, transportation, government, engineering, software development, and defense.
