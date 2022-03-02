# Arithmetic Game - Android Kotlin

When the application starts, it presents the user with 2 buttons labelled New Game, and About.
Clicking on the About button, it shows plagiarism alert message.

Clicking on the New Game button, the user will be presented with the game screen which they interact with. The screen displays 2 random arithmetic expressions one on the left and one on the right and 3 buttons below them. Each of the 2 arithmetic expressions involves 1, 2, 3 or 4 terms and it should be random (i.e. not hardcoded, or fixed, neither for the terms nor for the operations). Every time the game screen reappears, the user is displayed with 2 new diferent arithmetic expressions. The 2 arithmetic expressions could be of diferent lengths, e.g. the left could have 2 terms and the right one 3 terms. The next time that a new game screen appears to the user the left expression might involve 4 terms and the right expression 2 terms.

The operations allowed between terms are addition (+), subtraction (-), multiplication (*) and division (/).
The range of the random numbers (the random numbers are generated dynamically based on a a random generator) should be in the between 1 and 20 inclusive.
Both the terms and the operations must be  random and  diferent every  time that the user is presented with a new game screen.

The user needs to indicate whether the evaluation of the expression on the left is greater than, equal or less than the evaluation of the right expression, by pressing the buttons Greater, == or Less respectively.

The order of evaluation is always left to right and this is indicated by “compulsory” parentheses if the arithmetic expression involves more than 2 terms (i.e. 3 or 4 terms). An expression with 1 or 2 terms should NOT have any parentheses.
Examples of valid arithmetic expressions are:

2*3 (6+4)/2
((10-2)*3)/4

Examples of invalid arithmetic expressions are:

(2*3)	no parentheses for 2 terms, i.e. should be 2*3
6+(4/2) parentheses should be placed from left to right, i.e. should be (6+4)/2 (10-2)*3/4	parentheses are missing, i.e. should be ((10-2)*3)/4

As soon as the user submits the answer, the message CORRECT! (in green colour) or the message WRONG! (in red colour) appears on the screen.

Once the user submits an answer, the application displays 2 diferent random arithmetic expressions and the user can interact with the game again.

Modify the application so that the displayed arithmetic expressions involve sub-expressions which evaluate to whole numbers (i.e. integers).  This means that evaluating any part of the expression from left to right always results in an integer.
For example, (19-1)/3 is valid because (19-1) equals to 18 which is divisible by 3 (i.e. 3 is a factor of 18). In other words if we divide 18 by 3 the remainder is 0.

(19-1)/4 is would not be valid because 18 is not divisible by 4 (i.e. 4 is not a factor of 18). In other words, if we divide 18 by 4 the remainder is not 0.

Modify the application so that the displayed arithmetic expressions involve sub-expressions which do not evaluate above 100. This means that evaluating any part of the expression from left to right always results is a number less or equal than 100.

Extend the application so that it includes a count down timer counting from 50 seconds down to 0, every tick occurring after 1 second exactly.
As soon as the counter reaches the value of 0, the game stops and the application displays how many correct and incorrect answers the user has given. At this point the game is not playable any more. To play again the user must press the Back mobile device button to return to the main screen (displaying the New Game and the About buttons.

Extend the application (assuming that you implement the countdown timer question) so that every time that the user get 5 answers correct, 10 extra seconds are added to the timer. For example, if the countdown timer displays 20 seconds as remaining and at that point the user completes 5 correct answers the counter goes up to 30 seconds. Then again, while the timer shows 9 seconds as remaining, the user completes another 5 correct answers (they do not have to be 5 consecutive correct answers) the timer goes up to 19 seconds.
 
<img src="https://github.com/helderpgoncalves/ArithmeticGame-Android/blob/main/app/src/main/res/drawable/game_screen.png" width="200"/>
<img src="https://github.com/helderpgoncalves/ArithmeticGame-Android/blob/main/app/src/main/res/drawable/game_screen1.png" width="200"/>

