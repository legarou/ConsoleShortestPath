# ConsoleShortestPath

When using the console application, the follwoing actions are possible:
  - READ
 
    Read the building into the program from a prepared file. One building, the FH Technikum Wien, has already been prepared in the "building.txt" file.  
 
    To use your own building, the building has to prepared in either a txt or csv file.  
     The first line is ignored. Each line should contain one point of the building with:  
       - name (muste be unique, as it serves as the node’s id)  
       - node type (door, room, stairs, elevator, or path),  
       - leads outside value (true or false)   
       - a list of all neighbors and their distances to the node  
 
    The list of neighbors consists of the name, which is the id of the node, and a number representing the distance from the neighboring node to the current node.  
     These four properties are separated by a semicolon.   
     The first two lines of the building file might look like this:  
     
        name;type;leads outside;neigbours (name + distance)
        A0.03 Treppe;STAIRS;FALSE;A0.03 Seitenausgang,3,A0.03 Haupteingang,13,A0.15 Lift,21

 - PRINT
 
    prints a list of all nodes in the building
 - PROFILE
 
    sets up the profile
    
-  ALGORITHM
 
    sets only the algorithm preference in the profile
    
-  PATH
 
    Call the shortest path program. You will have to enter the start and end point (must be exact and exist in teh building structure).  
    You can choose between using your own profile or setting up a new one. Your profile preferences will not be changed.
  
-  QUIT
 
    Quit the program.
