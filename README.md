# project2
# Menu-Driven Python Utility Program

A console-based Python application that provides pattern printing, numerical range evaluation, and sum calculations through an interactive menu.

---

## Features

* **Pattern Generator (Option 1):** Generates a right-angled triangle pattern made of asterisks (`*`) based on the user's chosen line height.
* **Range Analysis & Summation (Option 2):** 
  * Accepts a starting integer (`n1`) and an ending integer (`n2`).
  * Iterates across the entire interval to classify each number as Even or Odd.
  * Computes and prints the cumulative sum of all numbers in the specified range.
* **Exit Program (Option 3):** Terminates the infinite execution loop.

---
while True:
    print('''Seelct an option 
            1.Generate a pattern
            2.Analyze the range of number
            3.Exit''')

    
    choice=int(input("enter your choice") )
    if(choice==1):
        n=int(input("enter range of pattern"))
        for i in range(1,n+1):
            for j in range(0,i):
                print("*",end="")
            print()


    if(choice ==2):
        n1=int(input("enter strat of the range"))
        n2=int(input("enter end of the range"))

        for i in range(n1,n2+1):
            if(n%2==0):
                print(f"no {i} is Even")
            else:
                print(f"no {2} is odd")

        sum=0
        for i in range(n1,n2+1):
            sum+=i
        print("sum of all number ",sum)

        
    if(choice==3):
        print("existing the program......")
        break


    if choice == 3:
        print("Exiting the program......")
        break
