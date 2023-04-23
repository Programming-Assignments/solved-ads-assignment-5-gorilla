Download Link: https://assignmentchef.com/product/solved-ads-assignment-5-gorilla
<br>
How closely related are humans and gorillas? It is well known that out DNA-sequencies are very similar. But how do we actually know this? How do we even measure the similarity between two strings of DNA. And speaking of strings, how do we know how similar two strings are? Is it possible to use almost the same algorithm to align all kinds of strings? Of course not, guitar strings are aligned in a completely different way.

<h1>Aims</h1>

The goals of the lab are:

<ul>

 <li>Implementing a DP-algorithm.</li>

 <li>Debugging your code.</li>

 <li>Structuring your code in a logical fashion.</li>

 <li>Parsing a bit messy input.</li>

 <li>Reason about correctness of your algorithm.</li>

 <li>Reason about upper bounds for time complexity.</li>

</ul>

<h1>Problem formulation</h1>

You are given two strings, which can be viewed as words or DNA-sequences. Furthermore you are given a matrix with the cost of aligning each pair of letters, i.e. the gain of aligning ”A” with ”B” and so on. Given these strings find an optimal alignment, such that the total gain of aligning the strings in maximized.

When aligning the two strings you are allowed to insert certain ”*”-characters in one or both of the strings at as many positions in the string as you like. Each such insertion can be done to a cost of −4. No letters in either of the strings can be changed, moved or removed – the only allowed modification is to insert ”*”.

<h1>Input</h1>

The first line contains a number of space-separated characters, <em>c</em><sub>1</sub><em>,…,c<sub>k </sub></em>– the characters that will be used in the strings. Then follows <em>k </em>lines with <em>k </em>space-separated integers where the <em>j</em>-th integer on the <em>i</em>-th row is the cost of aligning <em>c<sub>i </sub></em>and <em>c<sub>j</sub></em>. Then follows one line with an integer <em>Q </em>(1≤ <em>Q </em>≤10), the number of queries that you will solve. Then follows <em>Q </em>lines, each describing one query. Each of these lines contain two space-separated strings, the strings that should be aligned with maximal gain. It is guaranteed that each string in all queries has size at most 3500.

<h1>Output</h1>

The output should contain exactly one line per query. On each of these lines two strings should be given, the strings from the input possibly with some ”*” inserted. The strings have to be given in the same order as in the input.

<h1>Examination and Points of Discussion</h1>

To pass the lab make sure you have:

<ul>

 <li>Have successfully implemented the algorithm with the correct time complexity.</li>

 <li>Have neat and understandable code.</li>

 <li>Have descriptive variable names.</li>

 <li>Have filled in the blanks in the report.</li>

 <li>Have run the check_solution script to validate your solution.</li>

</ul>

During the oral presentation you will discuss the follwoing questions with the lab assistant:

<ul>

 <li>Is your solution recursive or iterative?</li>

 <li>What is the time complexity, and more importantly why?</li>

 <li>What would the time complexity of a recursive solution without cache be?</li>

 <li>Can you think of any applications of this type of string alignment?</li>

 <li>What could the costs represent in the applications?</li>

</ul>

<strong>Sample Input 1                                                                                 Sample Output 1</strong>

<table width="622">

 <tbody>

  <tr>

   <td width="311">A B C2 0 -10 3 1-1 1 32AABC ABCABA ACA</td>

   <td width="311">AABC *ABCABA ACA</td>

  </tr>

 </tbody>

</table>


