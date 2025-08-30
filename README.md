# Experiment-3
## PRIME NUMBER OR NOT

# Aim: Write a python program to check the number is prime or not and inspect for failures. 

# Algorithm
1. Start the program.
2. Get the number to be checked from the user.
3. If the number is less than or equal to 1, return "Not Prime".
4. If the number is 2, return "Prime".
5. Start the iteration from 3, For each iteration:
 - If the number is divisible by the current iteration value, return "Not Prime".
6. If the number is not divisible by any value from 2 to the square root, return "Prime".
7. Stop the program. 

## Program
```
num = input("Enter a number: ")  
flag = 0  

if num.isnumeric():  
    z = int(num)  

    if z == 2:  
        flag = 1  
    elif z > 2:  
        for i in range(2, z // 2 + 1):  # Loop should include z//2
            if z % i == 0:  
                flag = 0  
                break  
        else:  
            flag = 1  

    if flag == 1:  
        print("Prime Number")  
    else:  
        print("Not a Prime Number")  

else:  
    print("Enter a Positive Number")
```

## Output
1.
<img width="253" height="65" alt="image" src="https://github.com/user-attachments/assets/d7036620-402e-40e6-ae59-a166ad56cb08" />

2.
<img width="376" height="101" alt="image" src="https://github.com/user-attachments/assets/4a4eaba7-0c4a-493a-8dce-3502742a565e" />

3.
<img width="447" height="90" alt="image" src="https://github.com/user-attachments/assets/32ff4dd9-d3c2-4823-938a-2c0fcbdcb7c3" />



## Result
Thus, the python program to demonstrate the working of given constructs is implemented and the output is verified successfully.
