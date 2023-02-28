---
toc: true
layout: post
description: Rough Draft of Collegeboard Create Task
categories: [markdown, ap]
title: Create Task Write Up Draft
---
# Question 3

## Part a

### i
The overall purpose of this program is to help football fans practice their knowledge of NFL statistics by playing a game to see which quarterback has the higher of a certain statistic. This helps people learn more about football and bring them a fun way to interact with player statistics.

### ii
The video will show the user playing the game. The user will see player images pop up on screen and be able to select the player they think has more of a statistic.

### iii
The video will show the user playing the game. In one case, the user will guess the correct player with the higher of a statistic. This will output a message of "Score +1" and increase the tracked score by one. In another case, the user will guess the wrong player with the lower of a random statistic. This will output a message of "Game Over" and reset the score back to 0.

## Part b

![Frontend Ideation]({{ site.baseurl }}/images/code1.png)

![Frontend Ideation]({{ site.baseurl }}/images/code2.png)

### i
The data from the API containing the players and their statistics is stored in a list.

### ii
The second code segment shows the players and their statistics being randomly selected to be output onto the page for the user.

### iii
List: players

### iv
This represents the players and their data which are essential to the running of the game.

### v
Without a list, there would have to be many individual variable for each player and their statistics. This would make put a lot of strain on the computer to iterate through long lists and would also make it hard for the program to be efficient.

## Part c

![Frontend Ideation]({{ site.baseurl }}/images/code3.png)

![Frontend Ideation]({{ site.baseurl }}/images/code4.png)

### i
The given procedure randomly selects the players who will be for the user to choose from.

### ii
The program uses these players for the game.

### iii
The identified features ensures that there are no repeat players and makes the game less buggy for the users.

### iv
The algorithm works by first selecting two random players from the database in order to present to the user. Then, they are checked to make sure that they do not match. The code will then check for which player the user clicked on. If it is the one with more of the statistic, then they will get a point and continue the game. Otherwise, the user loses and the score resets to 0.

## Part d

### i
- First call: Selecting the player which has more of a statistic
- Second call: Selecting the player which has less of a statistic

### ii
- First call: If the user will gain points from selecting the player with more
- Second call: Seeing if the game will end if a player with less of statistic is selected

### iii
- First call: The user will see a message saying that their score is increased and the score will get 1 more.
- Second call: The user will see a message saying the game is over and the score is reset to 0.

# Scoring

| Item | Score | Reasoning |
|---|---|---|
| Program Purpose | 1 | The response describes the function of the program well. |
| Data Abstraction | 1 | The response shows a list being used in the program and talks about how data is abstracted. |
| Managing Complexity | 1 | The response shows why a list is necessary and then talks about how much harder it would be without a list. |
| Procedural Abstraction | 0 | The procedure could be more defined and there could be a better definition of the purpose. |
| Algorithm Implementation | 0 | There is not much sequencing, selection, or iteration going on. The steps are not very detailed and it would be hard to reconstruct the algorithm. |
| Testing | 0 | The response talks about two different general calls to the program. It does not have specific inputs to the program, thus losing the point. |
