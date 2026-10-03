
# 🐱 Cat Finding Puzzle

A classic logic puzzle solved using a systematic search strategy in Python.

## The Puzzle

- A cat is hiding in one of five boxes numbered 1 to 5.
- Every night, the cat moves exactly one box to the left or right.
- Every morning, we can open one box to look for the cat.
- The challenge is to find the cat without knowing its starting position or movements.


![alt text](image.png)

## The Strategy

1. Start by checking Box 2.
2. If the cat is not there, the cat moves to an adjacent box.
3. Next, check Box 3.
4. If the cat is not there, check Box 4.
5. Continue with the same pattern:
      2 → 3 → 4 → 2 → 3 → 4
6. The cat cannot keep moving between boxes without eventually being caught.
7. Therefore, within 6 mornings, you are guaranteed to find the cat.

## How the Code Works

1. Start by considering all five boxes as possible cat locations.
2. Check the next box in the search sequence.
3. Remove the checked box from the possible locations.
4. Move every remaining possible cat location one box left or right.
5. Repeat until no possible locations remain.

If no possible locations remain after a search, the cat must
have been found on that morning.

You can also run the code cell by cell in Jupyter Notebook.

## Key Learning

This puzzle demonstrates how tracking all possible states
can help solve a problem systematically instead of relying
on random guesses.