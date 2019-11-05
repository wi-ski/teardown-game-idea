# Teardown Game Idea: "Chess"

Hi there!  I don't know if you're active with communication, but I have have a game/mode in mind that would leverage the mechanics that youve been demonstrating in your engine - for Teardown - and I cant stop thinking about it. This is an attempt to see if:

1. You're human.
1. Are open to communication.
1. Would even appreciate me blabbing my thoughts into a form you could parse.

# Brief Game Format Outline

The game is best described as a 1v1 FPS/RTS Hybrid that revolves around balancing "macro-ing" groups of dota-spawn-style MOBs/NPCs and "micro-ing" individual MOBs in a First-person-shooter mode.

Two opposing sides of a chessboard-esque map are pitted against eachother with the goal of killing the other team's King.

## Map
The map is large-r and intended to mirror a Chess board.
1. Each player's "side/town" consists of the two rows most proximal to them.
1. The remaining 4 rows in the "middle" are neutral and sparse (few, if any, buildings)

### MOB Types and Squares
1. These player-owned "rows" have randomly alotted destructible buildings that spawn MOBs/NPCs in a DOTA-esque fashion.
    1. The front-most rows begin functional - meaning, they spawn units from the opening of the game.
        - More advanced squares are enabled/unlocked (details pending. Im still 90% Ill never speak with a human regarding this game idea #budget)
    1. The front-most "squares" spawn the most basic unit, "The Pawn"
        - Voxilated Human-looking soldier modal with a WW2 style helmet that resembles a "Pawn" in chess.
        - Melee attack only: Hammer.
    1. The back-most "squares" spawn more advance units.
        1. "The Knight"
            - Ranged Attack only: Simple gun with a slow moving pellet. Layers well with pawns in front.

        1. "The Bishop"
            - Melee attack only, but high damage. Has added benefit and auto-deleting building materials like walls.  Currently thinking this will feel like a "lightsaber" in the way it cuts through walls.

        1. "The Rook"
            - Large profile (literally bigger) ranged unit with splash damage.
            - Would be awesome if style was larger unit that had a boulder-throwing animation.

        1. Eventually "The Queen"
            - Playing around with the mechanics. But a larger, high damage unit, that can teardown buildings more quickly than normal units.

## Unit Spawn Mechanic
Units spawn on an interval, their MOBA-style objectives can be redirected by "The King" (the controlling player). The intention is to force a game style where the user is forced to balance between:
1. Macro-ing in the rts-stlye "god view" - similar to the view in Teardown's demos where you can review your escape path - where you command spawned MOBs/NPCs and have a generous field of view.
1. Micro-ing individual MOBS that a controlling player can assume control of - the assumption being the human's attention makes that unit more effective.
    - Thinking that mobs are less effective than a human (ie. miss ranged attacks frequently/randomly). "The Player" assuming control of a unit would make it more effective by having the accuracy of said player (FPS-style)

## Units Behavior

Like in DOTA, MOBs/NPCs default to agro-ing towards the opposing player's mirror-ed squares with the inention of destroying buildings they agro while en-route.
    - If MOBs manage to "demolish" a players building, that building ceases spawning units.
    -  Demolishing a building is destroying >50% the voxels the comprise the building.

```
                  _        _        _        __       __       _
        /\       |_)      /        | \      |_       |_       /        |_|
       /--\      |_)      \_       |_/      |__      |        \_?      | |

  _           #########         #########         #########         #########
 (_)   [`'`'] ##\`.'/##  ':v:`  ##/\:/\##  |:+:|  ##':v:`##  \`.'/  ##[`'`']#  
 (_)    |::|  ##(o:o)##  (o:0)  #/(o:o)\#  (o:o)  ##(o:0)##  (o:o)  ###|::|##
        |::|  ###\:/:\#   (:)   ###(:)###   (:)   ###(:)###   \:/:\ ###|::|##
              ####"####         #########         #########    "    #########
  __ #########    _    #########    _    #########    _    #########    _      Notes:
   / ###(:)###   (:)   ###(:)###   (:)   ###(:)###   (:)   ###(:)###   (:)      1. As outlined above, these "player owned" squares contain destructible buildings
  /  ###|:|###   |:|   ###|:|###   |:|   ###|:|###   |:|   ###|:|###   |:|      2. Mobs spawn from these squares and march to oppsing team.
     ###|:|###   |:|   ###|:|###   |:|   ###|:|###   |:|   ###|:|###   |:|      
     #########         #########         #########         #########              Units spawns!
              #########         #########         #########         #########   |
  /           #########         #########         #########         #########   |
 (_)          #########         #########         #########         #########   |
              #########         #########         #########         #########   |  ...marching to the fight!
              #########         #########         #########         #########   |
  _  #########         #########         #########         #########            |
 |_  #########         #########         #########         #########            |
  _) #########         #########         #########         #########            |
     #########         #########         #########         #########            |
     #########         #########         #########         #########            ▼ 3. In the early game, MOBs meet here. "The King's" actions determine the outcome of these
   .          #########         #########         #########         #########   ▲    early fights.
  /|          #########         #########         #########         #########   | |
 '-|          #########         #########         #########         #########   | |
              #########         #########         #########         #########   | |
              #########         #########         #########         #########   | |
  _  #########         #########         #########         #########            | |
  _) #########         #########         #########         #########            | |
  _) #########         #########         #########         #########            | |
     #########         #########         #########         #########            | |
     #########         #########         #########         #########            | | 4. Eventually, a fight is won/lost and the MOB can begin attacking these buildings.
  _      _    #########    _    #########    _    #########    _    #########     ▼
   )    (_)   ###(_)###   (_)   ###(_)###   (_)   ###(_)###   (_)   ###(_)###   
  /_    | |   ###| |###   | |   ###| |###   | |   ###| |###   | |   ###| |###   
        |_|   ###|_|###   |_|   ###|_|###   |_|   ###|_|###   |_|   ###|_|###   
              #########         #########         #########         #########   
     #########         #########   ___   #########         #########            
  /| ##[`'`']#  \`~'/  ##'\v/`##  /\*/\  ##|`+'|##  '\v/`  ##\`~'/##  [`'`']    
   | ###|  |##  (o o)  ##(o 0)## /(o o)\ ##(o o)##  (o 0)  ##(o o)##   |  |     
     ###|__|##   \ / \ ###(_)###   (_)   ###(_)###   (_)   ###\ / \#   |__|     
     #########    "    #########         #########         ####"####            
```

## Win Condition
The game is won when the one of the players' "Kings" are killed.  "The King" is a unit that:
1. Represents "The Player" - but is a MOB just-the-same.
1. It has a normal amount of health. But a high-damage ranged attack "Deagle" that deals 80% damage to a Pawn.
1. Unlike the other pieces, "The King" spawn behind the final rows.

