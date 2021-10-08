---
title: Unit Entities
date: 2021-10-05 13:00:48
tags: 
---
I've been working on getting units into the game world using the same entity base classed used by trees. This means that units like other entities will be updated 
together in the same way each tick.

The unit entity will have a UnitAI object that uses the state desgin pattern, this will hopfully result in being able to change the AI applied to the unit easily.
I plan to use A* pathfinding for finding a path accross the world, right now the units wonder around a bit more randomly but the basics for A* are there and I 
should not have much issue adding it soon. 

Below is a short video of the units and AI in action, I recorded this on my macbook while away on holiday which was also intresting as I was able to get the game
working on both MacOS and Windows! 

There is a small issue in this video also with units moving more then once per tick due to them moving into a block that has not yet been updated, updating the same entity more then once. I plan on fixing this using a list of entities already updated this tick which is cleared every tick.

{{< youtube U3T5syUySmg >}}
