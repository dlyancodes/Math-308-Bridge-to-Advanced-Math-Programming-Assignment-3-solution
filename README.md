# Math-308-Bridge-to-Advanced-Math-Programming-Assignment-3-solution

Download Here: [Math 308: Bridge to Advanced Math Programming Assignment 3 solution](https://jarviscodinghub.com/assignment/math-308-bridge-to-advanced-math-programming-assignment-3-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Instructions.
• Use IDLE to create a text file entitled pa3.py containing the functions described in the
problems listed below. It is okay to include other functions to help you do the problems.
• After you create each function you should test that it works correctly.
• Upload this file to blackboard. To do this, log in to blackboard. Click on “Programming
Assignments” in the left panel, then click “Programming Assignment 3”. Click on the button
“Browse My Computer” and select your pa3.py file. Then click the “Submit” button at the
bottom of the page.
• You do not need to record your name in the pa3.py file. Blackboard knows your name and
relays that information to me.
Grading. You work will be graded based on the following criteria:
• If the file generates an error when loaded into Python, your grade will be a zero. (You should
test your file!)
• I will call the functions listed in the problems with the exact names listed below with test
cases. Your program should return a correct answer. You will get full credit for that case if
it returns a correct answer, and zero credit if it returns a wrong answer, returns no answer,
or generates an error.
• The correct response must be returned from each function. (Printing it out will not count.
Use the return statement!)
Problems. Inside the file pa3.py place functions as described below which solve each of the
following problems. Only include these three functions, and be sure to title them as described in
the problems. (Improperly titled functions will not be called properly.) To write these functions,
it should be sufficient to understand the documents on Logic and on Tuples and Sets listed on the
course programming page.
1. The tribonacci sequence is a sequence of integers defined inductively by a0 = a1 = 0, a2 = 1,
and an+3 = an + an+1 + an+2 for integers n ≥ 0. Write a function tribonacci(m) which takes
as input an number m ≥ 1 and returns the list [a0, a1, a2, . . . , ak] where ak is the largest number
in the sequence with ak < m.
2. Viewing addition as a binary operation, the Catalan number Ck is the number of ways to write
k + 1 as a sum of k + 1 ones. Here k ≥ 0 is an integer. For example C0 = 1 because 1 can only
be expressed as 1, and C1 = 1 because 2 = 1 + 1 is the only way to write 2 as a sum of ones.
But, C2 = 2 because
3 = (1 + 1) + 1 = 1 + (1 + 1),
and C3 = 5 because
4 = 1+
1+ (1+1)
= 1+
(1+1)+1
= (1+1)+ (1+1) =
(1+1)+1
+1 =
1+ (1+1)
Suppose we have an expression for k + 1 as a sum of ones. Then there is an outermost addition,
and we can simplify the left and right sides. For example, the sum
1 + (1 + 1)
+ 1 simplifies
to 3 + 1. Every sum representing k + 1 simplifies to a sum of the form a + b with a ≥ 1, b ≥ 1
and a + b = k + 1. Furthermore in such a sum a and b are each represented as a sum of ones.
It follows that for k ≥ 1 we have
Ck =
X
k−1
i=0
CiCk−i−1.
(Here each term CiCk−i−1 represents number of ways to write k + 1 as a sum of ones which
simplifies to (i + 1) + (k − i).)
Write a function catalan_numbers(n) which returns the list of the first n Catalan numbers:
[C0, C1, . . . , Cn−1]. Remark: All you really need to know about the Catalan numbers is that
C0 = 1 and the summation formula above. (The Catalan numbers show up in a lot of counting
problems. Wikipedia has a nice article on the Catalan numbers.)
3. Write a recursive function multiply(m,n) which takes as input two integers m and n, and
returns their product m ∗ n only using addition and subtraction. Hints:
m ∗ 0 = 0, m ∗ n = m ∗ (n − 1) + m and m ∗ n = m ∗ (n + 1) − m.
(Remark: Your function should work for all integers.)
4. Suppose f : R → R. Then, we define f
◦k
to be f applied k ∈ N times:
f
◦k
(x) =
k
z }| {
f ◦ f ◦ . . . ◦ f(x)
for x ∈ R. Write a recursive function iterate(f,k,x) which takes as input a function f : R →
R, a natural number k, and a floating point number x and returns the value of f
◦k
(x).
5. The middle third Cantor set is defined by a limiting process. We define C0 = [0, 1] and will
define Ci
inductively for integers i ≥ 0. Each Ci
is a finite union of closed intervals. For each
integer i ≥ 0, we define Ci+1 ⊂ Ci by removing the middle third of the intervals in Ci
. So for
example
C1 =

0,
1
3

∪

2
3
, 1

and C2 =

0,
1
9

∪

2
9
,
1
3

∪

2
3
,
7
9

∪

8
9
, 1

.
The middle third Cantor set is defined by C =
T∞
i=0 Ci
.
Write a function cantors_set_contains(n,x) which takes as input an integer n ≥ 0 and
returns the truth value of the statement x ∈ Cn.
You do not have to use recursion. But, if you want to use recursion, it might be helpful to use
the function f : C1 → C0 defined by
f(x) = (
3x if x ∈

0,
1
3

3x − 2 if x ∈

2
3
, 1

.
Then you can define Ci by iteration:
Ci =
n
x ∈ [0, 1] : {x, f(x), f ◦2
(x), . . . , f ◦(i−1)(x)} ⊂ C1
o
.
Page
An equivalent way to define Ci
is
Ci = {x : f
◦i
(x) is well defined}.
(Can you see why these versions of Ci are correct?)
Hint: For testing, it may be useful to note that 1
4
∈ C while 1
2·3
k 6∈ C for any integer k ≥ 0.

