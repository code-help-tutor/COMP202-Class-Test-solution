COMP202 Class Test solution
  Part A:
1. Assume that T (1) = c for some fixed constant c > 0. What are the correct statements below
if function T satisfies the following recurrence:
T(n) = n · T(n/2).
NOTE: More than one answer is correct. The base of log is 2. Recall that we learned about at least two methods to solve recurrences: the Substitution Method and the Master Method.
⌅A. T(1)=1,thatisc=1 ⇤B. T(n)=n(log(n)+1)/3
⇤C. T(n)=n(log(n))/2 ⌅D. T(n)=n(log(n)+1)/2
⇤E. T(1)=2,thatisc=2 ⇤F. T(1)=3,thatisc=3
Solution: Let us first observe that if we take as T(n) any of the formulas in B, C or D, then using any of those formulas gives us T(1) = 1. This suggests that we should choose A as one of the correct answers, that is, T (1) = 1.
Now, how to decide which of B, C , D is correct? There are two ways to do this, one is to use the Substitution Method to solve the above recurrence. The second, quicker and easier, method is to directly try these three formulas B, C, D, under the assumption that T (1) = 1. Let us indeed do that (I am doing it here for the right formula only). Assume that T (n) = n(log(n)+1)/2, then:
n·T(n/2)=n·(n/2)(log(n/2)+1)/2 =n·(n/2)(log(n) log(2)+1)/2 =n·(n/2)(log(n) 1+1)/2 =n·(n/2)(log(n))/2
(log(n))/2 ✓n(log(n))/2◆ ✓ n(log(n))/2 ◆ ✓n(log(n))/2◆
= n · (n/2) = n · 2(log(n))/2 = n · (2log(n))1/2 = n · (n)1/2 = n · pn
✓n(log(n))/2◆ = pn · n(log(n))/2 = (n)1/2 · n(log(n))/2 = n1/2+(log(n))/2 = n(1+log(n))/2 = T (n).
    2. Assume that T(n) = c for n  d, for some constants c and d. What is the correct asymptotic solution to the following recurrence:
T (n) = 4 T (n/2) + n2 log n.
NOTE: Only one answer is correct. The base of log is 2. Recall that we learned about at least
two methods to solve recurrences: the Substitution Method and the Master Method.
⇤A. T(n)is⇥(n2)
⌅B. T(n) is ⇥(n2 log2 n) ⇤C. T(n) is ⇥(n2 logn) ⇤D. T(n) is ⇥(nlog2 n) ⇤E. T(n) is ⇥(nlogn)
Hint: Use Master Method. PAPER CODE COMP202
page 2 of 10
Continued
----PAGE----
  3. Assume that T(n) = c for n  d, for some constants c and d. What is the correct asymptotic solution to the following recurrence:
T (n) = 4 T (n/3) + n2 log n.
NOTE: Only one answer is correct. The base of log is 2. Recall that we learned about at least
two methods to solve recurrences: the Substitution Method and the Master Method.
⇤A. T(n) is ⇥(nlog3 4 logn) ⇤B. T(n) is ⇥(nlog3 4 log2 n) ⇤C. T(n) is ⇥(n2 log2 n) ⌅D. T(n) is ⇥(n2 logn) ⇤E. T(n)is⇥(nlog34)
Hint: Use Master Method.
4. Assume that T(n) = c for n  d, for some constants c and d. What is the correct asymptotic
solution to the following recurrence:
T (n) = T (n/2) + 2 log n.
NOTE: Only one answer is correct. The base of log is 2. Recall that we learned about at least two methods to solve recurrences: the Substitution Method and the Master Method.
⇤A. T(n) is ⇥(n)
⇤B. T(n) is ⇥(nlogn) ⇤C. T(n) is ⇥(logn) ⇤D. T(n) is ⇥(nlog2 n) ⌅E. T(n)is⇥(log2n)
Hint: Use Master Method. You can also use the Substitution Method, or just observe that we can halve n under T(n/2) in the recurrence log(n) times until we reach constant n  d and each time we halve n, we add 2 log(n) in the recurrence. This means that we add 2 log(n), log(n) times, and at the end T(n) = c for constant n  d, so we obtain that T(n) = ⇥(log2 n).
5. NOTE: Only one answer is correct.
An instance of the Fractional Knapsack Problem is given by a set, S, of items, each item i has weight wi and benefit bi , and the knapsack weight is W . This problem asks the question: Find a setting for variables xi (one for each item i), where 0  xi  wi that
Continued
⇤A. maximizes Pi2S ⇤ B. maximizes P
bi, and such that Pi2S wi  W. bi xi ,andsuchthatP wi W.
⌅C. maximizes
⇤D. maximizes i2S ⇤E. maximizes Pi2S
PAPER CODE COMP202
wi Pi2S
bixi, and such that i2S xi  W.
Pi2S Pi2S
wi Pi2S
bi xi ,andsuchthat xi W.
bi, and such that Pi2S xi  W. page 3 of 10
----PAGE----
  6. What is the solution to the following instance of the Fractional Knapsack problem with knapsack weight W = 11.
