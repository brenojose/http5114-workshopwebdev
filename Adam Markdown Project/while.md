
 **WHILE**

The WHILE construct is used to specify a loop with a test at the top. The beginning and ending of the loop are indicated by two keywords WHILTE and ENDWHILE. The general form is:

<ul style= "list-style: none;">
<li>WHILE condition</li>
<ul style= "list-style: none; margin-top: 5px;">
<li>sequence</li>
</ul>
<li>ENDWHILE</li>
</ul>

The loop is entered only if the condition is ture. The "sequence" is performed for each iteration. At the conclusion of each iteration, the condition is evaluated and the loop continues as long as the condition is ture.

Example

<ul style= "font-size:10px; list-style: none;">
<li>WHILE Population < Limit</li>
<ul style= "font-size:10px; list-style: none; margin-top: 5px;">
<li>Compute Population as Population + Births - Deaths</li>
</ul>
<li>ENDWHILE</li>
</ul>

Example

<ul style= "font-size:10px; list-style: none;">
<li>WHILE employee.type NOT EQUAL manager AND personCount < numEmployees</li>
<ul style= "font-size:10px; list-style: none; margin-top:5px;">
<li>INCREMENT personCount</li>
<li>CALL employeeList.getPerson with personCount RETURNING employee</li>
</ul>
<li>ENDWHILE</li>
</ul>


<div style="text-align: center; display: flex; justify-content: center; margin-top: 30px">

[Next](if-then-else.md)                        
[Previous](case.md)

</div>




<div style="text-align: center; text-decoration: underline; text-decoration-color: #3486E3; margin-top: 150px;" markdown="1">

[Home](home.md)   
[What is Pseudocode?](what-is.md)  
[If-Then-Else](if-then-else.md)  
[While]   
[Case](case.md)
[Repeat-Until](repeat-until.md)  
[For](for.md)  
[Nested-Constructs](nested.md)  
[Subprocedures](subprocedures.md)  
[Exception-Handling](exceptionhandle.md)  
[Examples](examples.md)  
<div>

> This repo is available to view at  
> [https://tidy.codeadam.ca](https://tidy.codeadam.ca).

---
Excerpted from the original at https://users.csc.calpoly.edu/~jdalbey/SWE/pdl_std.html

---

<a href="https://brickmmo.com">
<img src="https://brickmmo.com/images/brickmmo-logo-horizontal.jpg" width="100">
</a>

