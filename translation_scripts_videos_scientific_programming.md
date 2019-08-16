# Scripts Videos Scientific Programming

## Summary
1. How to use VSC (Marleen)
2. Variables (Simon/Mees)
3. Conditions (Martijn)
4. Loops
    * Counting/repetition (Simon)
    * Calculations (Marleen)
    * Filters (Martijn)
    * User input (Mees/Simon)
5. Lists
6. Functions
    * Declaring & Calling functions *Low priority* (Was nog een oude versie van?) (Mees/Simon)
    * Functions with a single parameter (Martijn)
    * Functions with multiple parameters (Simon)
    * Functions with lists (Marleen)
    * Calling and Passing functions to and in functions *low priority* (niet af?)

## 1. How to use Visual Studio Code

In this video I'll explain you the basics of writing a program in Visual Studio Code.

This programming environment has a lot of tools and features that help make coding comfortable, but you really only need a few of the components to get started.

Before you can start programming, you generally want to create a folder that will contain the code you're about to write. After creating that folder on your computer you can click "Open Folder" on the welcome screen of Visual Studio Code to open that folder.

You'll now find that folder and all of its contents on the left hand side of your screen. For now though, it's still empty.

By clicking the document icon you can create a new file within the folder and give it a name. For example: hello.py. 
After creating the file, it is automatically opened on the right hand side of the screen.

You can now start writing code in your new file, hello.py. Let's add the line `print("Hello Python")` and save it by holding down **control** and then pressing **s**.

To run your newly written program, you first have to open a terminal. You can do so by holding **control** and then pressing the **back tick**, usually found next to either 1 or Z on your keyboard. 

The terminal pops up from the bottom of the screen.
Your terminal can look a little different from ours.

Next, type out "python" followed by the name of the file, in our case "hello.py", and press Enter. 

And as you can see, the text "Hello Python" is printed to the screen.

You can also use the terminal to issue commands directly. 
Once again type out "python", but this time immediately hit enter afterwards. 

You've now entered the Python Interactive Shell. If you type print("Hello") and hit enter, you'll see it instantly prints "Hello" to the screen.
Besides printing, you can also perform some calculations, for example: 4 + 4.

To exit the interactive shell you can type  "exit" followed by parentheses and then hit enter.

Sometimes your terminal has opened in a different directory than where your program is located. When you then try to execute the program, you'll encounter an error: "can't open file 'hello.py'".

By running the command "pwd" you can find out in which folder the terminal is located. You can see that the terminal is in the **downloads** directory, but the file hello.py has been placed in a specific folder. 
To fix this issue you can click the right mouse button on the file hello.py and subsequently click "Open in command prompt" or "Open in terminal". 
Now you can run your program.

Oh and here's another trick.
Imagine that you adjust your program to now contain some punctuation ...
[Hello comma Python exclamation mark edit]

If you want to run your program again, you can use the arrow up key on your keyboard to cycle through previous commands in the terminal.
By clicking enter again the command is executed and your program is ran.

## 2. Variables

In this video I'll explain how you can make use of variables

Variables can be very convenient when, for example, you want to use the result from a calculation in another calculation. 
Each variable is assigned a *name* and a *value*.
~~~~You are free to choose the name of the variable yourself, but be sure to always choose a short and descriptive name~~~~

An example.
Imagine you want to calculate your income and expenses for the month.

First your income.
You receive 277 euros worth of study loan from DUO each month.
So you make a variable "study_loan", and assign it a value of 277.
You also have a part time job that nets you 500 euro per month.
So you make another variable called "job" and assign it a value of 500.
You can now calculate all of your income by adding those variables together.
The result can also be stored in a variable; "income... equals... study_loan... plus job".
And now, if you print the variable income... and run the program...
[running program]

    study_loan = 277
    job = 500
    income = study_loan + job
    print(f"Income: {income}")

... then you can see that your total income is worth 777 euros.

In that same way, you can calculate your expenses.
The rent of your room is 390 euros per month.
You're going to spend 175 euros this month on groceries and 125 euros on fun stuff. 
[short break]

So the calculation for your expenses is: "expenses... equals... rent.. plus groceries... plus fun stuff".
So your expenses for this month are...
[running program]

    study_loan = 277
    job = 500
    income = study_loan + job
    print(f"Income: {income}")

    rent = 390
    groceries = 175
    fun_stuff = 125
    expenses = rent + groceries + fun_stuff
    print(f"Expenses: {expenses}")

