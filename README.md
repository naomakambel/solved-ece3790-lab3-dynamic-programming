Download Link: https://assignmentchef.com/product/solved-ece3790-lab3-dynamic-programming
<br>
<strong>The purpose of this lab is to give you practical experience programming and analyzing dynamic programming algorithms.</strong>

<strong>Important: </strong>Please include the following signed statement with your submission.

I (We), [insert name(s)] attest that the work I am (we are) submitting is my (our) own work and that it has not been copied/plagiarized from online or other sources. Any sourced material used for completing this work has been properly cited. [Signature(s)]

<strong>Also Important: </strong>Labs done in pairs must be submitted with a short paragraph outlining each partner’s contribution.

<h1>Introduction</h1>

In class we have been introduced to dynamic programming as a way of solving problems by subdividing problems into subproblems similar in structure to the original problem. In addition to this standard property, subproblems must 1) overlap and 2) have optimal substructure. The basic idea of dynamic programming is to obtain the optimal solution to a problem by exploiting the fact that it can be obtained from optimal solutions to subproblems <em>and </em>that we can save time by keeping track of subproblems we have already solved.

<h1>Problem 1 – The Fibonacci Numbers</h1>

There are many problems that can benefit from the ideas that go into dynamic programming, even if they are not naturally dynamic programming problems. Consider the Fibonacci numbers, defined by the recurrence:

<em>F<sub>n </sub></em>= <em>F<sub>n</sub></em><sub>−1 </sub>+ <em>F<sub>n</sub></em><sub>−2</sub><em>,               n </em>= 2<em>,</em>3<em>,…,              F</em><sub>0 </sub>= <em>F</em><sub>1 </sub>= 1

As discussed in class, this problem has overlapping subproblems. The concept of memoization can be applied to this problem with dramatic effects on performance.

<h2>Functions</h2>

<ol>

 <li>Implement a function called recursiveFibonacci that, given an integer <em>n</em>, applies a divide-and-conquer strategy (without memoization) and returns <em>F<sub>n</sub></em>.</li>

 <li>Implement a function called memoizedFibonacci that, given an integer <em>n</em>, applies a dynamic-programming strategy (top-down with memoization) and returns <em>F<sub>n</sub></em>. You may add whatever arguments you require, or a wrapper function as necessary, to make the memoized version of the function work to your liking.</li>

 <li>Implement a function called bottomupFibonacci that, given an integer <em>n</em>, applies a bottom-up dynamic programming strategy and returns <em>F<sub>n</sub></em>.</li>

</ol>

<h2>Main Program</h2>

Write a main program Lab 3 Problem 1 that specifies an array of values of <em>n </em>and collects the running times for your three functions A, B, and C for computing the Fibonacci numbers as a function of <em>n</em>.

<h2>Data Collection and Analysis</h2>

Once you have completed writing your functions and main program you need to:

<ul>

 <li>Call your main program on appropriate values of <em>n </em>to get the general trends of the computational costs of each method for computing the <em>n</em>th Fibonacci number. • Determine the best Big-O notation fit for each of the three approaches. Show your work! Remember that operation counting and order-of-growth is always a possibility. • For each of the three approaches, plot the analytic and measured costs/times and the output of the main program in one figure, producing 3 total plots. Scale the curves appropriately and provide details in the legend.</li>

</ul>

<h2>Evaluation and Discussion</h2>

Answer the following questions:

<ol>

 <li>How does your divide-and-conquer strategy solve the problem of computing the <em>n</em>th Fibonacci number? Explain briefly, relating your answer to the three steps of divideand-conquer.</li>

 <li>How does dynamic programming improve upon the divide-and-conquer solution? What makes this improvement possible? Explain briefly, relating your answer to the key features of dynamic programming.</li>

 <li>How would you summarize the general performance of the three approaches? Why do they perform the way they do?</li>

 <li>Which of the three approaches is “best”? Justify your reasoning.</li>

 <li>Do any of the three approaches have the same complexity? If so, which one would you use? Assuming you are using the faster one, why is it faster if the complexity is the same?</li>

 <li>What computer hardware are you running your program on, and what is the (approximate) index <em>n </em>of the largest Fibonacci number that you can compute on your system in one hour using each of the three methods? Justify your answer.</li>

</ol>

<strong>Hand in:</strong>

Hand in your derivations for the recurrence relation solutions, all code, plots, and your answers to the discussion questions.

<h1>Problem 2 – Choose Your Own Adventure</h1>

<h2>Introduction</h2>

In class we have seen two interesting problems that can benefit from dynamic programming: Matrix Chain Multiplication (MCM) and the Longest Common Subsequence (LCS). Your task is to implement a solution to either problem.

<h2>Functions</h2>

<ol>

 <li>Implement a function called recursiveMCM or recursiveLCS that returns the optimum <u>value </u>of the problem you have chosen to solve (this is the cost of the multiplication in MCM or the length of the LCS). We leave the input arguments to your discretion.</li>

 <li>Implement a function called memoizedMCM or memoizedLCS that improves the top-down recursive version using memoization. You may add whatever arguments you require, or a wrapper function as necessary, to make the memoized version of the function work to your liking.</li>

 <li>Augment B to also calculate the solution to the problem (i.e., the parenthesization forMCM or the actual longest subsequence for LCS).</li>

</ol>

<h2>Main Program</h2>

Write a main program Lab 3 Problem 2 that:

<ul>

 <li>Sets up problems of various sizes and evaluates and stores the computational time of your functions as the input sizes grows.</li>

</ul>

<h2>Validation and Data Collection</h2>

Once you have completed writing your functions and main program you need to: • Show that your function works. If you don’t want to program a brute-force answer you will need to show some examples that are convincing.

<ul>

 <li>Use your functions to collect timing data for various problem sizes.</li>

 <li>Determine the complexity of your solutions. Show your work!</li>

 <li>Plot the analytic and measured costs/times and the output of the main program in one figure, producing 2 plots (one for each implementation). Make sure to scale the curves appropriately.</li>

</ul>

<h2>Evaluation and Discussion</h2>

Answer the following questions:

<ol>

 <li>How do the 4 general steps of dynamic programming apply to the case of the problem you chose to implement? That is, what do you specifically do in each of these 4 steps to solve the problem?</li>

 <li>How did the performance of the algorithm improve using memoization? What technique did you use to determine the total cost of the algorithms? Is there an easy/logical “math-free” way to summarize the performance?</li>

 <li>For the problem you chose to solve, is a bottom-up implementation possible? If so how would it work? If not, why not?</li>

 <li>Research time: Find a problem that you find interesting and briefly explain how dynamic programming can be used to efficiently solve the problem focusing on optimal substructure and overlapping subproblems. Make sure to say things in your own words and provide references supporting your research.</li>

</ol>

<strong>Hand in:</strong>

Hand in all code, plots, and your answers to the discussion questions