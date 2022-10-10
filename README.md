# project-file
# Welcome massage.
print("Welcome To The Voting Center")

# Nominee info. You can also add more than 2 nominee.
nominee1 = input("Enter the nominee 1 name : ")
nominee2 = input("Enter the nominee 2 name : ")
nominee3 = input("Enter the nominee 3 name : ")
nominee4 = input("Enter the nominee 4 name : ")
nominee5 = input("Enter the nominee 5 name : ")
# Initial value of there vote must be 0 for both.
nominee1Votes = 0
nominee2Votes = 0
nominee3Votes = 0
nominee4Votes = 0
nominee5Votes = 0

# Voter id to detect fake voters.
voterId = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
numberOfVoters = len(voterId)

# main loop( we are using while loop).
while True:

    # To check voter list is completed or become empty.
    if voterId == []:
        print("Voting session is over !!!")
        if nominee1Votes > nominee2Votes:
            # To calculate the percentage.
            percent = (nominee1Votes/numberOfVoters)*100
            print(f"{nominee1} has won the election with {percent} %.")
            # to break the loop and exit the program.
            break
        elif nominee1Votes > nominee3Votes:
            # To calculate the percentage.
            percent = (nominee1Votes/numberOfVoters)*100
            print(f"{nominee1} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee1Votes > nominee4Votes:
            # To calculate the percentage.
            percent = (nominee1Votes/numberOfVoters)*100
            print(f"{nominee1} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee1Votes > nominee5Votes:
            # To calculate the percentage.
            percent = (nominee1Votes/numberOfVoters)*100
            print(f"{nominee1} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee2Votes > nominee1Votes:
            # To calculate the percentage.
            percent = (nominee2Votes/numberOfVoters)*100
            print(f"{nominee2} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee2Votes > nominee3Votes:
            # To calculate the percentage.
            percent = (nominee2Votes/numberOfVoters)*100
            print(f"{nominee2} has won the election with {percent} %.") 
          # to break the loop and exit the program.
            break
        elif nominee2Votes > nominee4Votes:
            # To calculate the percentage.
            percent = (nominee2Votes/numberOfVoters)*100
            print(f"{nominee2} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee2Votes > nominee5Votes:
            # To calculate the percentage.
            percent = (nominee2Votes/numberOfVoters)*100
            print(f"{nominee2} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee3Votes > nominee1Votes:
            # To calculate the percentage.
            percent = (nominee3Votes/numberOfVoters)*100
            print(f"{nominee3} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee3Votes > nominee2Votes:
            # To calculate the percentage.
            percent = (nominee3Votes/numberOfVoters)*100
            print(f"{nominee3} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee3Votes > nominee4Votes:
            # To calculate the percentage.
            percent = (nominee3Votes/numberOfVoters)*100
            print(f"{nominee3} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee3Votes > nominee5Votes:
            # To calculate the percentage.
            percent = (nominee3Votes/numberOfVoters)*100
            print(f"{nominee3} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee4Votes > nominee1Votes:
            # To calculate the percentage.
            percent = (nominee4Votes/numberOfVoters)*100
            print(f"{nominee4} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee4Votes > nominee2Votes:
            # To calculate the percentage.
            percent = (nominee4Votes/numberOfVoters)*100
            print(f"{nominee4} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee4Votes > nominee3Votes:
            # To calculate the percentage.
            percent = (nominee4Votes/numberOfVoters)*100
            print(f"{nominee4} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee4Votes > nominee5Votes:
            # To calculate the percentage.
            percent = (nominee4Votes/numberOfVoters)*100
            print(f"{nominee4} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee5Votes > nominee1Votes:
            # To calculate the percentage.
            percent = (nominee5Votes/numberOfVoters)*100
            print(f"{nominee5} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee5Votes > nominee2Votes:
            # To calculate the percentage.
            percent = (nominee5Votes/numberOfVoters)*100
            print(f"{nominee5} has won the election with {percent} %.") 
          # to break the loop and exit the program.
            break
        elif nominee5Votes > nominee3Votes:
            # To calculate the percentage.
            percent = (nominee5Votes/numberOfVoters)*100
            print(f"{nominee5} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        elif nominee5Votes > nominee4Votes:
            # To calculate the percentage.
            percent = (nominee5Votes/numberOfVoters)*100
            print(f"{nominee5} has won the election with {percent} %.")
          # to break the loop and exit the program.
            break
        # if they got equal votes.
        else:
            print("Both have got equal number of votes !! Heigher authority will decide the final result, Thankyou !!")
            # to break the loop and exit the program.
            break
    
    # For taking voter id
    voterIdDetection = int(input("Enter your voter id : "))
    # for detecting fake voters vs real voters.
    if voterIdDetection in voterId:
        print("You are a genuine voter ")
        # we will remove voterId so that same voter can't vote again.
        voterId.remove(voterIdDetection)
        print("______________________________________")
        print(f"To give a vote to {nominee1} Press 1 : ")
        print(f"To give a vote to {nominee2} Press 2 : ")
        print(f"To give a vote to {nominee3} Press 3 : ")
        print(f"To give a vote to {nominee4} Press 4 : ")
        print(f"To give a vote to {nominee5} Press 5 : ")
        print("______________________________________")
        # checking voter votes whom.
        vote = int(input("Enter your precious vote : "))
        if vote == 1:
            nominee1Votes += 1
            print(f"{nominee1}, Thanks you to give me your important vote !! ")
        elif vote == 2:
            nominee2Votes += 1
            print(f"{nominee2}, Thanks you to give me your important vote !! ")
        elif vote == 3:
            nominee3Votes += 1
            print(f"{nominee3}, Thanks you to give me your important vote !! ")
        elif vote == 4:
            nominee4Votes += 1
            print(f"{nominee4}, Thanks you to give me your important vote !! ")
        elif vote == 5:
            nominee5Votes += 1
            print(f"{nominee5}, Thanks you to give me your important vote !! ")
        elif vote > 5:
            print("Check your presed key is it right or wrong !!")
        else:
            print("You are not a genuine voter OR You have already voted ")
    else:
        print("You are not a genuine voter OR You have entered wrong Voter ID , else you already give your precious vote.")

# Goodbye massage.
print(" Thanks for giving your valuable time and vote.")