... 690 euros.

Now that you have both income and expenses, you can figure out how much you have left at the end of the month.
Subtract the "expenses" from the "income" and store that value in a new variable called "savings".
So: "savings... equals... income... minus... expenses".
Leaving you with:
[running program]

    study_loan = 277
    job = 500
    income = study_loan + job
    print(f"Income: {income}")

    rent = 390
    groceries = 175
    fun_stuff = 125
    expenses = rent + groceries + fun_stuff
    print(f"Expenses: {expenses}")

    savings = income - expenses
    print(f"Savings: {savings}")

... 87 euros at the end of the month.

Now that you have an oversight of all of the components that make up the formula to calculate your finances, you can easily make small changes.

Let's say you get a new job that doesn't net you 500, but 575 euros per month instead. 
You now only need to adjust your code in a single location for this change to take effect. 
More specifically... the value of the variable job needs to be changed to 575 euros. If you run the program again...
[running program]

    study_loan = 277
    job = 575
    income = study_loan + job
    print(f"Income: {income}")

    rent = 390
    groceries = 175
    fun_stuff = 125
    expenses = rent + groceries + fun_stuff
    print(f"Expenses: {expenses}")

    savings = income - expenses
    print(f"Savings: {savings}")

... you'll find that you have 162 euros left by the end of the month.

Always keep a close eye on the order in which you use your variables. Python reads them top to bottom. That means that a variable needs be declared before you can use it. 
If, for example, you had tried to print the value of "savings" at the top of the program...
[short break]
And you run the program...
[running program]

    print(f"Savings: {savings}")

    study_loan = 277
    job = 575
    income = study_loan + job
    print(f"Income: {income}")

    rent = 390
    groceries = 175
    fun_stuff = 125
    expenses = rent + groceries + fun_stuff
    print(f"Expenses: {expenses}")

    savings = income - expenses

... you'll see the error: "name 'savings' is not defined".

This is because when you try to print the value of savings at the first line, it doesn't exist yet. Not until you assign a value to that name, 'savings', only then you can use that variable.

## 3. If

In this video I'll explain the use of if-statements.

Let's say you want to create a program that checks a user's age.

The first step is to ask the user for their age. You can use the function *input* to do so: "age... equals... input... age".

The input function always returns a *string* of what the user entered.
To perform a correct age check you first need to convert this string into an integer.
This is done as follows: "age... equals... int... age".
This line only serves to change the data type of the input to an integer.
You're now done with the input.

Next you'll want to verify whether the age of the user is under 18. If this is the case, you're going to print that the user is not yet an adult. You can use an if statement to do so.
It'll look like this:
"if the age of the user is lower than 18... print... "you're not yet an adult...".

You'll also want to print something if the user is over or equal to 18 years old. This can be achieved by adding an else-statement.
So if the users' age is below 18 you print... "you're not yet an adult..." and ***else*** you print... "you're an adult!".
Let's run your program:
[running program]

    age = input("Age: ")
    age = int(age)

    if age < 18:
        print("You're not yet an adult...")
    else:
        print("You're an adult!")

If you were to enter 13 as your age...
then the program checks whether 13 is lower than 18,
which it is,
so the program then prints "you're not yet an adult",

If you run the program again...
[running program]
and you enter 21 as your age...
then the program first checks whether 21 is lower than 18...
which is *not* the case, so the program skips the code within the if statement and instead runs the code within the else statement that prints... "You're an adult!"...
... it works!

You can expand this program with more conditions.
If for example you want to also make a distinction between people older than 65,
You have to add an extra condition with an **elif**, short for **else if**.
So: "if the age is lower than 18... print.. 'You're not yet an adult...", **else if** the age is greater than or equal to 65... print.. "you're a senior!" and **else** print 'You're an adult!'.

Let's run the program...
[running program]

    age = input("Age: ")
    age = int(age)

    if age < 18:
        print("You're not yet an adult...")
    elif age >= 65:
        print("You're a senior!")
    else:
        print("You're an adult!")

Now if you enter 15 as your age...
the program prints "you're not yet an adult",
since 15 is lower than 18.

[running program]

and if you enter 71 as your age...
... then the program prints "You're a senior!"...
since 71 is greater than 65.

