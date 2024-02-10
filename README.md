import turtle

def dibujar_tallo():
    turtle.color("green")
    turtle.penup()
    turtle.goto(0, -200)
    turtle.pendown()
    turtle.right(90)
    turtle.forward(200)

def dibujar_petalo():
    turtle.color("red")
    turtle.begin_fill()
    turtle.circle(100, 60)
    turtle.left(120)
    turtle.circle(100, 60)
    turtle.left(120)
    turtle.end_fill()

def dibujar_tulipan():
    dibujar_tallo()
    for _ in range(6):
        dibujar_petalo()
        turtle.right(60)

def main():
    turtle.speed(0)
    dibujar_tulipan()
    turtle.hideturtle()
    turtle.done()

if __name__ == "__main__":
    main()
