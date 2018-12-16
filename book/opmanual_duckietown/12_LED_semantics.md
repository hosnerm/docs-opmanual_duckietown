# Semantics of LEDS {#LED-semantics status=draft}

Assigned: ???

Since different implementations could mean different semantic mappings, a versioning is kept here to maintain overview.

## master18

This is the semantics assumed by the algorithms implemented in `master18`


Headlights: white, constant

### Traffic light

"go" = green(5s) + orange(3s) **XX Hz square wave**
"stop" = red, **constant**  

### Duckiebot
(F) Stands for front LEDs

"CAR_SIGNAL_SACRIFICE_FOR_PRIORITY" = white, **1.9 Hz square wave** (F)
"CAR_SIGNAL_A" = white, **4 Hz square wave** (F)
"CAR_SIGNAL_GREEN" = green, **5.7 Hz square wave** (F)
"CAR_SIGNAL_PRIORITY" = purple, **5.7 Hz square wave** (F)





## master17
headlights: white, constant

Assumption:

- **20 fps** to do LED detection

- 1s to decide

- 3 frequencies to detect


tail lights: red, **6 hz square wave**

traffic light "GO" = green, 1 hz** square wave**

traffic light "STOP" = red, 1.5 Hz** square wave**

duckie light on top, state 0 = off

duckie light on top, state 1 = blue, **3 Hz, square wave**

duckie light on top, state 2 = ?, **2.5 Hz square wave**

duckie light on top, state 3 = ?,** ****2 Hz square wave**
