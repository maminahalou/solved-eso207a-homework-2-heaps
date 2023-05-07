Download Link: https://assignmentchef.com/product/solved-eso207a-homework-2-heaps
<br>
<table width="573">

 <tbody>

  <tr>

   <td width="169"><strong>ESO207A:</strong></td>

   <td width="81"><strong>Data</strong></td>

   <td width="122"><strong>Structures</strong></td>

   <td width="202"><strong>and                   Algorithms</strong></td>

  </tr>

  <tr>

   <td width="169">Homework <em>2: Heaps,</em></td>

   <td width="81"> </td>

   <td width="122"> </td>

   <td width="202"> </td>

  </tr>

 </tbody>

</table>

<strong>Instructions.</strong>

<ol>

 <li>Solutions have to be submitted on Gradescope. For this, each problem should start on a newsheet. If this is not followed then it may not be possible to grade your answers.</li>

 <li>For each problem, write your name, Roll No., problem number, the date and the names ofany students with whom you collaborated. Remember that you must write the answer and the algorithm in your own words.</li>

 <li>For questions in which algorithms are asked for, your answer should provide the following: (a) A clear description of the algorithm in English and/or pseudo-code, where, helpful, (b) A proof/argument of the correctness of the algorithm, and, (c) an analysis of the running time of the algorithm.</li>

</ol>

<em>Full marks will be given only to correct solutions which are described clearly</em>. Convoluted and unclear descriptions will receive <em>low marks</em>.

<strong>Problem 1. </strong><em>Heap</em>. The following is an alternative routine to build a max-heap by permuting the elements of an array. It uses the subroutine <em>Max-Heap-Insert</em>(<em>A,v</em>). Here <em>A </em>is a max-heap where the elements are stored in the array <em>A</em>[1<em>…N</em>], where, <em>N </em>is the maximum capacity of the array, and (ii) the field <em>A</em>.<em>heapsize </em>that counts the number of items in the heap <em>A</em>. This routine takes the heap <em>A </em>and inserts <em>v </em>into the max-heap. It also increments <em>A.heapsize </em>by 1.

<ol>

 <li>Consider the following procedure for building a heap.</li>

</ol>

<em>procedure Build-Max-Heap</em>(<em>A,n</em>) // Build Max Heap for the elements in <em>A</em>[1<em>,…,n</em>]

<ol>

 <li><em>heapsize </em>= 1</li>

 <li><strong>for </strong><em>i </em>= 2 <strong>to </strong><em>n</em></li>

 <li><em>Max-Heap-Insert</em>(<em>A,A</em>[<em>i</em>])</li>

</ol>

Show that this procedure takes <em>O</em>(<em>n</em>log<em>n</em>) time.                                                                                                   (10)

<ol start="2">

 <li>Show a worst case input and analyze it to show that on that input the procedure takesΩ(<em>n</em>log<em>n</em>) time. Hence this algorithm takes Θ(<em>n</em>log<em>n</em>) time worst-case. (15)</li>

</ol>

<strong>Problem 2. </strong><em>Young tableau</em>.                                                                                                                                         (12<em>.</em>5 × 4 = 50)

An <em>m </em>× <em>n </em>Young tableau is an <em>m </em>× <em>n </em>matrix such that the entries of each row are in sorted order from left to right and the entries of each column are in sorted order from top to bottom. Some of the entries may be ∞ that are treated as non-existent items. Thus a Young tableau can be used to hold <em>r </em>≤ <em>mn </em>finite numbers. Note that an <em>m </em>× <em>n </em>tableau <em>Y </em>is empty if <em>Y </em>[1<em>,</em>1] = ∞ and is full if <em>Y </em>[<em>m,n</em>] <em>&lt; </em>∞. An example Young tableau is

1

<ol>

 <li>Give an algorithm for Extract-Min on a non-empty <em>m</em>×<em>n </em>Young tableau that runs in time <em>O</em>(<em>m </em>+ <em>n</em>). (<em>Hint</em>: Follow Min-Heapify.)</li>

 <li>Show how to insert a new element into a non-full <em>m </em>× <em>n </em>Young tableau in <em>O</em>(<em>m </em>+ <em>n</em>) time.</li>

 <li>Using no other sorting method as a subroutine, show how to use an <em>n </em>× <em>n </em>Young tableau to sort <em>n</em><sup>2 </sup>numbers in <em>O</em>(<em>n</em><sup>3</sup>) time.</li>

 <li>Given an <em>O</em>(<em>m</em>+<em>n</em>)-time algorithm to determine whether a given number is stored in a given <em>m </em>× <em>n </em></li>

</ol>

<strong>Problem 3. </strong><em>Stack: a span problem</em>. You are given an array <em>P</em>[1<em>,…,n</em>] giving the daily price quotes for a stock for <em>n </em>consecutive days. The span of the stock’s price on a given day <em>i </em>is the maximum number of consecutive days that the stock’s price is less than or equal to its price on day <em>i</em>. (This includes day <em>i</em>, so span is at least 1). For example, suppose <em>P </em>is the array {50<em>,</em>45<em>,</em>35<em>,</em>40<em>,</em>60<em>,</em>50<em>,</em>55}. Then, the span array for these 7 consecutive days is {1<em>,</em>1<em>,</em>1<em>,</em>2<em>,</em>5<em>,</em>1<em>,</em>2}. An <em>O</em>(<em>n</em><sup>2</sup>) algorithm follows in a straightforward way from the definition. Design an <em>O</em>(<em>n</em>) (linear-time) algorithm and provide an analysis.              (20+5)

2