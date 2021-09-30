# Synchronization

## When I synchronise my data, I get some files with 'conf' in their names

Input supports collaborative editing, if you use Geopackage file format for your survey layer. If you use for example ESRI Shapefile for your survey layer, Input is not able to detect changes from other users and overwrites them. It will keep a copy of the overwritten files with 'conf' in the name. So, in summary, **always use Geopackage for your survey layer**.

## I use Geopackage for my survey layer, but I still see 'conf' files

 Input does not support changing of the data schema. So, if you delete or add columns to your survey layer, Input cannot detect the change. Therefore, it is always recommended to stick with the same attribute table structure once you have set up your survey layer.

 Another reason you might be seeing conf files is due to [storing raster data in Geopackage](https://github.com/lutraconsulting/geodiff/issues/91) for your survey layer. We recommend using GeoTIFF or at least a separate Geopackage database for all your raster files. 

## I cannot synchronise changes from the Mergin server

 - Make sure you have data connectivity.
 - Ensure you have not exceeded or reached your storage allowance