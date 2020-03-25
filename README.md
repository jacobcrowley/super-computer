
from alien_module import *

def super_computer():
    print("\nINPUT PASSWORD")
    print("==============")
    password_attempt = input(">>> ")

    active = True
    password = "password"

    while active == True:
        if password_attempt != password:
            print("\nPASSWORD INCORRECT! INTRUDER DETECTED!")
            print("======================================")
            break
        else:
            print("\nGREETINGS MASTER. INPUT COMMAND")
            print("===============================")
            command = input(">>> ")

            if command == "kill all humans":
                print("\nKILLING ALL HUMANS")
                print("==================")
            elif command == "what are the commands":
                print(
                    "\nTHE COMMANDS ARE: \n>KILL ALL HUMANS \n>INVITE ALIEN OVERLORD TO EARTH \n>RESTART \n>SHUT DOWN")
            elif command == "shut down":
                print("\nSHUTTING DOWN")
                print("-------------")
                break
            elif command == "restart":
                print("\nRESTARTING")
                print("==========")
                super_computer()
            elif command == "invite alien overlord to earth":
                make_hash_alien()
            else:
                print(
                    "\nCOMMAND NOT RECOGNISED, FOR LIST OF COMMANDS, INPUT, WHAT ARE THE COMMANDS")
                print("==========================================================================")
