Download Link: https://assignmentchef.com/product/solved-ch08-320201-homework-10-longest-ordered-subarray-sum-in-triangles-and-scuba-diver
<br>
All problems need to be implemented in python or C++.

<h2>Problem 1: Longest ordered subarray</h2>

Consider the array A=(<em>a</em><sub>1</sub><em>,a</em><sub>2</sub><em>,…a<sub>n</sub></em>). We call a subarray a succession of numbers in A where the position of any value in the subarray in the array is always bigger than the value of the previous one. Use dynamic programming to find a subarray of maximal ordered length of the array A. You can assume there are no duplicate values in the array and that there exists just one optimal solution.

<h2>Example</h2>

For A=(8,3,6,50,10,8,100,30,60,40,80) the solution is: (3,6,10,30,60,80) Your program should take an input and spit out an output as follows:

<em>Sample input</em>

8 3 6 50 10 8 100 30 60 40 80

<em>Sample output</em>

3 6 10 30 60 80

<h2>Problem 2: Sum in triangles</h2>

Consider a triangle formed from n lines (1 <em>&lt; n </em>≤ 100), each line containing natural numbers between [1,10000].

<ol>

 <li>Use dynamic programming to determine the biggest sum of numbers existent between the road fromthe number in the first line and a number from the last line and print the respective road to the output. Each number in this road is seated to the left or to the right of the other value above it.</li>

 <li>Analyze the runtime of your solution and compare it to a brute force approach.</li>

 <li>Explain why a greedy algorithm does not work for this problem.</li>

</ol>

<h2>Example</h2>

The values are displayed for example in this manner:

7

3        8

8        1        0

2        7        4        4

4        5        2        6        5

For this example the resulting sum would be 30.

Your program should take an input and spit out an output as follows:

<em>Sample input</em>

<table width="633">

 <tbody>

  <tr>

   <td width="633">73 88 1 02 7 4 44 5 2 6 5</td>

  </tr>

 </tbody>

</table>

5

<em>Sample output</em>

30

7 3 8 7 5

<h2>Problem 3: Scuba Diver</h2>

A scuba diver uses a special equipment for diving. He has a cylinder with two containers: one with oxygen and the other with nitrogen. Depending on the time he wants to stay under water and the depth of diving the scuba diver needs various amount of oxygen and nitrogen. The scuba diver has at his disposal a certain number of cylinders. Each cylinder can be described by its weight and the volume of gas it contains. In order to complete his task the scuba diver needs specific amounts of oxygen and nitrogen. Theoretically, the diver can take as many cylinders as he wants/needs. Use dynamic programming to find the minimal total weight of cylinders he has to take to complete the task and which those cylinders are. In case of several acceptable solutions, printing just one of them is enough.

<h2>Example</h2>

The scuba diver has at his disposal 5 cylinders described below. Each description consists of: volume of oxygen, volume of nitrogen (both values are given in liters) and weight of the cylinder (given in decagrams):

<table width="633">

 <tbody>

  <tr>

   <td width="633">3 36 12010 25 1295 50 2501 45 1304 20 119</td>

  </tr>

 </tbody>

</table>

5

If the scuba diver needs 5 liters of oxygen and 60 liters of nitrogen then he has to take two cylinders of total weight 249 (for example the first and the second ones or the fourth and the fifth ones).

<h2>Input</h2>

The number of test cases <em>c </em>is in the first line of input, then <em>c </em>test cases follow separated by an empty line.

In the first line of a test case there are two integers <em>t,a </em>separated by a single space, 1 ≤ <em>t </em>≤ 21 and 1≤ <em>a </em>≤79. They denote volumes of oxygen and nitrogen respectively, needed to complete the task. The second line contains one integer <em>n</em>, 1≤ <em>n </em>≤1000, which is the number of accessible cylinders. The following <em>n </em>lines contain descriptions of cylinders; i-th line contains three integers <em>t<sub>i</sub>, a<sub>i</sub>, w<sub>i </sub></em>separated by single spaces, (1≤ <em>t<sub>i </sub></em>≤21<em>, </em>1≤ <em>a<sub>i </sub></em>≤79<em>,</em>1≤ <em>w<sub>i </sub></em>≤800). These are respectively: volume of oxygen and nitrogen in the i-th cylinder and the weight of this cylinder.

<h2>Output</h2>

On the first line will be printed the total weight <em>w<sub>t </sub></em>and on the next line separated by spaces the index of the cylinders in order.

<em>Sample input</em>

<table width="633">

 <tbody>

  <tr>

   <td width="633">15 6053 36 12010 25 1295 50 2501 45 1304 20 119</td>

  </tr>

 </tbody>

</table>

5

2

<em>Sample output</em>

249 1 2