[running program]

and if you enter 33 as your age...
... then the program prints "You're an adult!"...
since 33 is greater than 18, but ***also*** because it is not larger or equal to 65.
Once again the program works as intended.

Finally you'll combine multiple conditions into one.
Imagine people getting a discount on your entry ticket at a museum for being ***either*** younger than 18 or older than 65.
Then the combination of conditions would look like this:
"if age is less than 18...
***OR***
if age is greater than or equal to 65...
print.. 'You get a discount for this museum!'...
***else***
print.. 'Unfortunately, you do not get a discount'...

So only one of the conditions has to be true for the message 'you get a discount' to be printed.

Let's run the program...
[running program]

    age = input("Age: ")
    age = int(age)

    if age < 18 or age >= 65:
        print("You get a discount for the museum!")
    else:
        print("Unfortunately, you do not get a discount...")

if you now enter 17 as your age...
... the program prints "You get a discount".
since 17 is less than 18.

[running program]

and if you enter 45 as your age...
... the program prints "You do not get a discount"...
because 45 is neither smaller than 18 or greater or equal to 65

[running program]

and if you finally enter 81 as your age...
... the program once again prints "You get a discount"
because 81 is greater than 65.

## 4. Loops

**Repetition**
In this video I'll explain how to use loops to **repeat** pieces of code in your program.

Let's say you want to print the numbers 1 through 10,
you could do so by coding 10 individual print statements and run them in succession.
[copy pasting print statements then running]

    print("1")
    print("2")
    print("3")
    print("4")
    print("5")
    print("6")
    print("7")
    print("8")
    print("9")
    print("10")

As you can see, the numbers 1 through 10 are printed to the terminal.
Only this is not very practical. What would happen if you wanted to print 1 through 1 thousand?
It's best to use a loop in that case.
It looks like this: "for... number... in range... 1 **till** 11... print number".
Beware that the range you provide is 1 **up to** 11, **not** 1 up to and including 11. 
If you run this program the variable *number* will first assume the value of 1.
This value is subsequently printed to the terminal.
After which the program will loop back to the first line of the 'for loop', 
and the value of the variable *number* will become 2.
Then, **that** value is printed.
These steps will be repeated until the variable *number* becomes 11, so a total of 10 times.
Let's see if this is correct...
[running program]

    for number in range(1, 11):
        print(number)


... as you can see the numbers 1 through 10 are printed.

With this loop, you can now easily print the numbers 1 through 1 thousand. 
you only need to change the 11 into 1001.
[runs program]

    for number in range(1, 1001):
        print(number)

... and indeed, the numbers 1 through 1 thousand are printed.

This way you can print any amount of numbers by only a single change.

**Calculating**
In this video I'll explain how to do **calculations** using loops.

So, how can you use a loop to add a large amount of numbers together?
For example the sum of the numbers 1 through 1 thousand.

Using this piece of code in a file called calculating.py you can print each number up to and including 1 thousand:

    for number in range(1, 1001):
        print(number)

To add all these number together, first you need a variable to store that sum. Let's call it **result** and give it an initial value of 0.
**Inside** the for loop you'll be doing the additions.
You'll want to add the value of the variable "number" to the value of the variable "result": "result = result + number"... or in short... "result += number".
Beneath the for loop you'll print the final result... and that's it.

When you run this program you'll first initialize the variable "result" with a value of 0.
Then, in the first step of your loop the variable "number" will get a value of 1 and subsequently be added to the value of the variable "result". 
The current value of "result" is 0, so 0 + 1 equals 1.
Then the program will loop back to the start of the for loop.
The value of "number" becomes 2.
Once again the value of "number" is added to the value of "result", which was 1.
So now 1 + 2 equals 3.
This will be repeated until the computer has reached the "number" 1001, at which point it will continue below the for loop and print the result.
Let's run the program...
[running program]

    result = 0
    for number in range(1, 1001):
        result += number
    
    print(result)

... as you can see the sum of the numbers 1 through 1 thousand is 500500.

With only a simple adjustment to the program, you can calculate the sum of any range of numbers.

**Filtering**

In this video I'll explain how to use loops to **filter**.

