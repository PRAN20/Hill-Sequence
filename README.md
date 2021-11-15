# Hill-Sequence-

## Hill Sequence Problem Code: HILLSEQ
Add problem to Todo list
Read problem statements in Bengali, Russian, Mandarin and Vietnamese as well.
A sequence A1,A2,…,AN
 of length N
 is called good if any one of the following hold:

The sequence is strictly increasing, or
The sequence is strictly decreasing, or
There exists an index i(1<i<N)
 such that:
Aj<Aj+1
, for each 1≤j<i
Aj>Aj+1
, for each i≤j<N
For example, the sequences [3,5,9]
, [2,1]
, [5,7,4,1]
 are good, while [6,7,7]
, [5,2,3]
 are not.

You are given an array A
 consisting of N
 integers. Find a good sequence by rearranging the elements of the array A
 or report that this is impossible. If there are multiple good sequences, print the lexicographically largest one.

If two sequences A
 and B
 have the same length N
, we say that A
 is lexicographically larger than B
 if there exists an index i
, (1≤i≤N)
 such that A1=B1,A2=B2,…,Ai−1=Bi−1
 and Ai>Bi
.

## Input Format
The first line of input contains a single integer T
, denoting the number of test cases. The description of T
 test cases follows.
The first line of each test case contains an integer N
, denoting the length of the array.
The second line contains N
 space-separated integers A1,A2,…,AN
, denoting the given array.
## Output Format
For each test case, if it is not possible to rearrange the given array into a good sequence, print −1
. Otherwise, print a single line containing N
 space-separated integers - the lexicographically largest good sequence that can be made.

## Constraints
1≤T≤103
1≤N≤105
1≤Ai≤109
Sum of N
 over all test cases does not exceed 5⋅105
Subtasks
Subtask 1 (100 points): Original constraints
## Sample Input 1 
 4
3
2 3 5
3
1 1 1
5
5 7 2 1 2
5
1 2 3 2 2
## Sample Output 1 
 5 3 2
-1
2 7 5 2 1
-1
## Explanation
Test case 1
: The rearrangements of A
 which are good sequences are: [5,3,2]
, [3,5,2]
, [2,3,5]
, [2,5,3]
. Among these, [5,3,2]
 is the lexicographically largest.

Test case 2
: There is no way to obtain a good sequence by rearranging the elements of the array A=[1,1,1]
.
