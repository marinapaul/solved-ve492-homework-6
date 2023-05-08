Download Link: https://assignmentchef.com/product/solved-ve492-homework-6
<br>



<h1>1           Question 1: D-Separation</h1>

You are given several graphical models below, and each graphical model is associated with an independence (or conditional independence) assertion. Please specify if the assertion is true or false.

Please write your answer for each subpart in one row.

<ul>

 <li>Assertion: It is guaranteed that <strong>I </strong>is independent of <strong>G </strong>given <strong>H</strong><em>,</em><strong>E</strong><em>,</em><strong>C</strong></li>

 <li>Assertion: It is guaranteed that <strong>A </strong>is independent of <strong>I </strong>given <strong>B</strong><em>,</em><strong>D</strong></li>

</ul>

1

<ul>

 <li>Assertion: It is guaranteed that <strong>K </strong>is independent of <strong>H </strong>given <strong>A</strong><em>,</em><strong>L</strong></li>

 <li>Assertion: It is guaranteed that <strong>L </strong>is independent of <strong>K </strong>given <strong>A</strong><em>,</em><strong>C</strong><em>,</em><strong>J</strong></li>

 <li>Assertion: It is guaranteed that <strong>F </strong>is independent of <strong>H </strong>given <strong>A</strong><em>,</em><strong>I</strong></li>

 <li>Assertion: It is guaranteed that <strong>C </strong>is independent of <strong>L </strong>given <strong>K</strong>.</li>

</ul>

<h1>2           Question 2: Variable Elimination</h1>

Consider the graphical model shown below, where all variables have binary domains. We are given the query <em>P</em>(<em>F</em>| + <em>c</em>). Assume that we run variable elimination with the following ordering: <em>B,D,E,A</em>.

After introducing evidence, we have the following factors:

<h2>                         P(A),        P(B),          P(+c | A,B),           P(D | +c),          P(E | +c,D),             P(F | A,+c,B,E)</h2>

Step 1: After joining on <em>B </em>and summing out over <em>B</em>, we have generated a new factor <em>f</em><sub>1 </sub>over the following variables and/or evidence (note <em>B </em>is not included after summing out over <em>B</em>):

<table width="387">

 <tbody>

  <tr>

   <td width="64">A</td>

   <td width="63">B</td>

   <td width="71">+c</td>

   <td width="64">D</td>

   <td width="63">E</td>

   <td width="62">F</td>

  </tr>

  <tr>

   <td width="64">x</td>

   <td width="63"> </td>

   <td width="71">x</td>

   <td width="64"> </td>

   <td width="63">x</td>

   <td width="62">x</td>

  </tr>

 </tbody>

</table>

After this step, the remaining factors are:

<table width="681">

 <tbody>

  <tr>

   <td width="77">P(A)</td>

   <td width="77">P(B)</td>

   <td width="114">P(+c|A,B)</td>

   <td width="99">P(D|+c)</td>

   <td width="113">P(E|+c,D)</td>

   <td width="141">P(F|A,+c,B,E)</td>

   <td width="59"><em>f</em><sub>1</sub></td>

  </tr>

  <tr>

   <td width="77">x</td>

   <td width="77"> </td>

   <td width="114"> </td>

   <td width="99">x</td>

   <td width="113">x</td>

   <td width="141"> </td>

   <td width="59">x</td>

  </tr>

 </tbody>

</table>

Step 2: After joining on <em>D </em>and summing out over <em>D</em>, we have generated a new factor <em>f</em><sub>2 </sub>over the following variables and/or evidence (note <em>D </em>is not included after summing out over D):

Sample answer:

<strong>AB </strong>+ <strong>cDEF</strong>

After this step, the remaining factors are:

Sample answer:

<strong>P</strong>(<strong>A</strong>)<strong>P</strong>(<strong>B</strong>)<strong>P</strong>(+<strong>c </strong>| <strong>A</strong><em>,</em><strong>B</strong>)<strong>P</strong>(<strong>D </strong>| +<strong>c</strong>)<strong>P</strong>(<strong>E </strong>| +<strong>c</strong><em>,</em><strong>D</strong>)<strong>P</strong>(<strong>F </strong>| <strong>A</strong><em>,</em>+<strong>c</strong><em>,</em><strong>B</strong><em>,</em><strong>E</strong>)<strong>f1f2</strong>

Step 3: After joining on <em>E </em>and summing out over <em>E</em>, we have generated a new factor <em>f</em><sub>3 </sub>over the following variables and/or evidence (note <em>E </em>is not included after summing out over <em>E</em>): Sample answer:

<strong>AB </strong>+ <strong>cDEF</strong>

After this step, the remaining factors are:

Sample answer:

<strong>P</strong>(<strong>A</strong>)<strong>P</strong>(<strong>B</strong>)<strong>P</strong>(+<strong>c </strong>| <strong>A</strong><em>,</em><strong>B</strong>)<strong>P</strong>(<strong>D </strong>| +<strong>c</strong>)<strong>P</strong>(<strong>E </strong>| +<strong>c</strong><em>,</em><strong>D</strong>)<strong>P</strong>(<strong>F </strong>| <strong>A</strong><em>,</em>+<strong>c</strong><em>,</em><strong>B</strong><em>,</em><strong>E</strong>)<strong>f1f2f3</strong>

Step 4: After joining on <em>A </em>and summing out over <em>A</em>, we have generated a new factor <em>f</em><sub>4 </sub>over the following variables and/or evidence (note <em>A </em>is not included after summing out over <em>A</em>): Sample answer:

<strong>AB </strong>+ <strong>cDEF</strong>

After this step, the remaining factors are:

Sample answer:

<strong>P</strong>(<strong>A</strong>)<strong>P</strong>(<strong>B</strong>)<strong>P</strong>(+<strong>c </strong>| <strong>A</strong><em>,</em><strong>B</strong>)<strong>P</strong>(<strong>D </strong>| +<strong>c</strong>)<strong>P</strong>(<strong>E </strong>| +<strong>c</strong><em>,</em><strong>D</strong>)<strong>P</strong>(<strong>F </strong>| <strong>A</strong><em>,</em>+<strong>c</strong><em>,</em><strong>B</strong><em>,</em><strong>E</strong>)<strong>f1f2f3f4</strong>

Reminder: The final factor (or the product of final factors if there are more than one) is guaranteed to be equal to selected joint <em>P</em>(<em>F,</em>+<em>c</em>). To answer the original query, we need to renormalize to obtain <em>P</em>(<em>F</em>|+<em>c</em>).