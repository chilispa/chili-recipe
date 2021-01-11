# Learn TDD - Kata

## What is Kata?
Kata is a Japanese word meaning <i>“form”</i>, and in the martial arts it describes 
a choreographed pattern of movements used to train yourself to the level of 
muscle memory.

The idea of kata for software development was originally coined by Dave Thomas, 
co-author of handbooks 
[The Pragmatic Programmer: From Journeyman to Master](https://en.wikipedia.org/wiki/The_Pragmatic_Programmer#:~:text=The%20Pragmatic%20Programmer%3A%20From%20Journeyman,and%20published%20in%20October%201999.&text=The%20book%20does%20not%20present,process%20in%20a%20pragmatic%20way.). 
The idea is the same as in martial arts: practice and repetition to refine 
the skills and lock in the patterns.

One of the reasons TDD is hard for newcomers is that you can't add anything more 
than what current testing requires. 
For experienced developers, this is very difficult to do, 
especially when working on <b>real code</b>.

By using the precise nature of the kata to practice TDD skills, 
you can understand that the purpose for the small steps is to learn the movements.

## Kata #1: The Bowling Game Kata

The essence of this kata is to create a scoring engine for 10-pin Bowling. 
In 10-pin bowling you have ten frames where you can roll one, 
two (or three) balls and score the pins that you knock down.

Except the scoring is weird. You’d think 10 pins and ten frames would 
yield a highest possible score of 100, but you’d be wrong. 
The lowest possible score (all misses) is zero, but the highest possible score is 300.

This kata can be break into the following five tests:

1. <i>The game scores zero - When you roll all misses, you get a total score of zero.</i>
2. <i>All ones scores 20 - When you knock down one pin with each ball, 
   your total score is 20.</i>
3. <i>A spare in the first frame, followed by three pins, followed by all misses scores 16.</i>
4. <i>A strike in the first frame, followed by three and then four pins, 
   followed by all misses, scores 24.</i>
5. <i>A perfect game (12 strikes) scores 300.</i>

He has some very explicit refactorings that you are to perform 
while implementing the third and fourth tests, and doing this is important.

## Kata #2: The String Calculator

Like the Bowling Kata, this kata comes with a precise set of steps to follow. 
The essence is a method that given a delimited string, returns the sum of the values. 

This kata can be break into the following tests:
1. <i>An empty string returns zero</i>
2. <i>A single number returns the value</i>
3. <i>Two numbers, comma delimited, returns the sum</i>
4. <i>Two numbers, newline delimited, returns the sum</i>
5. <i>Three numbers, delimited either way, returns the sum</i>
6. <i>Negative numbers throw an exception</i>
7. <i>Numbers greater than 1000 are ignored</i>
8. <i>A single char delimiter can be defined on the first line (e.g. //# for a ‘#’ as the delimiter)</i>
9. <i>A multi char delimiter can be defined on the first line (e.g. //[###] for ‘###’ as the delimiter)</i>
10. <i>Many single or multi-char delimiters can be defined (each wrapped in square brackets)</i>
