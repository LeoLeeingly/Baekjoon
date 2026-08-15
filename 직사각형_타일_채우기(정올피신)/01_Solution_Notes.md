직사각형 타일 채우기
Link: https://jungol.co.kr/problem/18567

#FirstAttempt
Problem declared that squares' sizes are 2 to the power of n
Due to this, I realized that using a bigger size of square always makes the number of squares smaller. Because I can make a bigger square with the previous step's squares (ex. squre size of 2 to the power of n+1 can be made with 4 squares of size 2 to the power of n). 
Then, with this theory that I made, I figured out a solution.
First, I fill the rectangle with the smallest 1 by 1 square, and then divide the rectangle to know how many 2 by 2 squares as possible by using 4 of the 1 by 1 squares. While making it a bigger square, I should check if there are enough squares to fill the rectangle (if it doesn't print -1). As the square increases by 2 to the power of something, I can repeat the same method until I reach the biggest rectangle that the input gave me. Lastly, I print the number of squares that I used.
However, there was a counterexample to the code.
17 20 5
20 0 4 0 1
The answer to this example is 25, but my code printed -1. The reason the error occurred was that I didn't consider 0 on the number of squares.

#FinalAttempt
