
play_again = "y"

while play_again.lower() == "y":
    scoore = 0
    print("scoore equal 1 you win scoore eual 0 you lost")
    print("The available biomes are: sand, forest, water, ice")
    choice = input("What do you want to choose? 1- Sand 2- Forest 3- Water 4- Ice. Choose number: ")

    if choice == "1":
        print("You are going to fight the Sand Guardian")
        action = input("What do you do? 1- Use sword 2- Use random item. Choose 1 or 2: ")
        
        if action == "1":
            print("The sword worked well but he still didn't die. You died.")
        
        elif action == "2":
            print("It worked! Your random item was a spell book — you turned him into a frog.")
            scoore += 1
        else:
            print("Invalid action. You lose.")

    elif choice == "2":
        print("You are going to fight the Forest Guardian")
        action = input("He is going to throw a tree at you. To survive, choose: 1- Run away 2- Use shield: ")
        
        if action == "1":
            print("You were fast! You survived. Good run, don't look around and don't stop.")
            scoore += 1
        elif action == "2":
            print("The shield cracked. You died.")
        else:
            print("Invalid action. You lose.")

    elif choice == "3":
        print("You are drowning in water")
        action = input("You can't breathe underwater! Choose a way to survive: 1- Breathable face cover 2- Go to the roof: ")
        
        if action == "1":
            print("It worked! You survived.")
            scoore += 1
        elif action == "2":
            print("You died before you reached the roof.")
        else:
            print("Invalid action. You lose.")

    elif choice == "4":
        print("You are frozen!")
        action = input("To break the ice around you: 1- Use axe 2- Ignite a fire: ")
        
        if action == "1":
            print("The ice broke! You survived.")
            scoore += 1
        elif action == "2":
            print("You can't ignite a fire in ice! You froze until you died.")
        else:
            print("Invalid action. You lose.")
        
    else:
        print("Invalid biome choice.")

    print("Your final score is:", scoore)
    
    play_again = input("Do you want to play again? (y/n): ")

print("Thanks for playing Goodbye")

