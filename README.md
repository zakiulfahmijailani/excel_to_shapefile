# Excel to Shapefile

I had a problem with an excel file containing latitude and longitude coordinates since I was unable to convert it to CSV WKT (Well-Known Text) file, which typically QGIS can simply read.

So I made an attempt to do that using Python. Despite the fact that the final file produced by this solution is an ESRI Shapefile (.shp), I feel it to be a better solution for me.

I suppose we could use QGIS or ArcGIS to convert the shapefile to a CSV WKT file later on.

The file that you need to prepare is an excel file with extension of .xlsx or .xlx. The file must at least contains 2 columns, which are latitude (first column) and longitude (later column).

Example of data file:

![picture](https://drive.google.com/uc?export=view&id=1e1tOiWRmkXE4IjKAD1xjijy5hUg3dpur)

Don't forget to pay attention to your column header name. In this case, they are `Latitude (X)`, and `Longitude (Y)`.

After your geodataframe created and saved in your Google Colab file directory. You can download your file from that directory and then you can plot it in QGIS, ArcGIS or any other similar application.

Example of the map product:

![picture](https://drive.google.com/uc?export=view&id=1fz9O4f2VNmCuNhw9vRh79iix2x-YaecN)
 
