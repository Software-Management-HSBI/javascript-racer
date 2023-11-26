# Variables:


## segments[] (l.91):
speichert die fahrstrecke
initalisiert in l. 209 resetRoad()
    * p1 + p2: koordinaten eines segemtns in realtion zur welt, kamera, und screen
    * color
    * looped?
    später auch:
        * curve: signed integer
        * sprites: array, objekte am fahrbahn rand
        * cars: autos. position, geschwindigkeit, precent?
        * clip?
        * fog, wie viel nebel halt, muss lokal bleiben

## sprites[] (l. 96):
initalisierung in commmon.js
speichert größen von objekten autos und andere

## plyerX, plyerZ (ll. 107):
position des spielers

## speed (l. 111)

## position(l. 110):
z koordinate der kamera

# Methoden:

## update()
* updateCars()
* 
* aktualisiert psition und geschwindigkeit nach keyinputs
* kollisionen mit objekten werden erkannt
* kollision mit autos werden erkannt
* max speed und entfernung von bahn werden begrenzt
* hintergrund wird aktualisiert
* überprüfen ob eine runde gefahren wurde und HUD aktualisieren
    * if(position > playerZ) ??
* HUD generell aktualisieren

## updateCars()
* updateCarOffset()
* speed wird aktualisiert

## updateCarOffset()
akatualisiert die seitliche Position des Autos
sorgt wohl dafür dass es anderen ausweicht