Let's say you want to print the numbers between 1 and 50 **and** only the ones that can be divided by 3.
you first need a loop that passes through each of the numbers 1 through 50: "for number.. in range.. 1... to... 51".
Subsequently you need to check if the value of each number can be divided by 3.
you can do so by using the modulo operator, which finds the remainder after division of one number by another.
So: "if the variable 'number' ... modulo 3.. equals 0... print number".
If the result of the variable 'number' .. modulo 3.. is equal to 0, that means the remainder is 0. Ergo, that number is dividable by 3 and you should print it.

If you run this program, the variable 'number' will first assume a value of 1. 
Subsequently the program checks if the value of the variable 'number' modulo 3 is 0.
For the 'number' 1 this is not true, since 1 modulo 1 equals 1, which means the number 1 is not printed.
Then the program loops back to the start of the for loop and the value of "number" becomes 2.
This number is not printed either, since the result of 2 modulo 3 is 2. 
Once again the program loops back to the start of the for loop and the value of 'number' becomes 3.
For the first time a number is printed, because 3 modulo 3 is equal to 0.
These steps are repeated until 'number' is equal to 51.
Let's run the program...
[running program]

    for number in range(1, 51):
        if number % 3 == 0:
            print(number)

... as you can see numbers such as 3, 6 and 9 are printed. Which all can be divided by 3.

With only a simple adjustment to your code, you could also filter numbers based on a different condition.

**User input**
In this video I'll explain how to use loops to request and verify user input.

You've already written a program that prompts the user for their name and afterwards prints "Hello" and that users specified name.

Let's run the program to verify it's output...
[running program]

    name = input("What is your name? ")
    print(f"Hello {name}")

... the program prompts the user for their name...
... and then prints the string 'Hello ***Mirja***', so it works!

Except if you were to run this program again...
[running program]
... and you **do not** provide a name - which you're not supposed to do - the rest of the program is **still** executed.

To make sure a user always provides a valid name, you can use a loop that repeatedly prompts a user for their name, until they **do** enter a valid name.
you **won't** be using a for loop for this, but instead you use a while loop. 
you do so because you do not know ahead of times how often you'll have to prompt the user for a valid name.

SO: "while name... is equal to... an empty string... prompt the user for their name".
Now the program will request the user to provide their name, for as long as name is an empty string.
Let's run the program...
[running program]

    name = input("What is your name? ")

    while name == "":
        name = input("What is your name? ")

    print(f"Hello {name}")

Now, if you do not enter anything as your name, the program will keep prompting you to provide a name.
[press enter a couple of times]
And if you do type out your name and press enter, it prints, just like before, "hello ***Mirja***".

## 5. Lists

In this video I'll explain how to make effective use of Python lists.

Lists are useful to group data and to subsequently process that data as a whole.
A list can contain individual numbers, but also strings or characters. 
Think of a list of prime numbers, or a list of the names of your classmates. 
It's even possible to store lists within lists.

For now, I've created a shopping list with five items:
milk, rice, cucumber, oatmeal and bread.
you can print this entire list by executing "print groceries"...
[running program]

    groceries = ["milk", "rice", "cucumber", "oatmeal", "bread"]
    print(groceries)

... and as you can see the entire list is printed to the terminal.

you can also retrieve and print only one element from your list.
To do so you need the ***position*** of that element, also known as its ***index***.
If you want to know what the third element in your list is,
you can get that element the following way: "print... groceries... two".
Because Python starts indexing elements from the number 0...
"print groceries two" will print the third element of a list.

Let's verify this...
[running program]

    groceries = ["milk", "rice", "cucumber", "oatmeal", "bread"]
    print(groceries[2])

... and unsurprisingly the third element is printed.

you can also change elements within a list.
It can be done in the following way: "groceries... two.. equals... lettuce"
When you run the program...
[running program]

    groceries = ["milk", "rice", "cucumber", "oatmeal", "bread"]
    groceries[2] = "lettuce"
    print(groceries)

... you see that indeed the third element of the list has been changed to lettuce.

Besides changing existing elements, you can also add new elements to a list.
Cheese for example, can be added by first typing the name of your list... then a point... then append... and finally "cheese".

Let's print the shopping list to verify:
[running program]

    groceries = ["milk", "rice", "cucumber", "oatmeal", "bread"]
    groceries[2] = "lettuce"
    groceries.append("cheese")
    print(groceries)

... this time the list is one element larger and now contains cheese.

Finally, it is also possible to use a list within a loop, for example if you want to print each element in a list on separate lines. 
Like this:
"for each item in groceries... print item".

