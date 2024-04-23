**NESTED CONSTRUCTS**
</p>

The constructs can be embedded within each other, and this is made clear by use of indenting. Nested constructs should be clearly indented from their surrounding constructs.</p>

Example
<ul>
 SET total to zero<br>
 REPEAT
</ul>

<ul>
 <ul>
 READ Temperature<br>
 IF Temperature > Freezing THEN<br>
 INCREMENT total<br>
 END IF
 </ul>
</ul>

<ul>
UNTIL Temperature < zero<br>
Print total
</ul>

In the above example, the IF construct is nested within the REPEAT construct, and therefore is indented.

<div style="text-align: center; display: flex; justify-content: center; margin-top: 30px">

[Next](for.md)                        
[Previous](subprocedures.md)

</div>

<div style="text-align: center; text-decoration: underline; text-decoration-color: #3486E3; margin-top: 150px;" markdown="1">

[Home](home.md)   
[What is Pseudocode?](what-is.md)  
[If-Then-Else](if-then-else.md)  
[While](while.md)  
[Case](case.md)
[Repeat-Until](repeat-until.md)  
[For](for.md)  
[Nested-Constructs]    
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

