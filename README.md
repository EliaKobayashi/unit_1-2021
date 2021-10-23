# Unit 1: A classic game 
![](game.gif)

# Criteria A: Planning

## Problem definition

The owner of the local game shop is an enthusiast of classic computer games. He has been looking for a talented programmer that can help him revive his passion for text-based games. He has few requirements for this task:

1. The game has to be entirely text-based.
2. The game must record the time played.
3. The game must record the player name and score.

Apart for this requirements, the owner is open to any type of game, topic or genre. 


## Proposed Solution

I will design and make a classic video game for a client who is looking for a text-based video game with a record of player names and scores. The video game will about football and is constructed using the software python It will take a month to make and will be evaluated according to the criteria ____.

## Success Criteria

1. If the ranking table contains username, score, and is able to properly rank based on scores, it can be deemed successful.
2. It must validate user inputs.
4. The game will be a career mode video game based on the champions league. Meaning, the user will become a professional football player and play in the Champions League in the game. 
6. The video game will have a login system where the player can save their progress.
7. The user will have a rating which can be improved based on their proformances in matches.
8. The game will be available in English and Japanese.

## Personal Connection

Ever since I was little, I would watch the Champions League with family and friends anually. It was a competition that would bring people together with so much joy and excitement. Even if my favorite team could never win, I had a lot of fun watching the tournament. Thus, I wanted to turn all this nostalgia, joy, and excitement into a game. Additionally, I have seen many text-based games that are focused on mystery or survival. However, it is extremely rare to find a text-based game for football. Hence why I decided to create a football game based on the Champions League.

# Criteria B: Design

## System Diagram

![](system_diagram)

Figure 1. System diagram for the proposed solution.

As shown in Fig.1, the proposed solution runs on Python and it is developed using Pycharm (v. 2021). The proposed game, "Champions League Legend" has two inputs (1 and 2). Depending on the input, the output will differ in game situations.

## Flow Diagrams

![](one_flowchart.jpg)

Figure 2. Flow dagram of the entire game

As shown in Fig.2, the game will consist of a plethora of choices carried on by the users. Depending on the choices, the ending of the game will differ as well. Although Fif.2 does not contain all the details of the game, it contains the key elements.

![](second_function.jpg)

Figue 3. Flow diagram of tournament bracket making

As shown in Fig3, the game will contain a bracket making system. This system will randomly place teams into each seed.

![](third_flowchart.jpg)

Figure 4. Flow diagram of encoder

As shown in Fig. 4, there will be an encoder at the end of the game to store the data of the users in a manner which is safe. If the file is leaked, the encoder will ensure that no one is able to find personal details about the users.

### Cesar's Cypher
The database in the game has to be protected so that personal data is not exposed. To solve this I am using the Cesar Cypher. **Fig 2.** shows that flow diagram for this function. 

## Record of Tasks
| Task No | Planned Action                                  | Planned Outcome                                                                                                   | Time estimate | Target completion date | Criterion |
|---------|-------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1.      | Write a proposed solution                       | To find a solution that solves the client's problems                                                              | 15 minutes    | September 20           | A         |
| 2.      | To create a success criteria                    | To find ways to evaluate whether my solution is successful or not                                                 | 15 minutes    | September 20           | A         |
| 3.      | Create system diagram.                          | To have a clear idea of the hardware and software of the program                                                  | 10 minutes    | September 20           | B         |
| 4.      | code an introduction for the user               | For the users to understand how to play the game.                                                                 | 1 hour        | September 18           | C         |
| 5.      | Code a system that randomly generates a bracket | To generate random matches in a tournament style.                                                                 | 2 hours       | September 22           | C         |
| 6.      | Create a system that simulates random matches   | To have codes so that some matches can be simulated                                                               | 2 hour        | September 25           | C         |
| 7.      | Create an encryption for the user data          | A function tested that uses the Cesar Cypher                                                                      | 20 minutes    | October 6              | C         |
| 8.      | Create game scenarios                           | To create scenarios similar to what would happen in a real football game.                                         | 2 hours       | October 10             | C         |
| 9.      | Find an ASCII text                              | For the trophy when the user wins.                                                                                | 10 minutes    | October 12             | C         |
| 10.     | Add a delay function                            | To make the game run better                                                                                       | 15 minutes    | October 13             | C         |
| 11.     | Add a validation function                       | So that if the user inputs something that is not a 1 or a 2, it will ask the user until they put the right input. | 20 minutes    | October 13             | C         |
| 12.     | Add a clear function                            | To make the game run more smoothly                                                                                | 15 minutes    | October 13             | C         |
| 13.     | Organize everything into one game               | Organize everything so that the game can run smoothly                                                             | 30 minutes    | October 15             | C         |
| 14.     | Create the first flowchart                      | Create a flowchart that shows the general flow of the entire game                                                 | 30 minutes    | October 18             | B         |
| 15.     | Create the second flowchart                     | Create a flowchart that showcases how the tournament bracket is randomly generated.                               | 30 minutes.   | October 18             | B         |
| 16.     | Create the third flowchart                      | Create a flowchart that showcases how the game encodes users' information.                                        | 30 minutes    | October 23             | B         |
