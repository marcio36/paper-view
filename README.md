
import turtle as t
import random
screen = t.Turtle()

t.bgcolor('black')
t.speed(0)

color_code = ['#00ff00', '#6100ff', '#c4a0ff', '#05fffa',
              '#37ff00', '#c9ffba', '#ff00e5', '#eeff00',
              '#eeff00', '#979e3f', '#4ee0d4', '#8b56a5',
              '#b480ba', '#e5398f', '#ed6aab', '#8b56a5',
              '#37f7ac', '#c1f2df', '#ffb600', '#edcd7d',
              '#cd7ded', '#9927aa', '#54db3f', '#00ff11',
              '#667d8c', '#16ad7d', '#6bdbb7', '#d9ace0']

n = 0
j = 0
t.hideturtle()

for i in range(80):
    c = random.choice(color_code)
    t.pencolor(c)
    t.forward(2+n)
    n += 1
    t.left(45)
    t.backward(2+n)
    n += 1
    t.right(90)
    print(i)

t.done()
