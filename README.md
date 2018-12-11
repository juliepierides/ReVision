# ReVision
A 2D platformer game.

## Summary
The game that we’ve created is called “Re-Vision”. It is a narrative game that begins with the story of an honorable king who sacrificed himself for the people in his kingdom.

After reading this, the player begins as a knight character in a 2D platformer game and there is a text box on the bottom of the screen that shows someone talking to him. 

![alt text](https://raw.githubusercontent.com/juliepierides/ReVision/book.png)

This is the king from the story in the beginning. The king guides the knight throughout the game by telling him how to play and what he must do. 

We created all graphical assets in the game from scratch, except for the pages and the glasses.

## Goal
The king’s goal is to get the knight to free him from the game, but throughout the game, the knight uncovers the real version of the story and realizes that the king is actually evil. In order to keep the king imprisoned in the game, he must first find the skeleton of the person who failed the same mission. At the place of the skeleton, there is also a note and a pair of glasses. These glasses allow the player to see hidden platforms and also reveal which platforms are fake. The game is called Re-Vision because the evil king revised the original story and the knight can wear glasses to reveal the real platforms of each level. 
## Multiple Endings	
There are two different endings to the game. If the player does not realize that the king is evil (he probably did not read the beginning story and the note with the skeleton), then he will do what the king says and release him from the game, which causes the player to lose. The other ending occurs if the player chooses to disobey the king’s orders. The knight would then beat all of the levels and destroy the game by pressing the button in the last room. When the button is pressed, the game can no longer be opened without changing a variable in the code manually. In order to restart the game, you must relocate these files on your computer (C > Users > you > AppData > Local > ReVision > breakbutton) and change the 1 value to -1 in the text document. (the AppData folder is usually hidden, which can be revealed by clicking on the “View” tab and checking the box that says “Hidden Items” (this works for Windows).
## Inspiration
Many of the games that we were inspired by had twists and simple mechanics. We were inspired by Braid’s mind-blowing plot twist in which the game causes the player to think that he is saving a girl in need, but instead it is you she is running from. Other games with plot twists like these that we took inspiration from are Pony Island, Doki Doki Literature Club, and Bioshock. We also took graphic inspiration from Undertale and we decided to have a simple mechanic because of Super Meat Boy.

## Video
[![Watch the video](https://drive.google.com/open?id=1mb3IjaVdcyD48aDFLnWzxRlr3M9eyHIt)](https://drive.google.com/open?id=1N-PT56zL6xbHkulBCaLVZk-hNL6PJFey)

## How to Play
- Left arrow = left
- Right arrow = right
- Space = jump
- Control = glasses function (only works when you are not moving)
- K key = open big door with key

## Formal System
- Environment:
  - 2D platformer
  - The player begins outside of a castle and eventually enters the castle
- Objects (with attributes and internal relationships):
  - King
    - Text pops up on the bottom of the screen when he talks to the knight
    - He was trapped by a warlock because he was too evil for society.
  - Knight
    - Playable character who can jump, move left and right, and have events that occur when he collides with certain objects (spikes, book pages, glasses, key, doors)
  - Small doors 
    - Allows the knight to travel to the next room
  - Big door with keyhole
    - Contains the king
    - Player can press the K key on the door to free the king
  - Normal Platforms
    - Knight can jump on them
  - Invisible Platforms
    - Knight can jump on them
    - Invisible platforms can be seen after the knight has obtained the glasses and presses the control key without moving.
  - Fake Platforms
    - Knight cannot jump on them; he can travel through them
    - They can disappear after the knight has obtained the glasses and presses the control key without moving.
  - Arrows
    - Hazards that fall from above and kill the player character
  - Spikes
    - Knight can collide with them and be teleported to the beginning of the room (the knight dies)
  - Key
     - Can be picked up by the knight and used on the big door by pressing the K key.
    - Releases the king from his prison.
  - Destroy Button
    - Knight touches it to destroy the game
  - Glasses
    - Previous owner died while pursuing the destruction of the game
    - Can be picked up by the knight 
    - Lets the knight see invisible platforms by pressing the control key
    - Lets the knight see through fake platforms by pressing the control key
  - Torn pages from original book
    - When touched by the knight, a bigger version pops up on the screen that is readable by the player
    - Reveals the true story and nature of the king
  - Note from previous player’s journal
    - When touched by the knight, a bigger version pops up on the screen that is readable by the player
    - Tells the knight not to trust the king 
    - Tells the knight how to use his glasses
    - Tells the knight that it’s not just a simple game that he is playing for enjoyment

