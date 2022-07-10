# MapperPublic
**_Source Code Available upon Demand_**\
**Authors:**
- Dante Crescenzi \
**Contact Info:** \
https://github.com/dcrescenzi \
https://www.linkedin.com/in/dante-crescenzi/ \
dantecrescenzi@gmail.com
- Hannah Ghassabeh \
**Contact Info:**\
https://github.com/HannahGhassabyte \
https://www.linkedin.com/in/hannah-ghassabeh-92200b204/ \
hannah.ghassabeh@mail.utoronto.ca
- And Myself

## Video Demo of the Different Features

https://user-images.githubusercontent.com/70533174/178164228-366ce57b-8687-4dfe-a4c4-df10a1aaebea.mp4

\
**NOTE:** Due to GitHub README files not allowing videos over 10 Megabytes, I had to compress the video. For the full quality video you can see it here:\
https://www.youtube.com/watch?v=5GGsZbrTWwo&ab_channel=DanielLiu \

## How this project was divided
**-** This project was divided into four milestones throughout the course of four months. <br /><br />
**1.** The first milestone included organizing large amounts of data into data structures and extending and making further use of an existing API by implementing useful functions for later milestones.<br /><br />
**2.** The second milestone utilized a graphics library called EZGL which was really a wrapper around the GTK library. It depends on GTK 3 and Cairo. Full details here: https://github.com/mariobadr/ezgl . The objective of this milestone was to essentially draw the map using this library along with the functions implemented back in the first milestone. <br /><br />
**3.** The third milestone had an objective of implementing pathfinding between two intersection points that are in the graph that represents the map. This milestone also included the design and creation of directions that go along with the path found.<br /><br />
**4.** The last and final milestone had an objective of finding a path with multiple stops. More specifically, finding a valid path for multiple deliveries and dropoffs. An example would be: if we have four pickups labeled pickup A, B, C, D and four dropoffs labeled dropoff A, B, C, D. What is the shortest possible path such that by the time we reach dropoff C we have the package from pickup C? On top of this, the delivery driver has to start at a depot and end at a depot. 

## What I learned from this project 
There were many things that I tookaway from this project. I have included the main points into a list below:
* Proper git hygiene. This included frequent commits, meaningful commit messages, working on a branch and merging, frequent pulling, and communication with teammates
* The organization and design of software. An example of this would be the organization of different data types into their respective structs, the merging of code that performed different things.
* Efficiency of certain data structures over others. For example, the usage of a hashmap for large amounts of unordered data and quick access/insertion.
* Optimization & efficiency of code. This included preprocessing what can be preprocessed into data structures, clever implementations of algorithms, heuristics
* The leverage of a graphics library to draw the actual data in the graph.  
* Dijkstras algorithm and then a further extension of it using the A* algorithm.
* A look at heuristics used to solve a computational hard problem similar to travelling salesman. 

## What I would do differently if I were to restart this project.
Reflecting back on the project, there are certain aspects in the project that I would have redesigned. These things are listed below:
* This project was developed entirely in C++. I would have liked to leverage the object oriented programming aspects of C++ more than I did. The source code utilized structs in a way that was similar to structs seen in C. Looking back, leveraging the usage of methods in classes along with inheiritance to reuse methods would have made the source code much more refined and cleaner. 
* Multi-thread more aspects of the code where it was possible. 

## What I would refine in the existing code if I had more time
This is more so a reflection on what I would have liked to further refine on the already existing source code. 
* Less usage of global variables. Although we were very careful with modifying globals across files, global variables should still be avoided when they can be. This would be something that I would not use as freely as I did if I were to redesign the project.
* A brush up on style would be something that I would refine if I had more time. The overall style was pretty good and never received any complaints. However, I do think more detailed & higher level comments could have been included for certain parts of the code to make everything more readable.
* A deep dive into how to make the user experience of dragging around the map much smoother. This would require optimization of the code used to draw the map.

## What Extra Features would I have included if I had more time
This section is dedicated to what extra features I would have included if I had more time.
* Live traffic data. The current map's pathfinding assumes that there is no traffic. I would have included live traffic data from external libraries and included this calucation into the shortest possible path in our map
* Pathfinding for addresses. Currently our map only pathfinds between intersections. If I had more time I would have liked to look into the parsing of data that included addresses and develop the option to pathfind between addresses as well.
* Interactive GPS directions. Currently our map utilized directions that pop up on the screen but there is no audio that goes with it. An implementation of audio that reads out the directions and tracks your location similar to that of a GPS would have been an amaizng additional feature.
* A webapp that used the mapper. Currently our map is launched from the terminal but it is unable to be accessed through the web. Integrating our map into a web app would have taken lots of time but it would have been something I would be interested in doing if I had more time.
