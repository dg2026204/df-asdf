snow_body = sphere(pos=vec(0, 0, 0), axis=vec(3, 0, 0), radius=5, color=color.white)
snow_eye = sphere(pos=vec(-3,0.78, 4), axis=vec(1.5, 0, 0), radius=0.35, color=color.black)
snow_eyes = sphere(pos=vec(3, 0.78, 4), axis=vec(1.5, 0, 0), radius=0.35, color=color.black)
snow_mouse = ring (pos=vec(0, -1.5, 4.7), radius=0.8, color=color.black, axis=vec(0,0,1))

snow = compound([snow_body, snow_eye, snow_mouse, snow_eyes])

while True :
    rate(100)
    k = keysdown()
    if 'a' in k :
        snow.pos.x = snow.pos.x - 0.1
    if 'd' in k :
        snow.pos.x += 0.1
    


box (pos = vec(5,5,5), size = vec(5,5,5), texture = "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTDYUfuP5567tftgFEyAbhtNg_UACgpBviH2HLep20PQw&s=10")
# df-asdf
