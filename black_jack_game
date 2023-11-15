import random
def deal_card():
    """"Returns a random card from the list or lot of cards"""
    cards=[11,2,3,4,5,6,7,8,9,10,10,10,10]
    card=random.choice
    return card

def calculate_score(cards):
    """this function takes a list of cards and returns the score 
    calulated from the cards"""

    if sum(cards)==21 and len(cards)==2:
        return 0
    if 11 in cards and sum(cards)>21:
        cards.remove(11)
        cards.append(1)
    
    return sum(cards)

def compare(user_score,computer_score):
    if user_score==computer_score:
        return "draw"
    elif computer_score==0:
        return "win with a blakc jack"
    elif user_score >21:
        return "you scored over the limit you loose unfortunately"
    elif computer_score >21:
        return "opponet went over 21 you win"
    elif user_score>computer_score:
        return "you win"
    else:
        return "you loose"
def play_game():  
    user_cards=[]
    computer_cards=[]
    is_game_over=False

for _ in range(2):
    user_cards.append(deal_card())
    computer_cards.append(deal_card())

while not  is_game_over:

    user_score=calculate_score(user_cards)
    computer_score=calculate_score(computer_cards)
    print(f"your cards:{user_score},current scoe:{user_score}")
    print(f"Computers first card:{computer_cards[0]} ")

    if user_score==0 or computer_score==0 or user_score>21:
        is_game_over=True
    else:
        user_deal=input("type Yes to get another card, type no to pass ")
    if user_deal=="Yes":
        user_cards.append(deal_card())
    else:
        is_game_over=True

while computer_score !=0 and computer_score<17:
    computer_cards.apppend(deal_card())
    computer_score=calculate_score(computer_cards)

print(f"your final hand:{user_cards},final score:{user_score}")
print(f"computers final hand:{computer_cards},final score:{computer_score}")
print(compare(user_score,computer_score))

while input("do you want to play the game again type yes if not type no")== "yes":
    play_game()

   
   


       
       
    

