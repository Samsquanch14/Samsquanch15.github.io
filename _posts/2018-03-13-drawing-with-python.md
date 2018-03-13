---
layout: post
title: Drawing with Python
description: The is a python code that draws a cool star!
---
description
import turtle, random  #importing turtle to draw and random for random colors.
a=turtle.Turtle()

colors  = ["red","green","blue","orange","purple","pink","yellow",] # a list of colors to randomly be chosen from

def Octastar(a_turtle, size):
  a_turtle.width(10) # pen width for turtle
  a_turtle.speed(8) # the speed the turtle goes (0-10)
  length = 5 # length of line created by turtle move function
  for count in range(size):
    color = random.choice(colors) #Chooses a random color
    a_turtle.forward(length)
    a_turtle.right(135)
    a_turtle.color(color) # Changes turtle color to the random color chosen by the computer
    length = length + 5 # Gradually increases size if the line created by turtle
    
def Triangle(a_turtle, dist_forward):
  color = random.choice(colors)
  a_turtle.color(color)
  a_turtle.width(5)
  a_turtle.speed(5)
  length = 5
  for loop in range(3):
    a_turtle.forward(dist_forward)
    a_turtle.left(120)
  

Octastar(a, 150)
