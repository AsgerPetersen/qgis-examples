# Example using Septima shadow WMS in QGIS with TimeManager

The project is created using QGIS 3.6 with the TimeManager plugin v.3.0.2.

Note: If you get an exception message like `"WMSTRasterLayer" object has no attribute "resetSubsetString"` you need to uninstall and reinstall TimeManager.

When the project has loaded enable TimeManger. Now the shadows will be calculated for the time set in TimeManager.

The layer `Shadows` uses a WMS-T service from Septima. The service uses the [Danish DSM](https://www.geodata-info.dk/srv/eng/catalog.search;#/metadata/6cedf383-ad5d-4040-a88d-54d037d467b5) to calculate accurate shadows for the specified time. The WMS-T service also allows specifying additional 2.5D objects in the request which will be applied to the DSM before shadow calculation. This particular layer adds an object which represents the proposed 320m "Bestseller tower". 

The used service is a demo which is constrained to the area around the town of Brande.

Background maps are from [Kortforsyningen / The Danish Map Supply](https://kortforsyningen.dk/indhold/english).