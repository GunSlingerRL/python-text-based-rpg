# python-text-based-rpg

This is a text-based role-playing-game I wrote in Python for a school project last year. It is by no means a good game, but I think there is some good code here.

## Game help

The game is run by running play.py in the root of the repository.

There are three different classes: warrior, archer, and mage. Each class has a different set of starting stats, and gets different items in the game.

At a pause in the game when you are not in a battle, you will get a set of standard commands. These including equipping and unequipping items, using items, discarding items, and viewing your inventory, your currently equipped items, and your stats. Items are either equippable or consumable. Equippable items equip to different locations on your person (eg. "head", "torso", "arms"), providing you with stat boosts. Weapons also provide you with their own attacks, although the only real variation of attacks exists in the mage class and it's still very minimal. Additionally, the "map" command is available in every room. In lieu of a graphical map, the map command will textually tell you the room you are in and the rooms around it.

At the start of the list of commands you get will be the list of commands unique to your current situation. This will usually include "move" but may also include "talk" and "attack". After entering one of these commands, you will get a list of targets you can perform that action on eg. the rooms you can move to or the people you can talk to.

All classes have a health stat. If you are a warrior or an archer, you will get an additional stamina stat. If you are a mage, you will get an additional mana stat. Attacks for warriors and archers use stamina, and attacks for mages use mana. At the start of each turn in the battle, both you and your enemy will restore a small amount of stamina/mana. The "rest" command available in battles will use your turn, but restore a much larger amount of stamina/mana. You also recover all stamina/mana at the end of a battle, but your health does not automatically regenrate.

You can also use items during a battle, and this will not use up your turn. Primarily though, you can attack. Using the attack command will give you a list of all the attacks you can use, from which you can select one. Attacks have a base damage value associated with them. However, the actual amount of damage an attack will deal depends on your stats and your enemy's stats and some random number generation.
