Variables are named locations in memory you use to store things.

To declare a variable, you have to know what type of value are you wanting to store, and what to you want to call it. 


TASK 0:

  Inspect the code provided in Main.java.  Lines 4 and 12 are simple display lines. On line 7 a variable called age of type integer is created.  On line 8, the age variable is initialized with a value of 7. 

  The value stored in age is concatenated with the String "Age: " on Line 10 and displayed.


Task 1:

  Swap lines 7 and 8
  
  age = 7;
  int age;

  and run the program.
  
  You should have received the following error:

  Main.java:7: error: cannot find symbol
    age = 7;
    ^
  symbol:   variable age
  location: class Main

  The symbol age does not yet mean anything to the program because the program is read from top to bottom during compilation and in our code the variable declaration comes after we assigned age the value 7.
  
  Which leads us to the first rule of variables: 

  The rule: Variables must be declared before you can use them.

  Swap lines 7 and 8 again so that the program will again run without errors.
  

TASK 2:

  Change the name of the variable on line 7 to 

  int Age;

  and run the program.

  Notice that we receive a very similar error message to the one we received above.

  Main.java:8: error: cannot find symbol
    age = 7;
    ^
  symbol:   variable age
  location: class Main

  The reason is that Java sees a difference between age and Age.  
  
  Variable names in Java are case sensitive.

  Change line 7 back and confirm that the program will again run without errors.


TASK 3:

  Change the code on line 7 so that age is both declared and initialized in one step

  int age = 7;

  and then run the program. 

  The program should run and again display the value we stored in age.

  Variables may be declared and initialized either on separate lines or on one line. Which method is better? It is up to you as the programmer. 


TASK 4:

  Change the variable name for age to try and notice what happens....

  Main.java:7: error: not a statement
    int try = 7;
    ^

  Java has keywords that it uses.  You cannot declare your variables any of these keywords.  How do you know if you are using a keyword?  Keywords are colored blue in Replit.

  The rule: Variables cannot be what are called reserved words. 

  Change line 7 back and confirm that the program will again run without errors.


TASK 5:

  Change the variable from age to x in both line 7 and line 9.

  Notice the program will run, but the code has lost some readability. 

  The convention: Variable names should be short yet meaningful and descriptive. They should provide a sense of what it is you are storing/representing. One-character variable names should be avoided except for temporary "throwaway" variables.


Task 6:

  Try each of these variable names for age.  (Don't forget to change the variable in line 9 as well, or comment the line out, for this step.)
  
  int _age = 7;

  int AGE = 7;

  int 7age = 7;

  int $age = 7;

  int Age = 7;

  int aGe = 7;

  int age7 = 7;

  int #Age = 7;

  int my age = 7;

  int myAge = 7;

  Which ones worked and which ones did not?  Why?

  The rule: Variable names must be composed of letters, digits, underscores (_), and dollar signs ($), and cannot begin with a digit.

  The convention: Variable names should not start with underscore _ or dollar sign $ characters, even though both are allowed.

  Multiple words convention: Variables names cannot contain spaces, so the convention is to use camelCase, like myAge, to distinguish between different words in the variable name. The capital letters also make the variable name easier.

  All caps convention: Variable names written in all caps are extremely easy to see, so they are reserved for special variables called constants. 
  
  Change line 7 back and confirm that the program will again run without errors.

  
TASK 7:

  Let's change the value of age from 7 to 10. 
  
  Copy line 7 onto line 8 but change the value to 10. Then run the program.

  int age = 7;
  int age = 10;

  Whoops! You should have received the following error:

    Main.java:8: error: variable age is already defined in method main(String[])
    int age = 10;
        ^
  
  The error message directs us to Line 8 and tells us that age has already been defined.
  
  You only declare a variable once in Java.  To change the value of the variable, call the variable and assign it a new value. 

  Change Line 8 to 

  age = 10;

  and rerun the program.

  This time, you see the output has changed to show the new value of age, which is 10.