item a b c d benefit 9 8 12 4 weight42 4 2
NOTE: Only one answer is correct.
⇤ A. The optimal solution includes items a, b, c and d for the total benefit of 33.
⇤ B. The optimal solution includes items a, b, c and 1/3 of item d for the total benefit of 30 13 . ⇤ C. The optimal solution includes items a, b, d and 1/2 of item c for the total benefit of 27. ⇤ D. The optimal solution includes items a, b, d and 1/3 of item c for the total benefit of 25. ⌅ E. The optimal solution includes items a, b, c and 1/2 of item d for the total benefit of 31.
7. NOTE: More than one answer is correct.
The data structure AVL tree is a binary search tree with the
   ⌅ A.
⇤ B.
⇤ C.
⇤ D.
⇤ E. ⌅F.
height-balance property: for each internal node its two subtrees have heights differing by at most 1.
height-balance property: for each external node its two subtrees have heights differing by at most 1.
length-balance property: for each internal node its two subtrees have lengths differing by at most 1.
length-balance property: for each external node its two subtrees have lengths differing by at most 1.
height-balance property: for each internal node its two subtrees have the same heights.
height-balance property: for each internal node its two subtrees have lengths of their longest path from their root to a leaf differing by at most 1.
8. NOTE: More than one answer is correct.
What statement is true about sorting algorithms:
⇤ A. ⌅ B. ⇤ C. ⇤ D. ⌅ E. ⇤F.
MergeSort is a comparison-based sorting algorithm which sorts an array of n numbers always in O(n log log n) time.
MergeSort is a comparison-based sorting algorithm which sorts an array of n numbers always in O(n log n) time.
QuickSort is a comparison-based sorting algorithm which sorts an array of n numbers always in O(n log n) time.
QuickSort is a comparison-based sorting algorithm which sorts an array of n numbers in O(n) expected time.
HeapSort is a comparison-based sorting algorithm which sorts an array of n numbers in O(n log n) worst-case time.
HeapSort is a comparison-based sorting algorithm which sorts an array of n numbers in O(n) expected time.
PAPER CODE COMP202 page 4 of 10 Continued
----PAGE----
  Part B:
