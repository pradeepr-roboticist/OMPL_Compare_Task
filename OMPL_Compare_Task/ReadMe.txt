1. This is the CNC Machine scene with 0.4 diameter rod. All solidworks file can be find in the CNC_Scene_0.4_CAD folder.
2. The start and goal configuartion can be found in the "Start_and_Goal_Config.txt". Odd row represents start config, even row represents goal config.
3. To run the simulation, first open the VREP scene, then run the python script named "main.py". The python program uses "numpy" plugin, please make sure your computer have installed the package.
4. It takes about 10-20 secs for the VREP OMPL to find appropriate path. To view the detail of algorithm timing, please refer to the excel sheet shared on the Google Drive.  



Lamy's Notes:
Problems in this program
1. After getting the map file's name(xxxx.stl), the python program does not send proper string to vrep. For example:
      in pyhton: inStrings = "map_clustered_2.stl"
      in Vrep: inStrings = "m","a","p".....
Question: How can we put those characters together in vrep? or sent the entire string as whole to vrep

2. Python error: "float" object is not subscriptable (line 97: inFloat = start[i] + goal [i])
