```
import random
from turtle import Turtle

def cool_image(turtle,angle,length):
    colors = ["blue", "green", "red", "yellow","orange","violet", "indigo" ]
    color = (random.choice(colors))
    turtle.color(color)
    turtle.right(20)
    turtle.left(40)
    turtle.backward(angle)
    turtle.forward(length)
    length = length - 1
    angle = 70 + length
    if (length > 1):
        cool_image(turtle,angle,length)
       


def main():
    ANIMATION_SPEED = 0
    epic = Turtle()
    epic.speed(ANIMATION_SPEED)
    cool_image(epic,30,150)
main()
```
This is a neat turtle image which I made for another one of my classes. Run it in python, and check it out! It's quite cool.

Oh, and here is my resume if you're interested.
[My resume](resume.pdf)
