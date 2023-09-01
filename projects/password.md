---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "Password Matching"
date: 2015
published: true
labels:
  - Java
  - Programing
  - Security
summary: "As part of my first proyect in ICS 111 we created a simple password check code."
---



Micromouse is an event where small robot “mice” solve a 16 x 16 maze.  Events are held worldwide.  The maze is made up of a 16 by 16 gird of cells, each 180 mm square with walls 50 mm high.  The mice are completely autonomous robots that must find their way from a predetermined starting position to the central area of the maze unaided.  The mouse will need to keep track of where it is, discover walls as it explores, map out the maze and detect when it has reached the center.  having reached the center, the mouse will typically perform additional searches of the maze until it has found the most optimal route from the start to the center.  Once the most optimal route has been determined, the mouse will run that route in the shortest possible time.

For this project, I was the lead programmer who was responsible for programming the various capabilities of the mouse.  I started by programming the basics, such as sensor polling and motor actuation using interrupts.  From there, I then programmed the basic PD controls for the motors of the mouse.  The PD control the drive so that the mouse would stay centered while traversing the maze and keep the mouse driving straight.  I also programmed basic algorithms used to solve the maze such as a right wall hugger and a left wall hugger algorithm.  From there I worked on a flood-fill algorithm to help the mouse track where it is in the maze, and to map the route it takes.  We finished with the fastest mouse who finished the maze within our college.

Here is some code that illustrates how we read values from the line sensors:

```cpp
public static boolean userPasswordMatch(String user , String pass) {
String user1 ="alpha";
String user2 ="beta";
String user3 ="gamma";
String user4 ="delta";
String pass1 ="alpha1";
String pass2 ="beta1";
String pass3 ="gamma1";
String pass4 ="delta1";

 
    if (((user.equals(user1) && pass.equals(pass1)
    ||user.equals(user2)&& pass.equals(pass2)
               || user.equals(user3)&& pass.equals(pass3)
                  || user.equals(user4) && pass.equals(pass4)))){
   
  return true;
      }
   
return false;
}

```
