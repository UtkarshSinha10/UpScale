# UpScale

Question1. 
Print all nodes at distance k from a given node (Time limit to solve question 30
minutes)
Given a binary tree, a target node in the binary tree, and an integer value k, print all the nodes
that are at distance k from the given target node. No parent pointers are available.
Consider the tree shown in diagram
Input: target = pointer to node with data 8.
root = pointer to node with data 20.
k = 2.
Output : 10 14 22
If target is 14 and k is 3, then output
should be “4 20”
If target is 12 and k is 2, then output
should be “4 20”


Question2.
Given a matrix of dimension m*n where each cell in the matrix can have values 0, 1 or 2
which has the following meaning:
0: Empty cell
1: Cells have fresh oranges
2: Cells have rotten oranges
Determine what is the minimum time required so that all the oranges become rotten. A rotten
orange at index [i,j] can rot other fresh orange at indexes [i-1,j], [i+1,j], [i,j-1], [i,j+1] (up,
down, left and right). Output should contain total no of days for which rotten process will
continue, number of fresh oranges and number of rotten oranges at the end of process.
Examples:
Input: arr[][C] = { {2, 1, 0, 2, 1},
{1, 0, 1, 2, 1},
{1, 0, 0, 2, 1}};
Output:
time frames: 2
fresh oranges: 0
Rotten oranges: 11
Explanation:
At 0th time frame:
{2, 1, 0, 2, 1}
{1, 0, 1, 2, 1}
{1, 0, 0, 2, 1}
At 1st time frame:
{2, 2, 0, 2, 2}
{2, 0, 2, 2, 2}
{1, 0, 0, 2, 2}
At 2nd time frame:
{2, 2, 0, 2, 2}
{2, 0, 2, 2, 2}
{2, 0, 0, 2, 2}
Input: arr[][C] = { {2, 1, 0, 2, 1},
{0, 0, 1, 2, 1},
{1, 0, 0, 2, 1}};
Output:
time frames: 1
fresh oranges: 1
Rotten oranges: 9
Explanation:
At 0th time frame:
{2, 1, 0, 2, 1}
{0, 0, 1, 2, 1}
{1, 0, 0, 2, 1}
At 1st time frame:
{2, 2, 0, 2, 2}
{0, 0, 2, 2, 2}
{1, 0, 0, 2, 2}
At 2nd time frame:
{2, 2, 0, 2, 2}
{0, 0, 2, 2, 2}
{1, 0, 0, 2, 2}
...
The 1 at the bottom left corner of the matrix is never rotten.
Input: arr[][C] = { {2, 1, 0, 2, 1},
{1, 0, 1, 2, 1},
{1, 0, 0, 2, 1},
{1, 0, 0, 0, 0},
{1, 1, 1, 1, 1},
{1, 0, 0, 0, 1},
{1, 0, 1, 0, 1}};
Output:
time frames: 10
fresh oranges: 1
Rotten oranges: 21
Explanation:
At 0th time frame:
{2, 1, 0, 2, 1}
{0, 0, 1, 2, 1}
{1, 0, 0, 2, 1}
At 1st time frame:
{2, 2, 0, 2, 2}
{0, 0, 2, 2, 2}
{1, 0, 0, 2, 2}
At 2nd time frame:
{2, 2, 0, 2, 2}
{0, 0, 2, 2, 2}
{1, 0, 0, 2, 2}
...
The 1 at the bottom left corner of the matrix is never rotten.
