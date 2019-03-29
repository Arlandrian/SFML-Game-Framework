# SFML-Game-Framework
Simple framework for SFML games and that


Requires C++14 and SFML 2.4.1

Nothing special.

Features:

* State/Screen system

This is a system that allows you to organise different stages of the game. In other engines and frameworks, you may have seen this named as "Scene", "Stage", or "Room".

* Cruddy GUI system

* Animation

* Some maths

* file stuff

* resource manager

# Visual Studio Setup

Create an empty visual studio project

Add a .cpp file (Just add it)

Project -> Properties

C/C++ -> Additional Innclude Directories -> add below lines

C:\External Libs\SFML\include (change with your SFML Location)
%(ProjectDir)
%(ProjectDir)\Source
%(ProjectDir)\res


Linker -> General -> Additional Lib Dep -> add below lines

C:\External Libs\SFML\lib  (change with your SFML Location)
%(ProjectDir)
%(ProjectDir)\Source
%(ProjectDir)\res

Select Release from left top corner and 
Linker -> Input -> Additional Dependencies - > Edit -> add below lines


sfml-audio.lib
sfml-graphics.lib
sfml-window.lib
sfml-network.lib
sfml-system.lib

Select Debug from left top corner
add below lines
sfml-audio-d.lib
sfml-graphics-d.lib
sfml-window-d.lib
sfml-network-d.lib
sfml-system-d.lib

copy /bin content to exe location from SFML folder

Copy res, Source folder to project location

From Solution Explorer enable "Show All Files"
include source and res folder

start coding...
 
