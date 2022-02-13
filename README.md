# Visibility Analysis (VGA) on Dota 2 Maps

![GIF](https://github.com/RyanTanYiWei/Dota2VGA/blob/main/VGA%20Analysis/Diagrams/fixed%20scale.gif)

[Blogpost](https://ryantanyiwei.wixsite.com/blog/dota2-map)

![2Raster](https://github.com/RyanTanYiWei/Dota2VGA/blob/main/Sample%20Diagrams/Raster%20File.png)
![4VGAUnprocessed](https://github.com/RyanTanYiWei/Dota2VGA/blob/main/Sample%20Diagrams/VGA%20Unprocessed.png)
![5VGAProcessed](https://github.com/RyanTanYiWei/Dota2VGA/blob/main/Sample%20Diagrams/VGA%20Processed.png)
![7R](https://github.com/RyanTanYiWei/Dota2VGA/blob/main/Sample%20Diagrams/VGA%20R.png)
<img height = "146" src=https://github.com/RyanTanYiWei/Dota2VGA/blob/main/Sample%20Diagrams/QGIS.JPG />

<b> Technical Pipeline:</b>


> data acquisition (R)
1) Download/Borrow Raster Files from https://github.com/devilesk/dota-interactive-map
2) Crop Raster Files and Combine Layers (Trees and Boundary)
3) Convert Rasters into Polygons/Polylines

> data processing (DepthmapX)
4) Import Data into DepthmapX
5) Run VGA - Visual Graph Analysis

> data preprocessing and visualization (R)
6) Import VGA as SpatialPixelsDataFrame
7) Plot SpatialPixelsDataFrame
8) Build Time-Series Plot Animations
9) Resize SpatialPixelsDataFrame to fit map image (260x260) -> (4096x4096)

> analysis (QGIS)
10) Visualize in QGIS alongside full Map Images


  
  *You probably could do this manually, but because of the large number of map files- I did it as a batch process mostly in R.
