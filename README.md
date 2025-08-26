# 🐍 Day 19 - Part 1: Etch-A-Sketch with Turtle 🎨

Welcome to **Day 19 (Part 1)** of my **Python Bootcamp Journey** 🚀  
In this project, I created a fun **Etch-A-Sketch game** using Python's **turtle module** 🐢.  
This is a simple interactive program where you can control a turtle with your keyboard to draw cool shapes and patterns!

---

## 📜 Code Explanation  

### ✨ Importing the Modules
```python
from turtle import Turtle, Screen
```
- `Turtle` 🐢 → The main character that moves around the screen.
- `Screen` 🖥️ → The canvas where the turtle moves.
---
### 🐢 Turtle Setup
```python
tim = Turtle()
```
- Creates a turtle named **tim** who will be drawing on the screen.
---
### 🎮 Movement Functions
```python
def move_forward():
    tim.forward(10)

def move_backward():
    tim.backward(10)

def turn_left():
    tim.left(10)

def turn_right():
    tim.right(10)
```
- **W** → Move forward ⬆️
- **S** → Move backward ⬇️
- **A** → Turn left ↩️
- **D** → Turn right ↪️  
These functions let you control **tim** like a tiny turtle car! 🐢🚗
---
### 🧹 Clearing the Screen
```python
def clear_screen():
    tim.clear()
    tim.penup()
    tim.home()
    tim.pendown()
```
- **C** → Clears the screen 🧽
- Sends **tim** back to the center 🏠 and resets his path.
---
### ⌨️ Listening for Keys
```python
screen = Screen()
screen.listen()
screen.onkey(move_forward,key="w")
screen.onkey(move_backward,key="s")
screen.onkey(turn_left,key="a")
screen.onkey(turn_right,key="d")
screen.onkey(clear_screen,key="c")
```
- The program **listens** 👂 for key presses.
- Each key (`w`, `s`, `a`, `d`, `c`) is bound to a turtle action.
---
### 🖱️ Exit on Click
```python
screen.exitonclick()
```
- Closes the program when you click on the screen ❌🖱️
---
## 🎯 What I Learned
- How to use the **turtle module** 🐢
- How to set up **keyboard event listeners** ⌨️
- How to reset the turtle’s position and clear the canvas.
--- 