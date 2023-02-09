# THE PHANOMENA

### Description

This is the repository for storing Phanomena project files related to coding e.g. **Grasshopper (.ghx), Python, C# files**. \
We refer to the following folder on the server: **\\\\enac1files.epfl.ch\IBOIS\187_Phänomena\** . \
Please document uploaded files with a small **comment** and an **image** in the ReadMe below. \
The GitHub repository is necessary for code to avoid the clutter on the server which should normally be used only for drawings, large rhino files and documents. Work locally with your code in your computer, then send and retrieve files in this repository. HOW-TO GITHUB section will help you to use this repository :beer: . 

# HOW-TO GITHUB



### Send files
``` bash
git add --all
git commit -m "PREFIX message name"
git push
```

commit PREFIX rules for "git commit -m "PREFIX message name":
``` bash
"ADD detailed explanation what has been done" - new feature, e.g. added new file or folder
"FIX detailed explanation what has been done" - bug fix, e.g. grasshopper file change
"DOC detailed explanation what has been done" - documentation, e.g. you changed the readme file
"MISC detailed explanation what has been done" - unknown
```

### Get files
``` bash
git pull
```

# FOLDER STRUCTURE

### Grid

2023_02_29 - Addition by Petras Vestartas: \
Restaurant and biolab grid is stored in the following file: **phanomena_grid.ghx** 

These two buildings are generated from two boundary curves. There are 4 input curves because they refer to the ground and the roof. 
* First columns are created by division and interpolation of the side curves. 
* Second beams are added. 
* Thrid diagonals are added based on the user given points. Be aware that diagonals can be created in two directions.  
* Fourth, closed rectangles are created that represents the roof and floor grid. 

For baking the geometry and generating the Excel file use **phanomena_grid_excel.ghx** 
* The excel example is needed to measure the lengths of the beams, count them, specifiy units e.g. meters, and bake all the geometry to the appropriate layer in Rhino.

![image](https://user-images.githubusercontent.com/18013985/217834006-3ca7e29f-1b51-4a6c-9bda-c7b39739c64d.png)

