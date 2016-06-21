# Overview
A tower defense game inspired by PopCap Games' Plants Vs. Zombies. This project appl paradigms of functional and object-oriented programming. This project also involves understanding, extending, and testing a large program.

# Characters

* The Colony. The colony consists of several places that are chained together. The exit of each Place leads to another Place.
* Placing Ants. There are two constraints that limit ant production. Placing an ant uses up some amount of the colony's food, a different amount for each type of ant. Also, only one ant can occupy each Place.
* Bees. When it is time to act, a bee either moves to the exit of its current Place if no ant blocks its path, or stings an ant that blocks its path.
* Ants. Each type of ant takes a different action and requires a different amount of food to place. The two most basic ant types are the HarvesterAnt, which adds one food to the colony during each turn, and the ThrowerAnt, which throws a leaf at a bee each turn.

# Instructions

## Game Rules

Each turn, new bees may enter the ant colony. Then, new ants are placed. Finally, all insects (ants, then bees) take individual actions: bees sting ants, and ants throw leaves at bees. The game ends either when a bee reaches the ant queen (you lose), or the entire bee flotilla has been vanquished (you win).

## To start Ants Vs. SomeBees
On Terminal:
```
$ python3 ants_gui.py -f
```

Optional arguments:
```
$ python3 hog_gui.py -w            loads a full layout with water
$ python3 hog_gui.py -i            loads a difficult assault plan
$ python3 hog_gui.py --food FOOD   number of food to start with
```