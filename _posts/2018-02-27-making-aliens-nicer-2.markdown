---
layout: post
title:  "Making Alien Cruisers Nicer: Part II"
date:   2018-02-27 22:57:10 -0800
categories: dts game
---
Feb 27
Yesterday I made the alien cruisers a little nicer by making them vary their speed slightly to add some noise to their pattern.
This introduced a problem where one alien cruiser can spawn in the same lane as another, but move at a slower speed than the one behind, causing them to collide mid-screen, as in the top lane here:

I will fix this by not allowing an obstacle to spawn in a lane that’s already occupied by an obstacle.

This is the result:

![game screenshot](https://www.dropbox.com/s/7zvb32yzcbfqwh7/2018-02-27%2023.19.23.gif?raw=1)

A little better but highlights a problem with the spawner -- after destroying an enemy in a lane, there can be a quite significant (in rapid gameplay time) delay before the lane is occupied with another enemy.
