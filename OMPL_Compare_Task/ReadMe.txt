Lamy's Notes:
Problems in this program
1. After getting the map file's name(xxxx.stl), the python program does not send proper string to vrep. For example:
      in pyhton: inStrings = "map_clustered_2.stl"
      in Vrep: inStrings = "m","a","p".....
Question: How can we put those characters together in vrep? or sent the entire string as whole to vrep

2. Python error: "float" object is not subscriptable (line 97: inFloat = start[i] + goal [i])
