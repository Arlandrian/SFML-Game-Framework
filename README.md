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
</br>

<ul>
<li>C:\External Libs\SFML\include (change with your SFML Location) </li>
<li>%(ProjectDir)\</li>
<li>%(ProjectDir)\Source</li>
<li>%(ProjectDir)\res</li>
</ul>
</br>
*Linker -> General -> Additional Lib Dep -> add below lines
</br>
<ul>
<li>C:\External Libs\SFML\lib (change with your SFML Location) </li>
<li>%(ProjectDir)\</li>
<li>%(ProjectDir)\Source</li>
<li>%(ProjectDir)\res</li>
</ul>

*Select Release from left top corner and 
Linker -> Input -> Additional Dependencies - > Edit -> add below lines
</br>
<ul>
 <li>sfml-audio.lib</li>
 <li>sfml-graphics.lib</li>
 <li>sfml-window.lib</li>
 <li>sfml-network.lib</li>
 <li>sfml-system.lib</li>
</ul>
</br>
*Select Debug from left top corner 
Linker -> Input -> Additional Dependencies - > Edit -> add below lines
</br>
<ul>
 <li>sfml-audio-d.lib</li>
 <li>sfml-graphics-d.lib</li>
 <li>sfml-window-d.lib</li>
 <li>sfml-network-d.lib</li>
 <li>sfml-system-d.lib</li>
</ul>
</br>
copy /bin content to exe location from SFML folder

Copy res, Source folder to project location

From Solution Explorer enable "Show All Files"
include source and res folder

start coding...
 
