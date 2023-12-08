So far, we've learned how to create Python files, write Python expressions and statements and execute them. However, all the programs we wrote up to this point have been linear — all the instructions were executed line by line. That's not how a program usually works in real life scenarios.

The real power of programming is giving computers the ability to choose specific instructions to execute and others to skip or "jump", based on conditions we supply as programmers.

## So, What Is Control Flow?

Control flow is the order in which statements are executed in a program. It determines the path that the program takes based on conditions and decisions. In programming languages like Python, control flow is managed through structures like conditionals (if statements), loops, and function calls.

To understand control flow, let's look at a few examples.

Imagine you need to do some operation on your bank account via ATM. You head to the ATM, insert your card, enter your security PIN and you are presented with a few options to choose from. Suppose the options are as follows:

1. Withdraw
2. Deposit
3. Balance Inquiry
4. Charity/Donation
5. Cancel

Based on the option you choose, the ATM will display a different screen with a different view.

Another example is when you register an account on a website. Usually, you are asked to enter your username, password and password confirmation. Assume that the minimum password length is 8 characters.

When you supply your information, the program checks if this information meets the criteria. If the password you supplied is less than 8 characters long, the registration won't proceed and you will get an error. Otherwise, the registration will be completed successfully.

Your choice at the ATM in the first example and the minimum password length requirement in the second example are known as "conditions". If these conditions are fulfilled, the program will take a specified route. If not fulfilled, the program will take an alternate route. Hence, the flow of the program is "controlled" based on these conditions.

In the next concept, we'll learn how to graphically represent control flow of a program.