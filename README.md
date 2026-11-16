snow_body = sphere(pos=vec(0, 0, 0), axis=vec(3, 0, 0), radius=3, color=color.white)
snow_eye = sphere(pos=vec(-1.4,0.6, 2.5), axis=vec(1.5, 0, 0), radius=0.15, color=color.black)
snow_eyes = sphere(pos=vec(1.4, 0.6, 2.5), axis=vec(1.5, 0, 0), radius=0.15, color=color.black)
snow_mouse = ring (pos=vec(0, -1,2.8), radius=0.4, color=color.black, axis=vec(0,0,1))

snow = compound([snow_body, snow_eye, snow_mouse, snow_eyes])
b = box (pos = vec(-10,0,0), size = vec(2.5, 2.5, 2.5), texture = "https://www.shutterstock.com/image-vector/star-pixel-v2-world-cuteness-260nw-2365872663.jpg")
c = box (pos = vec(-15,0,0), size = vec(2.5, 2.5, 2.5), texture = "https://www.shutterstock.com/image-vector/star-pixel-v2-world-cuteness-260nw-2365872663.jpg")
d = box (pos = vec(-20,0,0), size = vec(2.5, 2.5, 2.5), texture = "https://www.shutterstock.com/image-vector/star-pixel-v2-world-cuteness-260nw-2365872663.jpg")
e = box (pos = vec(-25,0,0), size = vec(2.5, 2.5, 2.5), texture = "https://www.shutterstock.com/image-vector/star-pixel-v2-world-cuteness-260nw-2365872663.jpg")
f = box (pos = vec(-30,0,0), size = vec(2.5, 2.5, 2.5), texture = "https://www.shutterstock.com/image-vector/star-pixel-v2-world-cuteness-260nw-2365872663.jpg")
g = box (pos = vec(-30,-5,0), size = vec(2.5, 2.5, 2.5), texture = "https://www.shutterstock.com/image-vector/star-pixel-v2-world-cuteness-260nw-2365872663.jpg")
h = box (pos = vec(-25,-5,0), size = vec(2.5, 2.5, 2.5), texture = "https://www.shutterstock.com/image-vector/star-pixel-v2-world-cuteness-260nw-2365872663.jpg")
i = box (pos = vec(-20,-5,0), size = vec(2.5, 2.5, 2.5), texture = "https://www.shutterstock.com/image-vector/star-pixel-v2-world-cuteness-260nw-2365872663.jpg")
j = box (pos = vec(-15,-5,0), size = vec(2.5, 2.5, 2.5), texture = "https://www.shutterstock.com/image-vector/star-pixel-v2-world-cuteness-260nw-2365872663.jpg")
kk = box (pos = vec(-10,-5,0), size = vec(2.5, 2.5, 2.5), texture = "https://www.shutterstock.com/image-vector/star-pixel-v2-world-cuteness-260nw-2365872663.jpg")



while True :
    rate(100)
    k = keysdown()
    if 'a' in k :
        snow.pos.x = snow.pos.x - 0.1
    if 'd' in k :
        snow.pos.x += 0.1
    if 's' in k :
        snow.pos.y -= 0.1
    if mag(b.pos - snow.pos) < 3 : 
        b.opacity = 0
    if mag(c.pos - snow.pos) < 3 : 
        c.opacity = 0
    if mag(d.pos - snow.pos) < 3 : 
        d.opacity = 0
    if mag(e.pos - snow.pos) < 3 : 
        e.opacity = 0
    if mag(f.pos - snow.pos) < 3 : 
        f.opacity = 0    
    if mag(g.pos - snow.pos) < 3 : 
        g.opacity = 0
    if mag(h.pos - snow.pos) < 3 : 
        h.opacity = 0
    if mag(i.pos - snow.pos) < 3 : 
        i.opacity = 0
    if mag(j.pos - snow.pos) < 3 : 
        j.opacity = 0
    if mag(kk.pos - snow.pos) < 3 : 
        kk.opacity = 0
