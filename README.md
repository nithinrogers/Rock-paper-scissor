import random

while True:
    p = input("Enter a choice (rock, paper, scissors): ")
    n = ["rock", "paper", "scissors"]
    m = random.choice(n)
    print(f"\nYou chose {p}, computer chose {m}.\n")

    if p == m:
        print(f"Both players selected {p}. It's a tie!")
    elif p == "rock":
        if m == "scissors":
            print("Rock smashes scissors! You win!")
        else:
            print("Paper covers rock! You lose.")
    elif p == "paper":
        if m == "rock":
            print("Paper covers rock! You win!")
        else:
            print("Scissors cuts paper! You lose.")
    elif p == "scissors":
        if m == "paper":
            print("Scissors cuts paper! You win!")
        else:
            print("Rock smashes scissors! You lose.")

    play = input("Wanna Play again? (y/n): ")
    if play.lower() != "y":
        break
