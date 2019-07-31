This plugin takes one vector grid and two raster layers and produces a cell input file for the
agent based model inSALMO.  The produced files looks like so

Line 1
Line 2
Cell#,FracVelShelter,DistToHidingCover,FracSpawnGravel,ReachEndCode
1, 0.5, 9.625, 0, U
2, 0.581111111244, 8.06361110856, 0, U
3, 0.10000000149, 17.3249999713, 0, U
4, 0.5, 9.625, 0, I
5, 0.615, 7.41125, 0, I
6, 0.10000000149, 17.3249999713, 0, I
7, 0.5, 9.625, 0, I
8, 0.60700000003, 7.56524999943, 0, I
9, 0.154000001401, 16.285499973, 0, I

Instructions: 
The grid file should only have the attribute that is the single letter reach code for inSALMO.
The gravel file should only be a single band raster of the fraction of gravel cover.
The cover file should only be a single band raster of the fraction of cover.
The “Cover Conversion Factor” is: (Distance to hiding cover) = (1-(Fraction flow cover))(Cover conversion factor).
Press the "Output File" button and select a file location and name.
The program will append “.Data” to your file name.
Press "OK" to run. 