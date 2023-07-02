from random import randint

print("nhap keo, bua, bao:")
player = input()
computer = randint(0,2)

if computer == 0:
    computer = "Bua"
if computer == 1:
    computer = "Bao"
if computer == 2:
    computer = "Keo"

print("---")
print("You choose: " + player)
print("Computer chooses: " + computer)
print("---")

if player == computer:
    print("Hoa")
else:
    if player == "Keo":
        if computer == "Bua":
            print("Thua")
        else:
            print("Thang")
 
    if player == "Bua":
        if computer == "Keo":
            print("Thang")
        else:
            print("Thua")

    if player == "Bao":
        if computer == "Keo":
            print("Thua")
        else:
            print("Thang")
    else:
        print("Nhap sai!")
