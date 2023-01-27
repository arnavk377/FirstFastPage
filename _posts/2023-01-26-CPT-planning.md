---
toc: true
layout: post
description: Planning Blog
categories: [markdown, ap]
title: Create Performance Task Planning
---

My project is creating a game about NFL statistics to see which player has more of a certain statistic.

# Meeting Collegeboard Standards

| Reporting Category | How my Project will meet it |
| --- | --- |
| Program Purpose and Function | My program will serve to be a way to entertain people and provide them with a source to practice sports trivia. |
| Data Abstraction | I will store players in lists based on their positions. Each player will have a variable assigned to them, which will hold their stats. I will then randomly select two players from a list and randomly select a statistic to test the user on. |
| Managing Complexity | The list would be used to manage the players. Without a list, the program would be inefficient, because it would have to call all players from a group before random selection. |
| Procedural Abstraction | I will develop a procedure to randomly select the two players and create an output for the user. I will store the user's response in a variable and use that to decide what to do on the next screen(game over or continue on). |
| Algorithm Implementation | The algorithm which I will use will check if the user chose the player with more of a certain statistic. If so, then another challenge will be generated. The challenges will appear until the user gets one wrong. This shows sequencing, selection, and iteration. |
| Testing | I will test multiple calls. I will test one call where I select the player who has more in the statistic than another player. Then, I will test a call where I select the player who has less in the statistic than the other player. This will test the continuation feature of the game as well as the ending of the game. | 

# Video Planning
This which I plan to show in my video:
- User correctly selecting player
- User incorrectly selecting player
- Final screen after wrong answer

# Code Plan
Potential code segments to submit to Collegeboard:
- Usage of list to store list of players
- Code which will determine whether user will get another question or if the game will end
- Accessing the list storing the player data