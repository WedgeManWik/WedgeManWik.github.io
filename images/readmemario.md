# Mario Bros Arcade - My take on it.

Recreating Mario Bros Arcade using C++ and SDL2 library.

![My Mario Game](https://github.com/WedgeManWik/MarioBaseProject/blob/main/MarioBaseProject/MarioBaseProject/Images/MarioImage.png?raw=true)

I didn't want to exactly re-create the original game, instead I felt like adding my own twists and turns would be more fun.

## Game Description 

### Playing the game

#### Some basic rules

There are three levels in each game, with each level having three waves of enemies. Each level has a different level map, with different tile positions, potential coin positions, and different POW block positions. On each level, the player’s respawn location will change.

In each game, the players start off with three lives, once a life is lost, there is no way to earn it back. The coin positions are completely randomised, but there are always exactly 20 coins on each level. To move onto the next level, the player must kill all enemies on the map. When collecting a coin, the player will receive 100 points.


There are two enemy types: Koopas and Goombas. 
On the first wave of a level, four Koopas will spawn. On the next levels, two Koopas and two Goombas will spawn. The only way to remove the enemies is to kill them, if a player doesn’t kill them, they’ll stay for ever!

**Koopas:** These guys walk left/ right and switch their direction after colliding with the edge of the map, or when flipping back up after being knocked over. When a player hits a POW block, the screen will shake and all Koopas on the map will be knocked over into their shell; in this state, the player can collect the Koopa shell. If the player collects a Koopa shell or kills it by jumping onto its back – the player will receive 200 points. Koopas can be knocked onto their shell either by shaking the screen from a POW block or hitting the ceiling of the tile map directly below the Koopa.

**Goombas:** The only way to kill Goombas is to squash them by jumping onto them! POW blocks don’t scare Goombas and hitting the map tile beneath them doesn’t rock them one bit! The player can only kill a Goomba by squashing it. However, because of this – the player is rewarded with a nice 300 points.

#### Player Info & Controls

The player can move around the map by using the “W”, “A” and “D” keys for Luigi, or arrow keys for Mario, excluding the down arrow. Pressing the “W” or up arrow will make the player jump. 

When jumping, if the player hits their head on the ceiling of a tile, it will cancel their jump and knock over any Koopas standing on that tile. If the player is directly below a POW block and hits it, it will use the POW block. 

When running, if the player lets go of their keys, the player will do a small sliding animation and carry on going in the same direction for a small moment. The Player can not go outside of the map.

Once a player dies and loses a life, they will respawn to the same location they first were spawned in on the map. On each level, the player’s respawn location will change. Once a player loses all of their lives, they will not respawn again in that game. If their score is high enough, they may be placed into the high score table after the game ends.

#### POW Blocks

POW blocks can be used to knock over any Koopas on the map. When a POW block is hit, it uses up one out if its three uses. When the POW block runs out of uses, it disappears into thin air!

#### Coins

Coin spawn in random positions all over the map, each time the user enters a game, the coins will be in different positions. There are always a total of 20 coins on each level. The coins spawn in dedicated “potential coin spawn locations”. They may even spawn in the air, so the player has to jump to reach them! 

 