9. NOTE: Write down answers to this question in an editor and convert the file to PDF. You may also hand-write your answers on a piece of paper, take a good quality picture and convert it to PDF. Submit the PDF file as your solution.
We consider the following problem: Given an unsorted array of n   4 distinct integers A[1, ..., n] (where both positive and negative integers are allowed), you want to find two dis- tinct indices i,j 2 {1,...,n}, i 6= j, for which the product A[i ] · A[j ] is as large as possible. It suffices if, as output, the value of such largest product is returned.
(a) [6 marks] Design a divide-and-conquer algorithm that solves this problem using at most 94n comparisons between elements of array A. Observe that there might be more than one pair of indices i , j which maximise the product A[ i ] · A[ j ], and in such a case it suffices to find
one such pair and output the maximum value of the product.
Remark: You should include an explanation of the ideas and reasons why your algorithm is correct. If your algorithm will use c · n comparisons, where constant c is larger than 49 ,k this will lead to less marks for such a solution. You may assume for simplicity that n = 2 for some positive integer k   2. For the purpose of this problem, if your algorithm computes two products x · y and z · w of elements x, y, z, w of array A and then compares these two products, then we assume that it uses one comparison between elements of array A.
(b) [5 marks] Give an argument that your algorithm indeed uses at most 94n comparisons between elements of array A, by formulating and solving an appropriate recurrence equation.
Solution:
(a) Let us first observe that the solution to this problem is to first find the two largest integers in array A, denote them max1 < max2, and the two smallest integers in array A, denote them min1 < min2. Then the solution is given by the pair max1, max2 and has value of max1 · max2 if max1 · max2   min1 · min2, and the solution is given by the pair min1, min2 and has value min1 · min2, if max1 · max2 < min1 · min2.
Observe here that the product min1 · min2 of the two smallest integers can be the solution to this problem in case if both min1, min2 are negative, because then their product is positive.
We will design a divide-and-conquer algorithm that uses the required number of comparisons and computes these four integers min1, min2 and max1, max2. The final algorithm compares max1 · max2 and min1 · min2, and outputs the larger of these products.
Solution sketch I: The base of the recursive algorithm is the case when n = 4 and suppose that in this case A = [a,b,c,d]. We will show that at most 5 comparisons suffice to solve this problem. We execute one recursive step of MergeSort, followed by a single merge step. Namely, the algorithm first compares a,b and c,d and suppose without loss of generality (w.l.o.g.) that a < b and c < d (this uses 2 comparisons). Now we merge these two sub-lists into one sorted list: compare a, c and let w.l.o.g. a < c, then compare b, c and then if b < c, then a < b < c < d and we are done (with 4 comparisons). Else, if b > c, then a < c are the
 PAPER CODE COMP202 page 5 of 10 Continued
----PAGE----
  in one of the Q and A sessions that we can find the two largest elements in an array of n numbers by using only (3/2)n comparisons between elements in this array. This is just a standard divide and conquer algorithm similar to the above one. Now we can first divide the input array A into two subarrays: A+ of only positive integers from A, and A  of all non-positive integers from A. Let A+ have n1 elements, and let A  have n2 elements, where n = n1 + n2. Note, that it is possible that n1  or n2  1. If n1   2, use the above algorithm to find the two largest elements max1,max2 in A+, using at most (3/2)n1 comparisons. Similarly, if n2   2, use this same algorithm to find the two smallest elements min1,min2 in A , using at most (3/2)n2 comparisons. Compare the two products max1 · max2 and min1 · min2, and return the larger of these as the solution.
What is the total number of comparisons of this algorithm? I said in the problem description that we count comparisons between elements of array A, which means that the comparisons that check whether elements in A are positive or non-positive when producing arrays A+ and A  do not count. This means that the total number of comparisons between elements of array A in this algorithm is at most (3/2)n1 + (3/2)n2 + 1 = (3/2)n + 1.
(b) Let us now denote by f(n) the total number of comparisons between the integers from array A that the above recursive algorithm uses. Then from the definition of the algorithms we obtain that:
f(4) = 5,f(n) = 2f(n/2) + 4. Using the substitution method, we now have:
f(n) = 2f(n/2) + 4 = 2(2f(n/4) + 4) + 4 = 22f(n/4) + 2 · 4 + 4 = 22(2f(n/8) + 4) + 2 · 4 + 4 = 23f(n/8)+22 ·4+2·4+4,
which after iterating this step for i times gives
f(n)=2if(n/(2i))+4·(2i 1 +2i 2 +···+20)=2if(n/(2i))+4·(2i  1),
where in the last equality we have used a formula for the sum of the geometric sequence. Let us now take i such that n/(2i ) = 4 (the initial condition for function f ), which leads to 2i = n/4 and i = log2(n)   2.
We therefore obtain that f (n) = (n/4) · f (4) + 4 · (n/4   1) = (9/4) · n   4.
Observe that the final algorithm compares max00 ·max00 and min00 ·min00 and outputs the larger
1212
of these products, and thus uses at most (9/4) · n   3 comparisons in total.
10. NOTE: Write down answers to this question in an editor and convert the file to PDF. You may also hand-write your answers on a piece of paper, take a good quality picture and convert it to PDF. Submit the PDF file as your solution.
We consider the following problem: Given a set N = {1,2,...,n} of n initial consecutive positive integers, we say that a non-empty subset S ✓ N is called satisfied subset of N = {1, 2, ... , n} if S contains its size |S| (the number of elements in S) as its element. For instance if n = 3 then {1}, {2, 3} are satisfied subsets of {1, 2, 3}, but {1, 3} is not.
PAPER CODE COMP202 page 7 of 10 Continued
----PAGE----
  Let s(n) denote the number of all satisfied subsets of the set N = {1, 2, ... , n}. For instance s(1) = 1, because the only satisfied sPubset of {1} is {1}. Let now s(n,i) denote the number of all satisfied subsets of N = {1,2,...,n} of size exactly i, where the integer i is such that 1  i  n. Let us observe that s(n) = ni=1 s(n,i).
