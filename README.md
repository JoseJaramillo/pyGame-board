# pyGame-board

Easy game created to test AI methods, the object of the game is take the key and go to the door.

Running in Python

pyGame library is needed to run, it can be installed via pip with the command:

'''
python3 -m pip install -U pygame
'''

## Goal

The agent goal is to go through the red door, to open the door it will need first to take the key.

Each time the game is restarted a new board of diferent dimensions with random
objects and agent position is generated, the score is set to zero.

### Rewards

- Each movement will have a penalty of 10.
- Steping into a cell with a nail on it will have a penalty of 100.
- Taking the Key will have a reward of 1000.
- Crossing the door with a Key will have a reward of 5000.

> Rewards can be easily changed in the 'def updateReward():' section

## Playability 

The agent can be controlled with the arrow keys, pressing the "Down" key will call the functions:

'''
agent.move("DOWN")    #Move the agent one cell down
refresh()             #Refresh the screen
updateReward()        #Update the score
'''

"r" key will restart the game
"x" key will close the window