If you run this...
[running program]

    groceries = ["milk", "rice", "cucumber", "oatmeal", "bread"]
    
    for item in groceries:
        print(item)

... all the elements of the list are printed clearly on each line.

## 6. Functions

**Declaring and calling functions**
In this video I'll explain how to declare functions and later call them.

If you need a specific piece of code multiple times in your program, then you can move that code to a function so that you can call it where ever and when ever you need it.
This way you prevent yourself from repeating bits of code and it helps you keep your code comprehensive and readable.

Python comes with a lot of functions included, "len", for example, is a function that is used to determine the length of a list...
or the function "round", which is used to round a number in a mathematically correct way.

Aside from these inbuilt functions, you can also write your own functions in Python.
Imagine having wrote a program that...

You start out a function with the word "def" followed by the name of the function, which you can choose yourself. 
Choose a name that is short, descriptive and unique, so that it is instantly clear what your function is supposed to do and that it does not conflict with other code.
Indented is WITHIN the function, else you write code outside of the function.
You end this line with parentheses and a colon.
[write and run function -> nothing happens]
function has to be called
You practically use the name of the function, but don't need to add all the corresponding code.
That is already included in the definition.

**Functions with one parameter**
In this video I'll explain how to write functions with one parameter.

~~~~
We write a function that calculates the square of a random number. 
We first declare the function by writing down "def",
followed by the name of the function, in this case "squared".
The function has only one parameter, that we'll call "x".
~~~~
The contents of the functions is kept simple: 
the result is X multiplied by X... or: "return x... times... x".

To test it, we call the function immediately: "print squared"...
and run the program...
[running program]


    def squared(x):
        return x * x
            
    print(squared())

As you can see we get an error: "missing 1 required positional argument: 'x'" 
This happens because in our test the function wasn't passed any parameter,
even though the function does need one,
specifically the number of which we want to know the square.
So let's put the number 3 at the location of the parameter.
Now the square is calculated of the number 3 and printed to the terminal...

[running program]


    def squared(x):
        return x * x
            
    print(squared(3))

... which is correct.

We can also pass a variable as a parameter to the function.
We define the variable "number" and give it the value 12.
If we pass on the variable 'number', when we call the function,
then the parameter 'x' will assume the value of the variable 'number', which is 12.

Let's run the program...
[running program]


    def squared(x):
        return x * x
            
    number = 12
    print(squared(number))

... and indeed, 144 is printed to the screen.

**Functions with multiple variables**
In this video I'll explain how to use functions with multiple variables.

We write a function that compares two numbers with each other and returns the *largest* number.
You define a function with "def" and give it a name, for example "largest_of".
The function has two parameters, both of the numbers that you wish to compare: a and b.
You'll first want to check whether parameter "a" is larger than "b",
so: "if a is larger than b".
If this is the case, than you'll want to return that parameter.
And else you'll want to return "b".

    def largest_of(a, b):
        if a > b:
            return a
        else:
            return b

Now you have to test the function.
First, we create two variables, "number_1" and "number_2",
and we give both a value.
To call the function "largest_of", we pass the variables "number_1" and "number_2" as parameters.

If you run this program, parameter 'a' will assume the value of 'number_1', which is 126.
The parameter 'b' will assume the value of 'number_2', which is 14.
Then the function verifies whether parameter 'a' is larger than parameter 'b'.
And finally, parameter 'a' is returned and then printed.

Let's run the program...
[running program]

    def largest_of(a, b):
        if a > b:
            return a
        else:
            return b
    
    number_1 = 126
    number_2 = 14
    print(largest_of(number_1, number_2))

... and indeed, the number 126 is printed.

**Functions with lists**
In this video I'll explain how to use lists in your functions.

We write a functions that takes a list of x-values and returns a list in which for each x-value the corresponding y-value has been calculated.

For example the following list... 'positions'

    # f(x) = x * *
    positions = [1, 2, 3, 4, 5, 6]

We define a function and give it the name "list_squared"
with one parameter "x_coords".

Now we need a list to collect all the results before we can return it.
"y_coords.. is.. an empty list".
Next we loop over the list of x_values: "for each x... in the list... with x-coordinates".
Then we calculate the y-value with our functions x... times x...
and the results are appended to the list y_coords.
If all calculations have been done and the list is completed, we return that list.

