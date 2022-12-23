# Computer-Engineering---Assignment-15
def on_on_chat():

    mobs.spawn(PIG, pos(0, 0, 0))
    
player.on_chat("pig", on_on_chat)

def on_on_chat2():

    mobs.spawn(COW, pos(0, 0, 0))
    
player.on_chat("cow", on_on_chat2)

def on_on_chat3():

    blocks.fill(AIR, pos(-5, -5, -5), pos(5, 5, 5), FillOperation.REPLACE)
    
player.on_chat("dig", on_on_chat3)

def on_on_chat4():

    player.teleport(pos(0, 100, 0))
    
player.on_chat("jump", on_on_chat4)

def on_on_chat5():

    blocks.fill(POPPY, pos(-1, 0, -1), pos(1, 0, 1), FillOperation.DESTROY)
    
player.on_chat("flower", on_on_chat5)

def on_travelled_fly():

    blocks.place(GRASS, pos(0, 0, 0))
    
player.on_travelled(FLY, on_travelled_fly)

def on_on_chat6():

    mobs.spawn(CHICKEN, pos(0, 0, 0))
    
player.on_chat("chicken", on_on_chat6)

def on_on_chat7():

    gameplay.set_weather(CLEAR)
    
player.on_chat("weather clear", on_on_chat7)
