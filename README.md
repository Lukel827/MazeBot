# MazeBot
# Vincent flum the IP seeker
# This one hugs the wall
from BirdBrain import Finch
myFinch = Finch()


while True:
    if myFinch.getDistance() > 35:
        myFinch.setMove('F',31,50)
    else:
        myFinch.setTurn('L',92,100)
        if myFinch.getDistance() < 35:
            myFinch.setTurn('R',186,100)



# Node seach still work in progress 
"""
from BirdBrain import Finch
myFinch = Finch()
nodes = []
directions = {0:-90,1:0,2:90}

def move():
    myFinch.setMove('F',31.5,50)

def turn(degrees):
    myFinch.setTurn('R',degrees,1000)


class Node:
    
    def __init__(self, surroundings):
        self._surroundings = surroundings

    def pick_direction():
        for i in range(3):
            if surroundings[i]:
                surroundings[i] = False
                return directions[i]
        return 


def collect_surroundings():
    turn(-90)
    surroundings = []
    for i in range(3):
        surroundings.append(myFinch.getDistance() < 20)
        turn(90)
    turn(180)
    return surroundings


while len(surroundings := collect_surroundings) < 4:
    nodes.append(Node(surroundings))
    turn(nodes[-1].pick_direction())
    move()
    
    
myFinch.stopAll()
"""




