---
title: Trees and Grass
date: 2021-09-26 22:46:48
tags:
---

Tonight I was able to get block floors and trees updating on update ticks. At the moment we are going by 1 update tick == 1 game world hour. Update ticks can be set to be any fraction of real world seconds so .5 real world seconds could equal 1 game hour for example, this should result in being able to set the games speed.

Grass growing right now is done by looking for blocks with grass as the floor checking if a dirt floor block is nearby and if it is doing a dice roll, the dice roll chooses if a grow happens and the direction it will grow in.

Trees are my first World Entity class. The update method for entities is called every tick and for trees a tick count is used to grow fruit or drop the fruit. This can be seen in the video with trees gaining and losing red dots which represent apples.

{{< youtube s8G2osx-I2s >}}

[Video of Trees and Grass](https://www.youtube.com/watch?v=s8G2osx-I2s)
