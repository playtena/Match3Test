# Match 3 game short description

## Project overview
Implement collapse match 3 game. 
Example: ToyBlast, ToonBlast (AppStore, PlayStore), PandaJam (Facebook game)

### Objective
Implement collapse game with basic gameplay functionality.
Game should be implemented using Unity game engine.

### Game description

#### UI
There are two screens in the game. Intro screen and gameplay screen.
On Intro screen there is a "Start" button on clicking which Gameplay screen is opened.
On Gameplay screen game board is drawn with color figure items.

#### Gameplay short description
When user clicks on the items game is looking for same color matches and if there is any same color group size >= 2 that group is cleared and items are dropping down.

Game has objective. That is to collect some ammount of color figures items. Ex, 10 red, 20 orange.
User has predefined moves count using which he has to fullfil the objective. Every successfull tap is counted as a move.
Game is considered as won if player manages to fullfil the objective before he runs out of moves. If the moves are finished before fullfiling the objective game is lost.

If player wins the game 'You won' popup is shown with "Play Again" button on it.
If he loses 'You loose' popup is shown with "Play Again" button on it.

When 'Play Again' button is pressed game is restarted.

#### Boosters
There are power ups in game.
##### Line Bomb
If player taps onf a color group which size is 5 some special item called "lineBomb-Horizontal" or "lineBomb-Vertical" booster is generated.
Line Bomb clears whole row or column depending on its type.

##### Radial Bomb
If the cleared group size is 6 than "Radial Bomb" booster is generated.
Radial Bomb clears all it's neighbours.

Boosters are activated when tapped.

 For more details check example games listed above.

### Visual requirements
The only required visual effect is to implement figures dropping animation. All other graphical part can be kept maximal simple.
##### Note: Implementation should not be based on any 2D Physics.

### Game Configuration
There are some values that should be possible to configure in Unity Edtior before starting the game.
1. Board row/column size. (min 7, max 10)
2. Moves count.
3. Objectives count (max 3) their colors and values. i.e. 10 red, 12 orange, 20 blue.
4. Figures colors count. (min 4, max 7)

![alt text](https://github.com/plexonic/Match3Test/blob/master/Resources/toy-blast_info.png)
