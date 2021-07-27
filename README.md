print("You have 10 LIFES in this game\n","You entered a STONNE PAPER SCISSOR Gam\n")
import random
l= ["stone","paper","scissor"]
while(1):

        d=0
        e=0
        b=1
        while(b<12,d<b,e<b):
            b=b+1
            if b==12:
                print("LIFES COMPLETED\n\n")
                break
            c = random.choice(l)
            a = input("\n\n\nYour Turn Enter\n\t s--for Stone\n\t p--for Paper\n\t sc--for Scissor:\n")
            if c=="stone":
                if a=="s":
                    print("\nNO ONE WIN\n"),         print("Lifes Remained--",11-b)
                elif a=="p":
                    d=d+1
                    print("\nCOMPUTER IS A WINNER\n"),      print("Lifes Remained--",11-b),     print("\nCOMPUTER SCORE--",d)

                elif a=="sc":
                    e=e+1
                    print("\nYOU WON\n"),      print("Lifes Remained--",11-b),    print("\nYOUR SCORE--",e)

                    continue
            elif c == "paper":
                if a == "p":
                    print("\nNO ONE WIN\n"), print("Lifes Remained--", 11-b)
                elif a == "sc":
                    d=d+1
                    print("\nCOMPUTER IS A WINNER\n"), print("Lifes Remained--",11-b),print("\nCOMPUTER SCORE--\n",d)

                elif a == "s":
                    e=e+1
                    print("\nYOU WON\n"), print("Lifes Remained--",11-b),print("\nYOUR SCORE--",e)

                    continue
            elif c == "scissor":
                if a == "sc":
                    print("\nNO ONE WIN\n"), print("Lifes Remained--",11-b)
                elif a == "":
                    d=d+1
                    print("\nCOMPUTER IS A WINNER\n"), print("Lifes Remained--",11-b), print("\nCOMPUTER SCORE--",d)

                elif a == "s":
                    e=e+1
                    print("\nYOU WON\n"), print("Lifes Remained--",11-b), print("\nYOUR SCORE--",e)

                    continue
        if d>e:
                print("\t\tCOMPUTER IS WINNER\n","\nTotal points Computer gained:  ",d), print("\n\t\tYOU ARE LOSER","\nTotal points You gained:  ",e)
        elif d<e:
                print("\t\tYOU ARE WINNER\n","\nTotal points You gained:",e), print("\n\t\tCOMPUTER IS LOSER","\nTotal points Computer gained:  ",d)
        else:
                print("\n\nRESTART GAME,NO ONE WON\n\n\n")
        k = input("\n\nEnter R for RESTARTING GAME or Q for OUIT game:")
        if(k=="r" or k=="R"):
            print("\nRESTARTING GAME\n")
            continue
        elif(k=="q" or k=="Q"):
            print("\nQUIT GAME\n")
            break
