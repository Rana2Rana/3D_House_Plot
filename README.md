# 3D_House_Plot


### Project overview
This project is to plot a three dimentional projection for any building in Flanders.

Just by providing the address of that building.

 
### Instructions

* Clone the repository.
* Run the code.
* Give the address without spaces

### Requirements
python 3.9 or 3.10

Python libraries:
* `requests`
* `json`
* `os`
* `shapely`
* `rasterio`
* `plotly`


### Project Steps
1. Providing the address as street name, house number, zip_code, city without spaces.
2. Match the address with correct `API`.
3. Get the coordinates.
4. Check this coordinates in which file of the Digital Surface Model (DSM) and Digital Terrain Model (DTM).
5. Clip the target zone from the DSM.tif
6. Clip the target zone from the DTM.tif
7. Subtract the Clipped DTM from the Clipped DSM to compute The Canopy Height Model CHM.
8. Plot the CHM.

### Contributing
Any kind of contributions are welcome. 

1. Fork the Project.
2. Create your Feature Branch.
3. Commit your Changes.
4. Push to the Branch.
5. Open a Pull Request.

### Difficulties
1. Some Libraries like rasterio was not able to install. So the right way to install some libraries packages is: to load the .whl packages then install it.
2. Selecting the way of clipping the tif files.

### Conclusion 
1. Find a way to void the gapping in the plot image that appear in some addresses.
2. Access The DSM Files and DTM files without loading or extracting them.
