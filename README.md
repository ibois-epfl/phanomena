# Phanomena

This is the repository for storing Phanomena project files related to coding e.g. **Grasshopper (.ghx), Python, C# files**. \
We refer to the following folder on the server: **\\enac1files.epfl.ch\IBOIS\187_Phänomena** . \
Please document uploaded files with a small **comment** and an **image** in the ReadMe below. \
The GitHub repository is necessary for code to avoid the clutter on the server which should normally be used only for drawings, large rhino files and documents.

# How-to GitHub:

Work locally with your code in your computer, then send and retrieve files in this repository. \
Following commands will help you to get started:

to send the files:
``` bash
git add --all
git commit -m "PREFIX message name"
git push
```

commit PREFIX rules for "git commit -m "PREFIX message name":
``` bash
"ADD detailed explanation what has been done" - new feature, e.g. added new file or folder
"FIX detailed explanation what has been done " - bug fix, e.g. grasshopper file change
"DOC detailed explanation what has been done " - documentation, e.g. you changed the readme file
"MISC detailed explanation what has been done " - unknown
```

to get the files:
``` bash
git pull
```

# Folder Structure of  ibois-epfl / phanomena 

## grid

2023_02_29 - Addition by Petras Vestartas: \
Restaurant and biolab grid is stored in the following file: **phanomena_grid.ghx** \
For baking the geometry and generating the excel file for the structure use **phanomena_grid_excel.ghx** \
These two buildings are generated from two boundary curves. There are 4 input curves because they refer to the ground and the roof. \
First columns are created by division and interpolation of the side curves. \
Second beams are added. \
Thrid diagonals are added based on the user give points. Be aware that diagonals can be create in two directions.  \
Fourth, closed rectangles are created that represents roof and floor grid. \
The excel example is needed to measure the lengths of the beams, count them, specifiy units e.g. meters, and bake all the geometry to the appropriate layer in Rhino.

![image](https://user-images.githubusercontent.com/18013985/217834006-3ca7e29f-1b51-4a6c-9bda-c7b39739c64d.png)

