# Intro-to-CS50-Lab-2-
point = []
ply1sum = 0
ply2sum = 0
point = [1,3,3,2,1,4,2,4,1,8,5,1,3,1,1,3,10,1,1,1,1,4,4,8,4,10]

#coverting characters to integers
ply1 = (input("Player 1: "))
ply1 = ply1.lower()
output1 = []
for character in ply1:
    number = ord(character) - 97
    output1.append(number)
    
ply2 = (input("Player 2: "))
ply2 = ply2.lower()
output2 = []
for character in ply2:
    number = ord(character) - 97
    output2.append(number)

#Referencing the corresponding character index to the points array
for i in range(0,len(output1)):
    sum1 = point[i]
    ply1sum = sum1 + ply1sum
    
for i in range(0,len(output2)):
    sum2 = point[i]
    ply2sum = sum2 + ply2sum
    
#logic to determine who wins
if ply1sum>ply2sum:
    print("Player 1 wins!")
else:
    print("Player 2 wins!")
    
