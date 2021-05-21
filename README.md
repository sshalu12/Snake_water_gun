# Snake_water_gun
import random
i=9
print("choice : ")
print("s for snake ")
print("w for water ")
print("g for gun ")
c1=0
u1=0
while(i>0):
    
    lst=["s","w","g"]
    ch=random.choice(lst)
    i=i-1
    ch1=input("Enter your choice : ")
    
    if(ch=="s" and ch1=="w" ) :
        print("computer choosed snake , opponent wins!")
        c1=c1+1
    elif(ch=="s" and ch1=="g"):
        print("computer choosed snake , you win!")
        u1=u1+1
    elif(ch=="w" and ch1=="s"):
        print("computer choosed water , you win!")
        u1=u1+1
    elif(ch=="w" and ch1=="g"):
        print("computer choosed water , opponent wins!")
        c1=c1+1
    elif(ch=="g" and ch1=="s"):
        print("computer choosed gun , opponent wins!")
        c1=c1+1
    elif(ch=="g" and ch1=="w"):
        print("computer choosed gun , you win!")
        u1=u1+1
    else:
        print("same choice, draw!")
if(c1>u1):
    print("computer won",c1,"times , so opponent wins !")
elif(c1==u1):
    print("you both won",c1,"times")
else:
    print("you won",c1,"times , so you wins !")
