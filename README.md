# Problem 485: Max Consecutive Ones

09/04/2025

## Thought Process
My initial thought process was that I had to traverse through the list and count the ones in order. Whenever I hit a 0, I would start counting all over again. 

## Solution
I initially created a count variable to count all consecutive ones. Then I created a for loop to traverse through the list. I then had a simple if-else statement saying that if the number is one, then add to count, else set count to zero. I then returned count. This initially failed because I failed to take into account where the max consecutive line was in the list. This would only work if the consecutive line was found at the end of the List. To counteract this, I created a big variable which would keep track of the max consecutive line throughout the traversing. Whenever a number was equal to 0, I would see whether or not count was greater than big. If it was, I would set big to count then set count to zero. At the end, I would return the max value of big or count just so I can take into account the final string of consecutive ones count was counting. 

Initial solution - 9 ms 

Complexity - O(N)

## Takeaways
The takeaway is mainly the max() function, which just tells me the max value between two different values. I also learned to look at things hollistically for these types of problems because usually the most obvious solution only focuses on one part of the problem. Instead of blindly following the obvious solution, I learned to use it as a framework to solve the problems from all types of standpoints and solve it as a whole. 