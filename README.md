Details of the procedure

Here is a detailed description of our procedure:
In concrete terms, the script will use the three-dimensional file in its .wrl form and import it into ArcGis, which transforms it into an .shp file and is then able to consider it in its environment. On this basis, it measures a series of data to create raster and shapefile files, following a defined procedure.
In ArcGis, we insert the script, which will use the documents stored in a folder on the computer's desktop, called Paleospeleology, to carry out its operations.
The results are organised in a folder into a series of subfolders. These are made up of several elements: 
1) Temporary results files, used to perform the calculations required for other files
2) Final results files, whose data will subsequently be interpreted and integrated into the statistics. 

It is necessary to apply the script to each motif one by one, naming the shapefile of the graphic unit analysed ‘GU’. 
It should be pointed out that the results are sent to the same folder in the Office and then need to be moved when it's time to analyse another pattern, because the script application will systematically send its results to the same location.
Files needed to run the script
The two scripts each need a series of files to work. It is necessary to apply Script_general first, as it will provide some of the data needed to apply Script_for_each_hand. The documents required for the analysis are as follows.
1) Script_general
- The shapefile of the access point to the cavity: ‘Access.shp’.
- The shapefile of the entire cavity's negative hands: ‘Allin.shp’.
- The 3D file of the entire cave in its Palaeolithic state: ‘CeilingsMax.wrl’.
- The 3D file of the lower ceilings of the cave, in the case of superimposed levels, in their Palaeolithic state: ‘CeilingsMin.wrl’.
- The shapefile of the deepest point of the cave: ‘Depths.shp’.
- The 3D file of the cave floor in its Palaeolithic state: ‘GroundOk.wrl’.
- The script in the form of a python document: ‘Script_Général_1.py’.
2) Script_pour_chaque_main
- The shapefile of the access point to the cavity: ‘Access.shp’.
- The 3D shp file of the entire cave in its Palaeolithic state (obtained by applying Script_general): ‘CeilingsMax.shp’.
- The shapefile of the deepest point of the cave: ‘Depths.shp’.
- The image of the floor of the cavity (obtained by applying the Script_general): ‘GroundOk.tif’.
- The shapefile of the graphic unit to be analysed: ‘GU.shp’.
- The image of the cavity ceilings (obtained by applying Script_general): ‘Height.tif’.
- The script in the form of a python document: ‘Script_for_each_hand.py’.
