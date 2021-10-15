## My MVP
```.py
import os
import time
time.sleep(1.5)
import sys
def dp(str):
    for char in str:
        sys.stdout.write(char)
        sys.stdout.flush()
        time.sleep(0.025)
    return ""
def clear():
    os.system("clear")

def validation(msg):
    option = int(input(dp(msg)))
    while option not in [1, 2]:
        option = int(input(dp("Wrong input" + msg)))
    return option

username = input(dp("Welcome to Champions League Career! Please input your username: \n"))
dp(f"Hi {username}! This game is a simulation of a Champions League. \n")
dp("You will be making decisions which will affect your player's rating.\n ")
dp("Your player's current rating is 70. The maximum rating is 99. \n ")
clear()
rating = 70
age = 20
dp("For your player's first team, please pick between: Sevilla, Atalanta, Porto, Milan: \n ")
first_team = input(dp("Please enter the name of the team you would like to join here: \n "))
while first_team not in "SevillaAtalantaPortoMilan":
    first_team = input(dp("Wrong input. Please enter the team name including the first letter being capital: \n"))
dp(f"Welcome {username} to your first team {first_team}. \n")
clear()
#print("If you would like to be a goalkeeper, type: GK. ")
#print("If you would like to be a defender, type: DF. ")
#print("If you would like to be a midfielder, type: MF. ")
#print("If you would like to be an attacker, type: AC. ")
#position = input("Enter here: ")
#while position not in "GKDFMFAC":
    #position = input("Wrong input. Please enter either 'GK','DF', 'MF', 'AC': ")
import random
first_teams = ["Milan", "Atletico Madrid", "Real Madrid", "Dortmund", "Barcelona", "Atalanta", "Sevilla", "Juventus"]
second_teams = ["Manchester City", "PSG", "Chelsea", "Bayern", "Manchester United", "Liverpool", "Inter Milan", "Porto"]
first_bracket = random.choice(first_teams)
second_bracket = random.choice(second_teams)
first_teams.remove(first_bracket)
second_teams.remove(second_bracket)
third_bracket = random.choice(first_teams)
fourth_bracket = random.choice(second_teams)
first_teams.remove(third_bracket)
second_teams.remove(fourth_bracket)
fifth_bracket = random.choice(first_teams)
sixth_bracket = random.choice(second_teams)
first_teams.remove(fifth_bracket)
second_teams.remove(sixth_bracket)
seventh_bracket = random.choice(first_teams)
eighth_bracket = random.choice(second_teams)
first_teams.remove(seventh_bracket)
second_teams.remove(eighth_bracket)
ninth_bracket = random.choice(first_teams)
tenth_bracket = random.choice(second_teams)
first_teams.remove(ninth_bracket)
second_teams.remove(tenth_bracket)
eleventh_bracket = random.choice(first_teams)
twelfth_bracket = random.choice(second_teams)
first_teams.remove(eleventh_bracket)
second_teams.remove(twelfth_bracket)
thirteenth_bracket = random.choice(first_teams)
fourteenth_bracket = random.choice(second_teams)
first_teams.remove(thirteenth_bracket)
second_teams.remove(fourteenth_bracket)
fifteenth_bracket = random.choice(first_teams)
sixteenth_bracket = random.choice(second_teams)
dp("Now, the Champions League starts! The tournament starts with a round of 16. The following are the matches! \n")
dp(f"{first_bracket} versus {second_bracket} \n")
dp(f"{third_bracket} versus {fourth_bracket} \n")
dp(f"{fifth_bracket} versus {sixth_bracket} \n")
dp(f"{seventh_bracket} versus {eighth_bracket} \n")
dp(f"{ninth_bracket} versus {tenth_bracket} \n")
dp(f"{eleventh_bracket} versus {twelfth_bracket} \n")
dp(f"{thirteenth_bracket} versus {fourteenth_bracket} \n")
dp(f"{fifteenth_bracket} versus {sixteenth_bracket} \n")
clear()
if first_team == first_bracket:
    dp(f"You are going to go against {second_bracket} \n")
    first_team = first_bracket
    main_match = [first_bracket , second_bracket]
elif first_team == second_bracket:
    dp(f"You are going to go against {first_bracket} \n")
    first_team = second_bracket
    main_match = [first_bracket, second_bracket]
elif first_team == third_bracket:
    dp(f"You are going to go against {fourth_bracket} \n")
    first_team = third_bracket
    main_match = [third_bracket, fourth_bracket]
elif first_team == fourth_bracket:
    dp(f"You are going to go against {third_bracket} \n")
    first_team = fourth_bracket
    main_match = [third_bracket, fourth_bracket]
elif first_team == fifth_bracket:
    dp(f"You are going to go against {sixth_bracket} \n")
    first_team = fifth_bracket
    main_match = [fifth_bracket, sixth_bracket]
elif first_team == sixth_bracket:
    dp(f"You are going to go against {fifth_bracket} \n")
    first_team = sixth_bracket
    main_match = [fifth_bracket, sixth_bracket]
elif first_team == seventh_bracket:
    dp(f"You are going to go against {eighth_bracket} \n")
    first_team = seventh_bracket
    main_match = [seventh_bracket, eighth_bracket]
elif first_team == eighth_bracket:
    dp(f"You are going to go against {seventh_bracket} \n")
    first_team = eighth_bracket
    main_match = [seventh_bracket, eighth_bracket]
elif first_team == ninth_bracket:
    dp(f"You are going to go against {tenth_bracket} \n")
    first_team = ninth_bracket
    main_match = [ninth_bracket, tenth_bracket]
elif first_team == tenth_bracket:
    dp(f"You are going to go against {ninth_bracket} \n")
    first_team = tenth_bracket
    main_match = [ninth_bracket, tenth_bracket]
elif first_team == eleventh_bracket:
    dp(f"You are going to go against {twelfth_bracket} \n")
    first_team = eleventh_bracket
    main_match = [eleventh_bracket, twelfth_bracket]
elif first_team == twelfth_bracket:
    dp(f"You are going to go against {eleventh_bracket} \n")
    first_team = twelfth_bracket
    main_match = [eleventh_bracket, twelfth_bracket]
elif first_team == thirteenth_bracket:
    dp(f"You are going to go against {fourteenth_bracket} \n")
    first_team = thirteenth_bracket
    main_match = [thirteenth_bracket, fourteenth_bracket]
elif first_team == fourteenth_bracket:
    dp(f"You are going to go against {thirteenth_bracket} \n")
    first_team = fourteenth_bracket
    main_match = [thirteenth_bracket, fourteenth_bracket]
elif first_team == fifteenth_bracket:
    dp(f"You are going to go against {sixteenth_bracket} \n")
    first_team = fifteenth_bracket
    main_match = [fifteenth_bracket, sixteenth_bracket]
elif first_team == sixteenth_bracket:
    dp(f"You are going to go against {fifteenth_bracket} \n ")
    first_team = sixteenth_bracket
    main_match = [fifteenth_bracket, sixteenth_bracket]
clear()

first_match = [first_bracket , second_bracket]
second_match = [third_bracket , fourth_bracket]
third_match = [fifth_bracket , sixth_bracket]
fourth_match = [seventh_bracket , eighth_bracket]
fifth_match = [ninth_bracket , tenth_bracket]
sixth_match = [eleventh_bracket , twelfth_bracket]
seventh_match = [thirteenth_bracket , fourteenth_bracket]
eighth_match = [fifteenth_bracket , sixteenth_bracket]

game_rating = 0
goal = 0
#First scenario
dp("And the whistle blows! The round of 16 starts now! \n")
clear()
one_ac = validation("You are in the box and a player crossed the ball to you. \n Type 1 for an overhead kick. 2 to head the ball: \n")
if one_ac == 1:
    dp("SCORE! You scored a beautiful overhead kick that nestled into the top right corner \n")
    game_rating += 1
    goal += 1
elif one_ac == 2:
    dp("You headed the ball to the center of the goal. The keeper comfortably saved it. \n")
clear()
one_ac = validation("The other team is attacking down the left side of the field. You are in the box defending a player from the other team. The other team's winger crosses the ball. \n Type 1 for heading the ball away. Type 2 for shoulder checking the other team: \n")
if one_ac == 1:
    dp("You head the ball away and defend perfectly.")
    game_rating += 1
if one_ac == 2:
    dp("You foul the other team which leads to a penalty. The other team scores the penalty. \n")
    goal -= 1
clear()
one_ac = validation("You are attacking in a counter attack. There is a player defending you. \n Type 1 to send a long pass to a teammate of yours running down the left side. Type 2 to dribble past the defender. \n")
if one_ac == 1:
    dp("The defender blocks your pass. The other team counters your attack and scores from outside the box. \n")
    goal -= 1
if one_ac == 2:
    dp("You dribble past the defender and score a banger from outside the box. \n")
    game_rating += 1
    goal += 1
clear()
if goal == 0:
    penalty1 = validation("The match tied and you have a last minute penalty. \n Type 1 for shooting left. Type 2 for shooting right: \n")
    if penalty1 == 1:
        dp("You scored!!! The referee blows his whistle and the game is over.\n")
        goal = 1
    if penalty1 == 2:
        dp("You missed!!! The other team launch a counter attack and win the game in the last minute. \n")
        goal = -1
clear()
if goal <= -1:
    dp("GAME OVER. Your team lost the Champions league \n")
else:
    if first_team not in first_match:
        q_first_match =(random.choice(first_match))
        # dp(f"{q_first_match} won! \n")
    else:
        q_first_match = first_team
    if first_team not in second_match:
        q_second_match = (random.choice(second_match))
        # dp(f"{q_second_match} won! \n")
    else:
        q_second_match = first_team
    if first_team not in third_match:
        q_third_match = (random.choice(third_match))
        # dp(f"{q_third_match} won! \n")
    else:
        q_third_match = first_team
    if first_team not in fourth_match:
        q_fourth_match = (random.choice(fourth_match))
        # dp(f"{q_fourth_match} won! \n")
    else:
        q_fourth_match = first_team
    if first_team not in fifth_match:
        q_fifth_match = (random.choice(fifth_match))
        # dp(f"{q_fifth_match} won! \n")
    else:
        q_fifth_match = first_team
    if first_team not in sixth_match:
        q_sixth_match = (random.choice(sixth_match))
        # dp(f"{q_sixth_match} won! \n")
    else:
        q_sixth_match = first_team
    if first_team not in seventh_match:
        q_seventh_match = (random.choice(seventh_match))
        # dp(f"{q_seventh_match} won! \n")
    else:
        q_seventh_match = first_team
    if first_team not in eighth_match:
        q_eighth_match = (random.choice(eighth_match))
        # dp(f"{q_eighth_match} won! \n")
    else:
        q_eighth_match = first_team
    quarterfinals = [q_first_match, q_second_match, q_third_match, q_fourth_match, q_fifth_match, q_sixth_match, q_seventh_match, q_eighth_match]
    first_bracket2 = random.choice(quarterfinals)
    quarterfinals.remove(first_bracket2)
    second_bracket2 = random.choice(quarterfinals)
    quarterfinals.remove(second_bracket2)
    third_bracket2 = random.choice(quarterfinals)
    quarterfinals.remove(third_bracket2)
    fourth_bracket2 = random.choice(quarterfinals)
    quarterfinals.remove(fourth_bracket2)
    fifth_bracket2 = random.choice(quarterfinals)
    quarterfinals.remove(fifth_bracket2)
    sixth_bracket2 = random.choice(quarterfinals)
    quarterfinals.remove(sixth_bracket2)
    seventh_bracket2 = random.choice(quarterfinals)
    quarterfinals.remove(seventh_bracket2)
    eighth_bracket2 = random.choice(quarterfinals)
    dp("Now the quarter finals start! The following are the matches! \n")
    dp(f"{first_bracket2} versus {second_bracket2} \n")
    dp(f"{third_bracket2} versus {fourth_bracket2} \n")
    dp(f"{fifth_bracket2} versus {sixth_bracket2} \n")
    dp(f"{seventh_bracket2} versus {eighth_bracket2} \n")
    clear()
    if first_team == first_bracket2:
        dp(f"You are going to go against {second_bracket2} \n")
        first_team = first_bracket2
        main_match = [first_bracket2, second_bracket2]
    elif first_team == second_bracket2:
        dp(f"You are going to go against {first_bracket2} \n")
        first_team = second_bracket2
        main_match = [first_bracket2, second_bracket2]
    elif first_team == third_bracket2:
        dp(f"You are going to go against {fourth_bracket2} \n")
        first_team = third_bracket2
        main_match = [third_bracket2, fourth_bracket2]
    elif first_team == fourth_bracket2:
        dp(f"You are going to go against {third_bracket2} \n")
        first_team = fourth_bracket2
        main_match = [third_bracket2, fourth_bracket2]
    elif first_team == fifth_bracket2:
        dp(f"You are going to go against {sixth_bracket2} \n")
        first_team = fifth_bracket2
        main_match = [fifth_bracket2, sixth_bracket2]
    elif first_team == sixth_bracket2:
        dp(f"You are going to go against {fifth_bracket2} \n")
        first_team = sixth_bracket2
        main_match = [fifth_bracket2, sixth_bracket2]
    elif first_team == seventh_bracket2:
        dp(f"You are going to go against {eighth_bracket2} \n")
        first_team = seventh_bracket2
        main_match = [seventh_bracket2, eighth_bracket2]
    elif first_team == eighth_bracket2:
        dp(f"You are going to go against {seventh_bracket2} \n")
        first_team = eighth_bracket2
        main_match = [seventh_bracket2, eighth_bracket2]
    clear()
    first_match2 = [first_bracket2 , second_bracket2]
    second_match2 = [third_bracket2 , fourth_bracket2]
    third_match2 = [fifth_bracket2 , sixth_bracket2]
    fourth_match2 = [seventh_bracket2 , eighth_bracket2]

    game_rating = 0
    goal = 0
    dp("The whistle blows! The quarter-finals start now! \n")
    clear()
    one_ac = validation("The other team gets a penalty! \n Type 1 to dive left. Type 2 to dive right. \n")
    if one_ac == 1:
        dp("The other team scores! And the other team is leading the game. \n")
        goal -= 1
    if one_ac == 2:
        game_rating +=1
        one_ac = validation("The keeper saves it! You are now on a counter attack. You are on the half-way line. \n Type 1 to pass the through ball on the ground. Type 2 to pass a long ball. \n")
        if one_ac == 1:
            dp("The other team gets the ball and the counter attack is stopped. \n")
        if one_ac == 2:
            dp("Your pass went straight to your striker's foot. He has a 1 v 1 opportunity against the goalkeeper. He shoots to the top right corner. GOALLLLL!!! \n")
            goal += 1
            game_rating +=1
    clear()
    one_ac = validation("After getting fouled right outside the opponent's box, you have a free-kick. \n Type 1 to shoot to the top corner. Type 2 to shoot under the wall. \n")
    if one_ac == 1:
        dp("GOALLL!!! You scored a beautiful nuckle ball to the top right corner.\n")
        goal += 1
        game_rating += 1
    if one_ac == 2:
        dp("The wall saves the shot!\n")
    clear()
    one_ac = validation("The other team has two attackers while your team only has one defender. \n Type 1 to defend the person dribbling. Type 2 to defend the person running. \n")
    if one_ac == 1:
        dp("The person dribbling passes to the player running down. But your keeper dives in and saves the play. \n")
        game_rating += 1
    if one_ac == 2:
        dp("The player dribbling shoots and scores!\n")
        goal -= 1
    clear()
    if goal == 0:
        one_ac = validation("You get a last minute corner kick. \n Type 1 to cross the ball. Type 2 to pass short.\n")
        if one_ac == 1:
            dp("Your team header the ball and he scores! GOALLLLLL!!! You win the game in the last minute.\n")
            goal += 1
        if one_ac == 2:
            dp("The other teams steals the ball and sends a long pass to their striker. They dribble past the keeper and score! Your team loses in the last minute. \n")
            goal -= 1
    if goal <= -1:
        dp("GAME OVER. Your team lost the Champions league.\n")
        clear()
    else:
        if first_team not in first_match2:
            s_first_match = (random.choice(first_match))
            # dp(f"{s_first_match} won! \n")
        else:
            s_first_match = first_team
        if first_team not in second_match2:
            s_second_match = (random.choice(second_match))
            # dp(f"{s_second_match} won! \n")
        else:
            s_second_match = first_team
        if first_team not in third_match2:
            s_third_match = (random.choice(third_match))
            # dp(f"{s_third_match} won! \n")
        else:
            s_third_match = first_team
        if first_team not in fourth_match2:
            s_fourth_match = (random.choice(fourth_match))
            # dp(f"{s_fourth_match} won! \n")
        else:
            s_fourth_match = first_team
        semifinals = [s_first_match, s_second_match, s_third_match, s_fourth_match]
        first_bracket3 = random.choice(semifinals)
        semifinals.remove(first_bracket3)
        second_bracket3 = random.choice(semifinals)
        semifinals.remove(second_bracket3)
        third_bracket3 = random.choice(semifinals)
        semifinals.remove(third_bracket3)
        fourth_bracket3 = random.choice(semifinals)
        dp("Now the semi-finals begin! The following are the matches! \n")
        dp(f"{first_bracket3} versus {second_bracket3} \n")
        dp(f"{third_bracket3} versus {fourth_bracket3} \n")
        clear()
        if first_team == first_bracket3:
            dp(f"You are going to go against {second_bracket3} \n")
            first_team = first_bracket3
            main_match = [first_bracket3, second_bracket3]
        elif first_team == second_bracket3:
            dp(f"You are going to go against {first_bracket3} \n")
            first_team = second_bracket3
            main_match = [first_bracket3, second_bracket3]
        elif first_team == third_bracket3:
            dp(f"You are going to go against {fourth_bracket3} \n")
            first_team = third_bracket3
            main_match = [third_bracket3, fourth_bracket3]
        elif first_team == fourth_bracket3:
            dp(f"You are going to go against {third_bracket3} \n")
            first_team = fourth_bracket3
            main_match = [third_bracket3, fourth_bracket3]
        clear()
        first_match3 = [first_bracket3, second_bracket3]
        second_match3 = [third_bracket3, fourth_bracket3]

        game_rating = 0
        goal = 0
        dp("The whistle blows and the semi-finals begin!\n")
        one_ac = validation("Your goalkeeper sends a long pass to you. There is only one defender near you. Type 1 to control and dribble the defender. Type 2 to shoot a volley.\n")
        if one_ac == 1:
            dp("You try to use skill moves against the defender but they steal the ball from you.\n")
        if one_ac == 2:
            dp("You score a beautiful volley that bangs into the top left corner of the goal!!! GOALLLLLL!!!\n")
            goal += 1
            game_rating += 1
        clear()

        one_ac = validation("You are in the middle of the pitch. You get the ball with two defenders near you. Type 1 to make a quick pass to a nearby teammate. Type 2 to try to skill the defenders\n")
        if one_ac == 1:
            two_ac = validation("Your pass was successful and your teammate is trying to decide where to pass the ball. Type 1 to run close to him to recieve the ball. Type 2 to run to the goal to receieve a long pass.")
            game_rating += 1
            if two_ac == 1:
                dp("Your ball got stolen by the defender. \n")
            if two_ac == 2:
                dp("You recieve the ball and shoot on goal. GOAL!!!! You chip the goalie and socre!\n")
                goal += 1
                game_rating += 1
        if one_ac == 2:
            two_ac = validation("Your skill moves fail and the defender strips the ball away. The other team is on a counter attacl. Type 1 to charge at the opponent. Type 2 to try to run back to defense.\n")
            if two_ac == 1:
                dp("You get a yellow card for fouling, but you stopped the coutner attack.\n")
                game_rating += 1
            if two_ac == 2:
                dp("You weren't fast enough to run back to defense and the other team scores.\n")
                goal -= 1
        clear()
        one_ac = validation("You are in the box and you get a ground ball. There is a teammate behind you. Type 1 to pass a back-heal to your teammate behind you. Type 2 to shoot to the goal.\n")
        if one_ac == 1:
            dp("You try the back-heal but you missed the ball.\n")
        if one_ac == 2:
            dp("GOALLLL!!! You tap the ball into the bottom right corner!\n")
            game_rating += 1
            goal += 1
        clear()
        one_ac = validation("The opponent has the ball outside your box. They are looking to shoot the ball. Type 1 to run near them. Type 2 to tackle at them.\n")
        if one_ac == 1:
            dp("You defence was excellence. The other team were unable to shoot.\n")
            game_rating += 1
        if one_ac == 2:
            dp("Your tackle leads to a foul. The other team receives a free kick and they score!\n")
            goal -= 1
        clear()

        if goal == 0:
            one_ac = validation("You are dribbling down the left side of the pitch. There is no one in the box to cross to. But, there is someone outside the box. Type 1 to pass to the player outside the box. Type 2 to keep dribbling.\n")
            if one_ac == 1:
                dp("Your pass is successful and your teammate shoots. GOAL!!!\n")
                goal += 1
            if one_ac == 2:
                two_ac = validation("The opponent strips the ball away from you. There are now in a counter attack. Type 1 for an offside trap. Type 2 to let the defense stay low.\n")
                if two_ac == 1:
                    dp("The offside trap worked! You stopped the attack.\n")
                    three_ac = validation("You get a last minute penalty. Type 1 to shoot left. Type 2 to shoot right.\n")
                    if three_ac == 1:
                        dp("You miss the penalty and the other team launches a counter attack. They cross into the box and GOAL! They score a header in the last minute.\n")
                        goal -= 1
                    if three_ac ==2:
                        dp("GOAL!!! You score a last minute penalty to win the game!")
                        goal += 1
                if two_ac == 2:
                    dp("The defense stays low and the opponent scores from outside the box!")
                    goal -= 1
        clear()
        if goal <= -1:
            dp("GAME OVER. You lost the Champioins League.")
        else:
            if first_team not in first_match3:
                f_first_match = (random.choice(first_match3))
                # dp(f"{q_first_match} won! \n")
            else:
                f_first_match = first_team
            if first_team not in second_match3:
                f_second_match = (random.choice(second_match))
                # dp(f"{q_second_match} won! \n")
            else:
                f_second_match = first_team
            final = [f_first_match, f_second_match]
            dp("Now the final begins! Tha match is the following:\n")
            dp(f"{f_first_match} versus {f_second_match} \n")
            if first_team == f_first_match:
                dp(f"You are going to go against {f_second_match}\n")
                first_team = f_first_match
            elif first_team == f_second_match:
                dp(f"You are going to go against {f_first_match}\n")
                first_team = f_second_match
            clear()

            game_rating = 0
            goal = 0
            dp("The whistle blows and the champions league final begins!\n")
            clear()
            one_ac = validation("You have the ball in the opponent's half with the ball. Type 1 to pass to the striker in the middle. Type 2 to pass a through ball to the winger.\n")
            if one_ac == 1:
                two_ac = validation("Your pass was intercepted. The other team is on a counter attack. Type 1 to try to tackle the opponent with the ball. Type 2 to run back to defense.\n")
                if two_ac == 1:
                    dp("You miss the tackle and the opponent passes a long ball to their teammate. The opponent's striker controls the ball and SCORES!\n")
                    goal -= 1
                if two_ac ==2:
                    dp("You run back to defense and intercept a long pass to the striker.\n")
                    game_rating += 1
            if one_ac == 2:
                game_rating += 1
                two_ac = validation("Your pass was successful. Your teammate is now looking to cross the ball. Type 1 to shoot the ball from outside the box. Type 2 to look for a header in the box.\n")
                if two_ac == 2:
                    dp("Your shot missed the goal by a centimeter.\n")
                if two_ac == 1:
                    dp("You run in for the header and SCORE!!! Your header nestles into the net of the goal!!!\n")
                    goal += 1
                    game_rating += 1
            clear()
            one_ac = validation("You dribble past two defenders and there is only one defneder left. Type 1 to pass to a nearby teammate. Type 2 to keep dribbling.\n")
            if one_ac == 1:
                dp("Your pass was successful but the opponent's defense ran back and your attack was stopped\n")
            if one_ac == 2:
                game_rating += 1
                two_ac = validation("You dribbled past the defender and are going 1 vs. 1 against the keeper. Type 1 to chip the keeper. Type 2 to shoot to one of the top corners.\n")
                if two_ac == 1:
                    dp("The keeper easily saved your chip.\n")
                if two_ac == 2:
                    dp("GOALLL!!! Your shot banged into the top corner!\n")
                    goal += 1
                    game_rating +=1
            clear()
            one_ac = validation("The opponent is dribbling down the right side of the pitch. Type 1 to slide tackle. Type 2 to chase the player.\n")
            if one_ac == 1:
                dp("You slide tackled beautifully and stopped the attack.\n")
                game_rating += 1
            if one_ac == 2:
                dp("You weren't fast enough and the opponent sprinted away. They crossed the ball into the box and SCORE!!\n")
                goal -= 1
            clear()
            if goal == 0:
                one_ac = validation("You get a last minute penalty. Type 1 to shoot right. Type 2 to shoot left.\n")
                if one_ac == 1:
                    two_ac = validation("The keeper saved your shot. The opponent is off with the counter attack. Type 1 to shoulder tap. Type 2 to tackle.\n")
                    if two_ac == 1:
                        three_ac = validation("You successfully stop the play and have a counter attack opportunity. Type 1 to pass a short pass. Type 2 to pass a long pass.\n")
                        if three_ac == 1:
                            dp("Your short pass gets intercepted. The opponent crosses the ball. The striker goes up and SCORE. THEY SCORE A LAST MINUTE PENALTY.\n")
                            goal -=1
                        if three_ac == 2:
                            dp("Your long pass goes straight to the feet of your striker. He volleys and GOALLLL!!! HE SCORED AT THE LAST MINUTE TO WIN THE CHAMPIONS LEAGUE!!\n")
                            goal += 1
                    if two_ac == 2:
                        dp("Your tackle leads to a foul. The opponent steps up and SCORE!!! THEY SCORE IN THE LAST MINUTE\n")
                        goal -= 1
                if one_ac == 2:
                    dp("GOAL!! YOU SCORED IN THE LAST MINUTE TO WIN THE CHAMPIONS LEAGUE!!!\n")
                    goal += 1
                clear()
            if goal <= -1:
                dp("GAME OVER. You lost the Champioins League.\n")
            else:
                dp("YOU ARE NOW THE CHAMPIONS LEAGUE WINNER! CONGRATULATIONS!\n")
            trophy = '''
             ___________
            '._==_==_=_.'
            .-\:      /-.
           | (|:.     |) |
            '-|:.     |-'
              \::.    /
               '::. .'
                 ) (
               _.' '._
              `"""""""`
            '''
            print(trophy)

```
