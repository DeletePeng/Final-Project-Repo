`import random
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
main()`