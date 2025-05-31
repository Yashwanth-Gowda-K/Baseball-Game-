# Baseball-Game-



Problem Overview
This problem simulates scoring operations in a baseball game where each operation affects the record of scores in different ways. The challenge is to process a sequence of operations and calculate the final sum of all valid scores.

Operations Explained
The input consists of four possible operations:

Integer (x):
Records a new score of x
Example: "5" adds 5 to the record
Plus Sign ('+'):
Records a new score that's the sum of the previous two scores
Example: If last two scores are 5 and 3, adds 8
Double ('D'):
Records a new score that's double the previous score
Example: If last score is 3, adds 6

Cancel ('C'):
Invalidates the previous score (removes it from record)
Example: Removes the most recently added score

Solution Approach
The optimal solution uses a stack data structure to:
Dynamically track valid scores as operations are processed
Efficiently handle each operation in constant time
Maintain correct score sequence throughout all operations

Key Features
Stack Operations: Perfectly matches the problem's LIFO requirements
Error Handling: Automatically skips invalid operations by design
Time Efficiency: Processes all operations in O(n) time
Space Efficiency: Uses O(n) space for the stack

Practical Applications
Understanding stack data structure applications
Learning to process sequential operations
Developing algorithmic thinking for game simulations
Common interview question for technical roles

Example Walkthrough
For operations ["5","2","C","D","+"]:
Add 5 → [5]
Add 2 → [5, 2]
Cancel → [5]
Double → [5, 10]
Sum → [5, 10, 15]
Final sum = 5 + 10 + 15 = 30
