# Girasol
# Código de phyton 
# SOY FRANK
from turtle import*
import colorsys
speed(20)
bgcolor("black")
h=0
# dibujar tallo del girasol
penup()

goto(0,-100)
pendown()
color("green")
begin_fill()
rt(90)
fd(400)
lt(90)
fd(20)
lt(90)
fd(400)
lt(90)
fd(20)
end_fill()

#dibujar girasol
penup()

goto(0, 0)
pendown()
for i in range(16):
    for j in range(18):
        color("yellow") # todos los petalos son amarillos
        h += 0.005
        rt(90)
        circle(150-j*6,90)
        lt(90)      
        circle(150-j*6,90)
        rt(180)
    circle(40 , 24)
#colorear el centro de marron
penup()

goto(-20,0)
pendown()
color("brown")
begin_fill()
circle(44)#ajustar el radio del centro
end_fill()
done()
