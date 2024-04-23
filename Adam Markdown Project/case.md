**CASE**

A CASE construct indicates a multiway branch based on conditions that are mutually exclusive. Four keywords, CASE, OF, OTHERS, and ENDCASE, and conditions are used to indicate the various alternatives. The general form is:

<ul style= "list-style: none;">
<li>CASE expression OF</li>
<ul style= "list-style: none; margin-top: 5px;">
<li>condition 1 : sequence 1</li>
<li>condition 2 : sequence 2</li>
<li>...</li>
<li>condition n : sequence n</li>
<li>OTHERS:</li>
<li>default sequence</li>
</ul>
<li>ENDCASE</li>
<li>The OTHERS clause with its default sequence is optional. Conditions are normally numbers or characters</li>
</ul>

indicating the value of "expression", but they can be English statements or some other notation that specifies the condition under which the given sequence is to be performed. A certain sequence may be associated with more than one condition.

Example

<ul style= "font-size:10px; list-style: none;">
<li>CASE  Title  OF</li>
<ul style= "font-size:10px; list-style: none;">
<li>Mr      : Print "Mister"</li>
<li>Mrs     : Print "Missus"</li>
<li> Miss    : Print "Miss"</li>
<li>Ms      : Print "Mizz"</li>
<li>Dr      : Print "Doctor"</li></ul>
<li>ENDCASE</li>
</ul>

Example

<ul style= "font-size:10px; list-style: none;">
<li>CASE  grade  OF</li>
<ul style= "font-size:10px; list-style: none;">
<li>A       : points = 4</li>
<li>B       : points = 3</li>
<li>C       : points = 2</li>
<li>D       : points = 1</li>
<li>F       : points = 0</li>
</ul>
<li>ENDCASE</li>
</ul>

<div style="text-align: center; display: flex; justify-content: center; margin-top: 30px">

[Next](while.md)                        
[Previous](repeat-until.md)

</div>
<div style="text-align: center; text-decoration: underline; text-decoration-color: #3486E3; margin-top: 150px;" markdown="1">

[Home](home.md)   
[What is Pseudocode?](what-is.md)  
[If-Then-Else](if-then-else.md)  
[While](while.md)  
[Case]  
[Repeat-Until](repeat-until.md)  
[For](for.md)  
[Nested-Constructs](nested.md)  
[Subprocedures](subprocedures.md)  
[Exception-Handling](exceptionhandle.md)  
[Examples](examples.md)  
<div>


---
Excerpted from the original at https://users.csc.calpoly.edu/~jdalbey/SWE/pdl_std.html

---

<a href="https://brickmmo.com">
<img src="https://brickmmo.com/images/brickmmo-logo-horizontal.jpg" width="100">
</a>

