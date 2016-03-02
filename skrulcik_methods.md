
# 15294 Final Project

Author: Scott Krulcik
AndrewID: skrulcik
Project Name: Colosseum


## Methods

I used to do modelling in Autodesk Inventor for my high school robotics team, so I am a little bit more comfortable with that than SolidWorks, but they are mostly equivalent. That choice caused some STL export issues, but they were eventually resolved.

The primary feature I used to accomplish my goals was the revolve and circular pattern tools. Originally, I used parameters to define what fraction of the circle my detailed pi wedge would represent, and used that to calculate angles and pattern parameters. Once the project got more intricate, I was no longer able to change the parameters because there were too many dependencies between features.


## Autodesk Export Problems

The first day I tried printing, I had three prints fail. Originally these failures were attributed to the quality of the Cube's, but Autodesk was at least partially at fault. After the failures, an ideate staffer recommended I check my STL file, becaues sometimes bad STL files would make the prints fail. At first I thought this couldn't be the problem, because the STL rendered fine on Github (where I was doing version control) and Cube's own print software. But using Meshlab I determined some of the normals were messed up. Upon further research, I discovered this is a somewhat common problem when exporting revolved parts from Autodesk Inventor (See links at the bottom of the page) despite the fact that the STL export utility is specifically meant for 3D printing.

Using the forum posts as a guide, I kept tweaking STL export settings, such as surface and normal deviation (which I still don't quite understand). Eventually, I was able to get a low resolution STL ASCII file out of Autodesk that appeared satisfactory in meshlab. The cube was able to properly interpret this file and at last the print succeeded.


## Test Print

It may also be worth noting that I tested a small wedge, with no details, to make sure the arch structure would print properly because Professor Touretzky mentioned it may not hold itself up.


## Links

### Colosseum Information

  - [Spanish Website with good Cross Section](http://www.the-colosseum.net/images/sezione.jpg)
  - [General Information](https://en.wikipedia.org/wiki/Colosseum)

### Autodesk STL Export

  - [Forum Post 1](https://forums.autodesk.com/t5/inventor-general-discussion/stl-output-bad-high-resolution/td-p/1818994)
  - [Forum Post 1 (page 2)](https://forums.autodesk.com/t5/inventor-general-discussion/inventor-generating-bad-stl-mesh/m-p/4824733#M497942) - These reponses were the most useful, because they offered some troubleshooting tips.
  - [Forum Post 2](https://forums.autodesk.com/t5/inventor-general-discussion/inventor-generating-bad-stl-mesh/td-p/4819845)





