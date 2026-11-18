# sillyserver map data
Map landmark data for the sillyserver map webpage. [www.sillyserver.win/minecraft/map](https://www.sillyserver.win/minecraft/map)
# Data Structure
All the data is stored in JSON format. Thumbnail images should be 256px by 256px in .webp format with a file size less than 20kb. 
# Usage
Data can be accessed by downloading the .json file from this repository, or from [https://data.sillyserver.win/sillyserver-landmarks.json](https://data.sillyserver.win/sillyserver-landmarks.json)
# Required fields
## name
```String```
The name of the location in plain text.
## size
```String```
The style of label.
label-large
label-medium
label-small
## coordinates
```Array```
An array with two entries: the east/west coordinate, and the north/south coordinate.
Ex. ```[-570, 310]```
## type
For view filtering.
settlement
building
farm
# Optional fields
If the field is unused, mark it with boolean false.
## thumbnail
```String```
A url to the thumbnail image. Images should be 256px by 256px in .webp format with a file size less than 20kb.
## image
```String```
A url to the location image. A larger image used in the info panel for a location. Images should be 1920px by 1080px in .webp format with a file size less than 500kb.
## description
```String```
A description of the location used for the info panel.
## builder
```Array```
The username of the builder(s). In cases where the builder is unknown enter "Unknown".