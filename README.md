# Advanced-RPG
VB.Net Advanced RPG
Quiggly Game

The object of the game is to solve a quest.
As you read signs or talk to people, the
response you get will be different
depending on the quest you are on

Tiles.Csv - You can add new tiles to the game![q1](https://github.com/Billvbcode/Advanced-RPG/assets/74204458/b91984bf-1de7-45fa-ab3f-c0f25ce542d6)

  TileName, OldChr, Type, MapTile

******MagicPoints***** 
MagicPoints < 15  None 
MagicPoints > 14 And MagicPoints < 25  Thoughts
MagicPoints > 24 And MagicPoints < 35  Pence 
MagicPoints > 44 And MagicPoints < 55  1 - Transport 1 
MagicPoints > 54 And MagicPoints < 65  2 - Transport 2 
MagicPoints > 34 And MagicPoints < 135 3 - Transport 3 

******To making a game:***** 
xxxxyyyyNewxNewy            
<0001>                           = Number 1
Mother: Hello                    = Item 1 and and what they say 
0003=Any advice?                 = The answer will be number 3
0000=Goodby                      = End Speech
<0003>                           = Number 3
Mother: Talk to your brother     = Item 3 and and what they say 
SQuest!0001                      = Start quest 1 
QuestN!Talk to your brother      = Quest Name
EQuest!0001                      = End quest 1 
QuestNo!0001                     = Quest is started
QuestYes!0001                    = Quest is Done
QuestName!Talk to your brother   = Quest Name
Give!Ticket                      = Items given to you 
Giveqty!01                       = Give Qty
Need!Wood                         = Item you give away 
Needqty!01                       = Need Qty
Bombqty!01                       = Bombs given to you
FixX!0010                        = X Pos - Make grass
FixY!0022                        = Y Pos - Make grass
FixMap                           = Grass,Tile,Stargate,Stairs

*********Speach Sequence*********
1) What to say after quest is done  (QuestYes!0001)
2) What to say if quest is started  (QuestNo!0001  or EQuest!0001)
3) What to say 
4) What to say if you give me the item I need and quest is started (QuestNo!0001  or EQuest!0001)

*********Example*********

Your brother will not say this until you have started quest 1

<0004>
Brother: The White Wizard wants to talk to you, you can find him on Mini Island.
0000=Thanks
EQuest!0001
BombQty!01
SQuest!0002
QuestName!Find The White Wizard on Mini Island  

********Spells**********
A - Axe Tree          B - Bomb Wall 
C - Cut Weeds         D - Destroy Rock
F - Fill Swamp        G - Grow Grass
L - Light Darkness    1-Transport 1 space
2-Transport 2 spaces  3-Transport 3 spaces
