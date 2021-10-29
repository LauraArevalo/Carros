x = 500
y = 300

def setup():
    size (x,y)
    
class Carro :
    def __init__ (self):
        self.c = color(255)
        self.posX = 100
        self.posY = 100
        self.posA = 140
        self.posB = 140
        self.posC = 200
        self.posD = 200
        self.velE = 2
        self.velX = 1
        self.velF = 3

miCarro = Carro()

def draw():
    background(200)
    fill (200,255,150,80)
    stroke(120)
    rect (miCarro.posX,miCarro.posY,30,30)
    miCarro.posX = miCarro.posX + miCarro.velX
    if miCarro.posX > 500:
        miCarro.posX = 0
        
    fill (180,100,90,50)
    stroke(120)
    rect (miCarro.posA,miCarro.posB,30,30)
    miCarro.posA = miCarro.posA + miCarro.velE
    if miCarro.posA > 500:
        miCarro.posA = 0
        
    fill (20,120,80,40)
    stroke(120)
    rect (miCarro.posC,miCarro.posD,30,30)
    miCarro.posC = miCarro.posC + miCarro.velF
    if miCarro.posC > 500:
        miCarro.posC = 0