(a) [4 marks] What are the values s(2), s(3), s(4)? Provide arguments to your answer in each case.
(b) [4 marks] To gain an intuition for deriving a recurrence relation for s(n,i) in terms of s(n   1, i) and s(n   1, i   1) in the next question (c), we will consider a special case of ex- pressing s(4, i) in terms of s(3, i) and s(3, i   1) for each i = 1, 2, 3, 4. Namely, list all satisfied subsets of {1, 2, 3} and then argue how to create from those subsets of each size i = 1, 2, 3 corresponding satisfied subsets of {1, 2, 3, 4}. To do so explain how to create satisfied sub- sets of {1,2,3,4} of two different kinds from your listed satisfied subsets of {1,2,3}: (1) those that do not contain element 4, and (2) those which contain element 4. Conclude your reasoning by expressing s(4, i) in terms of s(3, i) and s(3, i   1) for each i = 1, 2, 3, 4.
(c) [3 marks] Explain what is the value of s(n,n)? Derive a recurrence relation for s(n,i) in terms of s(n   1, i) and s(n   1, i   1), for each integers n and i such that 1  i  n. Give an argument justifying your derivation.
Hint to (c): When deriving s(n,i), consider separately satisfied subsets of {1,2,...,n} that contain element n and those that do not contain element n, and try to construct them from the satisfied subsets of {1, 2, ... , n   1}, trying to follow ideas developed in part (b).
Solution I: I present very detailed solutions of part (b) and (c), but such details were not expected in the class test submission.
(a) The only satisfied subsets of {1, 2} are {1}, {1, 2} and therefore s(2) = 2. All satisfied sub- sets of {1, 2, 3} are {1}, {1, 2}, {2, 3}, {1, 2, 3} and so s(3) = 4. Finally, all satisfied subsets of {1,2,3,4} are {1},{1,2},{2,3},{2,4},{1,2,3},{2,3,4},{1,3,4},{1,2,3,4}, and thus we have that s(4) = 8.
(b) All satisfied subsets of {1, 2, 3} are: {1}, {1, 2}, {2, 3}, {1, 2, 3}. To create satisfied sub- sets of {1,2,3,4} we first observe that all satisfied subsets {1},{1,2},{2,3},{1,2,3} of {1, 2, 3} are also satisfied subsets of {1, 2, 3, 4} that do not contain element 4. Now to cre- ate satisfied subsets of {1, 2, 3, 4} that contain element 4 we create them from the satisfied subsets {1}, {1, 2}, {2, 3}, {1, 2, 3} of {1, 2, 3} one-by-one as follows:
• Take set {1}, add element 4 to it and increase the value of its element 1 (equal to its size) to 2, obtaining the new satisfied subset {2, 4} of of {1, 2, 3, 4}.
• Take set {1, 2}, add element 4 to it and increase the value of its element 2 (equal to its size) to 3, obtaining the new satisfied subset {1, 3, 4} of of {1, 2, 3, 4}.
• Takeset{2,3},addelement4andwedonotneedtochangeanythingelsebecauseital- ready contains 3 (its new size), obtaining the new satisfied subset {2, 3, 4} of {1, 2, 3, 4}.
PAPER CODE COMP202 page 8 of 10 Continued
----PAGE----
