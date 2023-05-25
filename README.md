# Starcraft Rank Prediction

<img src="https://media.altchar.com/prod/images/940_530/gm-cc4c052e-e9e0-43a1-86ea-eda2c97a786d-13872.jpeg" width="8000" height="450" alt="Gameplay of Starcraft II from Blizzard">

## Welcome to the repository! 

The ultimate goal here is to use a dataset to predict a player's rank. I also want to use this README as a step-by-step journal of the process.

## Step 0: Setting up the project and work enviroment.

Early on, I had a few potential options for a workflow floating around in my head, but I decided to go with a Jupyter notebook in the end.
That way, I could easily document each step I make in the markdown sections. It is also one of the set-ups that I am most familiar with
which helped me get set-up faster.

<img width="1440" alt="Screen Shot 2023-05-25 at 1 19 00 AM" src="https://github.com/ddeneau/StarcraftRankPrediction/assets/58960615/1de566ef-a018-44e8-98c7-4ddb35cc0929">


So all the work from here on out takes place here. It was the first time I've used Python 3.11 for a data science project, so I had to install a couple of packages using pip.
Once this folder was set-up, I created this repository using it.

## Step 1: Making Sense of the Player Data CSV file.

Honestly, a couple of terms confused me in the data dictionary, such as PACs, or what exactly minimap attacks were. I'll define them here in case its unclear to anyone reading this in the future. 

PACs or Perception Action Cycles are the loops that begin when a player moves the viewport (the game world shown on their screen) to perform 1-to-5 actions, and end when they move the viewport again. Since the players screen only can show so much of the game level, or, playing field, at a time, I think of it as: "How much can a player get done in any given screen-sized area, before going to another area?"

Minimap attacks and right clicks are just actions that involve the player clicking on the minimap. For example, you could select a Marine on the screen, and click on a far-away point on the minimap to send them there, rather than moving the viewport manually over to that far-away point and clicking on it in the level itself. In other words, this can let the player save the time it takes to move the viewport around manually to move units greater distances.

The rest of the varialble names seem pretty self-explanatory.

<img width="394" alt="Screen Shot 2023-05-25 at 1 22 54 AM" src="https://github.com/ddeneau/StarcraftRankPrediction/assets/58960615/e5bac6b0-ce4b-477a-9ed7-cf511f0ccbdb">