To test the function we use the list 'positions' that we've created earlier. Then we call our functions list_squared with the variable positions as argument.

Let's run the program...
[running program]

    def list_squared(x_coords):
        y_coords = []
        for x in x_coords:
            y_coords.append(x * x)

        return y_coords

    positions = [1, 2, 3, 4, 5, 6]
    values = list_squared(positions)

    print(values)

... and as you can see the list is printed with the square of each number in x_coords.

The lists could be used together to plot a graph of x-squared.

**Functions that call functions & passing functions to functions**
In this video I'll explain how to call a function from another function and also how to pass a function as parameter to another function.

Let's write a program that calculates the minimum of a mathematical function, for example "x squared", for a certain range.
We've written the function for x-squared before

    def squared(x):
        return x * x

To calculate the minimum, we're going to write another separate function.
... called "minimum"
This function takes two parameters: the lower bound and the upper bound of the area in which we're going to find the minimum.

**In** the function we'll initialize the variable "minimum_value".
A good starting value for the minimum_value is the value of the function at the lower bound.
We call the function "squared", that we've already written: "minimum_value... equals... squared...lower_bound".
That means you pass the lower_bound as the parameter to the function squared.
Subsequently the function squared returns the square of the lower_bound...
and this result is stored in the variable "minimum_value".

THen you start to loop over the specified range, finding the minimum value:
"for x... in range... lower_bound plus 1... upper_bound plus 1".
You start at the lower bound **plus 1**, since we've already stored the value of the square of the lower bound in the variable minimum_value.

X will start the loop with a value of lower_bound plus 1.
Then you'll want to check whether the square of x is lower than the value currently stored in 'minimum_value'.
If that is the case, than the 'minimum_value' needs to be assigned the value of x squared.
So: "if the result of the function 'squared' is lower than the variable 'minimum_value',
assign the result of 'squared' to the variable 'minimum_value'".
Once again we call teh function 'squared' that we've written before and this time we pass x as its parameter.
When the loop is finished, you can complete the function by returning the 'minimum_value' found: "return minimum_value".

Finally you call the function "minimum" and print its result: "print(minimum(lower_bound, upper_bound))".
The lower bound and upper bound could, for example, be -100 and 100 respectively.

Let's run the program...
[running program]

    def squared(x):
        return x * x

    def minimum(lower_bound, upper_bound):
        minimum_value = squared(lower_bound)

        for x in range(lower_bound + 1, upper_bound):
            if squared(x) < minimum_value:
                minimum_value = squared(x)
        
        return minimum_value

    print(minimum(-100, 100))

... and as you can see the minimum of the function "x squared" within the range of -100 and 100 is equal to 0.

If we would want to find the minimum of a different function, we could write a new minimum function, but that would be very awkward.
Instead we could pass the function of which we want to know the minimum as a parameter and call that function where we now always call 'squared'.
That means you'll have to add the parameter func to the function.
Then, you'll have to change all calls to 'squared' within 'minimum' with calls to 'func', because that parameter 'func' is now the function of which you want to calculate the minimum.
[short break]
Finally, when you call the function minimum, you now have to pass which function you want to know the minimum of, in this case it's still the function squared.

If we run the program...
[running program]

    def squared(x):
        return x * x

    def minimum(func, lower_bound, upper_bound):
        minimum_value = func(lower_bound)

        for x in range(lower_bound + 1, upper_bound):
            if func(x) < minimum_value:
                minimum_value = func(x)
        
        return minimum_value

    print(minimum(squared, -100, 100))

... you can then see that again the value 0 is printed.

To now change the function of which you want to know the minimum...
for example "x to the power of 3"...
we simply have to add a function:
"def power_of_three... x... return... x... power of... three".
And when we call the minimum function, instead of passing squared, you now pass the function "power_of_three".

Let's run the program...
[running program]

    def squared(x):
        return x * x

    def power_of_three(x):
        return x * x * x

    def minimum(func, lower_bound, upper_bound):
        minimum_value = func(lower_bound)

        for x in range(lower_bound + 1, upper_bound):
            if func(x) < minimum_value:
                minimum_value = func(x)
        
        return minimum_value

    print(minimum(power_of_three, -100, 100))

... and as you can see the minimum of the function x to the power of three within the range -100 and 100 is equal to -1.000.000. 