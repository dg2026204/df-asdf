snow_body = sphere(pos=vec(0, 0, 0), axis=vec(3, 0, 0), radius=3, color=color.white)
snow_eye = sphere(pos=vec(-1.4,0.6, 2.5), axis=vec(1.5, 0, 0), radius=0.15, color=color.black)
snow_eyes = sphere(pos=vec(1.4, 0.6, 2.5), axis=vec(1.5, 0, 0), radius=0.15, color=color.black)
snow_mouse = ring (pos=vec(0, -1,2.8), radius=0.4, color=color.black, axis=vec(0,0,1))

snow = compound([snow_body, snow_eye, snow_mouse, snow_eyes])
b = box (pos = vec(-10,0,0), size = vec(2.5, 2.5, 2.5), texture = "https://i.postimg.cc/BvZcJpCw/images.jpg")
c = box (pos = vec(-15,0,0), size = vec(2.5, 2.5, 2.5), texture = "https://i.postimg.cc/BvZcJpCw/images.jpg")
d = box (pos = vec(-20,0,0), size = vec(2.5, 2.5, 2.5), texture = "https://i.postimg.cc/BvZcJpCw/images.jpg")
e = box (pos = vec(-25,0,0), size = vec(2.5, 2.5, 2.5), texture = "https://i.postimg.cc/BvZcJpCw/images.jpg")


while True :
    rate(100)
    k = keysdown()
    if 'a' in k :
        snow.pos.x = snow.pos.x - 0.1
    if 'd' in k :
        snow.pos.x += 0.1
    if mag(b.pos - snow.pos) < 3 : 
        b.opacity = 0
    if mag(c.pos - snow.pos) < 3 : 
        c.opacity = 0
    if mag(d.pos - snow.pos) < 3 : 
        d.opacity = 0
    if mag(e.pos - snow.pos) < 3 : 
        e.opacity = 0
