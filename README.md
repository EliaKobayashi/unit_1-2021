# Unit 1: A classic game 
![](game.gif)

# Criteria A: Planning

## Problem definition

The owner of the local game shop is an enthusiast of classic computer games. He has been looking for a talented programmer that can help him revive his passion for text-based games. He has few requirements for this task:

1. The game has to be entirely text-based.
2. The game must record the time played.
3. The game must record the player name and score.

Apart for this requirements, the owner is open to any type of game, topic or genre. 

## Personal Problem Definition.

Ever since I was little, I would watch the Champions League with family and friends anually. It was a competition that would bring people together with so much joy and excitement. Even if my favorite team could never win, I had a lot of fun watching the tournament. Thus, I wanted to turn all this nostalgia, joy, and excitement into a game. Additionally, I have seen many text-based games that are focused on mystery or survival. However, it is extremely rare to find a text-based game for football. Hence why I decided to create a football game based on the Champions League.

# Proposed Solution

## Success Criteria

1. The game will calculate how well a user did in the game based on their rating.
2. It must validate user inputs.
4. The game will be a career mode video game based on the champions league. Meaning, the user will become a professional football player and play in the Champions League in the game. 
6. The video game save the rating, time spent, and username of a user.
7. The user will have a rating which can be improved based on their proformances in matches.
8. The game will be available in English and Japanese.

## Design Statement

I will design and make a classic video game for a client who is looking for a text-based video game with a record of player names and scores. The theme of the video game is football and is constructed using the software python 3.x. It will take a month to make and will be evaluated according to the success criteria mentioned prior.

## Justification

For this game, I will be using python which is, according to statisticstimes.org, the most used coding language in the world and the language I am most comfortable using. Additionally, according to cisin.com, Python is the most versatile language in the world. My text-based game will be coded on the MacOS system and on a Python editor called "PyCharm". Pycharm was chosen as it is simple and easy to code on. Furthermore, it is very easy to store files in.

## Details

My game, "Champions League Career", will be a text-based game that will allow users to play a Champions League tournament with real teams. The game will include a randomisation of the tournament bracket to ensure the game will differ each time the user plays. Furthermore, the games the user doesn't play will be simulated. The game will consist of decisions that have to be made by the users that will affect the outcome of a match. To win the game, one has to win every match and win the tournament. If one loses a match, it will be game over and they will have to replay the game. Each match will contain three to four decision points. Each decision point throughout the game differ from each other. The game will save the user's username, rating, and time spent on the game. Therefore, if the user were to play the game again, they can look at their previous score. 

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

![](unit_test1.jpg)

Figure 5. First unit testing evidence

![](unit_test2.jpg)

Figure 6. Second unit testing evidence
## Test Plan

| Description                                                                | Type                | Inputs                                                                                                                                                          | The Expected Output                                                                                                                                                                                                                                                                                 | Evidence of Output                           |
|----------------------------------------------------------------------------|---------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------------------------|
| Testing if the system which creates the tournament bracket works randomly. | Unit Testing        | 1. Initiate the program. 2. Enter the teams that you would like to be in the tournament                                                                         | Randomly places teams against each other for the round of 16.                                                                                                                                                                                                                                       | ![](unit_test1.jpg)                          |
| Test if the validation function.                                           | Unit Testing        | 1. Initiate the program. 2. When asked to input 1 or 2, input 3.                                                                                                | As the input was not 1 or 2, it should print "Wrong input." and the same message will print again.                                                                                                                                                                                                  | ![](unit_test2.jpg)                          |
| Test if the entirety of the first match works.                             | Integration Testing | 1. Initiate the program. 2. Input the first scenario. 3. Input the second scenario. 4. Input the third scenario.                                                | Depending on if the user chooses the right decision in the scenarios, they will win or lose. The game should accurately decide if the user won or lost. Furthermore, it should alter their rating according to their choices in the game.                                                           | https://www.youtube.com/watch?v=LoLProu7Gio  |
| Test if the entire game works                                              | System Testing      | 1. Initiate the program. 2. Complete the introduction. 3. Finish the round of 16. 4. Finish the quarter-finals. 5. Finish the semi-finals. 6. Finish the final. | The game should smoothly play through each match and depending on the results of the matches, the game should print the accurate outcome. The game will end with the user either winning or losing the tournament. Furthermore, the game should ask if the user would like to save their progress.  | https://www.youtube.com/watch?v=y8yJ-U5exgw  |


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
