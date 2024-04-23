<h1 style='text-align: center'>
    PSEUDOCODE STANDARD
</h1>
<p>
 Pseudocode is a kind of structured english for describing algorithms. It allows the designer to focus on the logic of the algorithm without being distracted by details of language syntax.  At the same time, the pseudocode needs to be complete.  It describe the entire logic of the algorithm so that implementation becomes a rote mechanical task of translating line by line into source code. 
</p>
<p>
 In general the vocabulary used in the pseudocode should be the vocabulary of the problem domain, not of the implementation domain.  The pseudocode is a narrative for someone who knows the requirements (problem domain) and is trying to learn how the solution is organized.  E.g., 
</p>
<ul>
    <p>
        Extract the next word from the line (good)<br>
        set word to get next token (poor) 
    </p>
    <p>
        Append the file extension to the name (good)<br>
        name = name + extension (poor) 
    </p>
    <p>
        FOR all the characters in the name (good)<br>
        FOR character = first to last (ok)
    </p>
</ul>
<p>
Note that the logic must be decomposed to the level of a single loop or decision. Thus "Search the list and find the customer with highest balance" is too vague because it takes a loop AND a nested decision to implement it. It's okay to use "Find" or "Lookup" if there's a predefined function for it such as String.indexOf(). 
</p>
<p>
Each textbook and each individual designer may have their own personal style of pseudocode. Pseudocode is not a rigorous notation, since it is read by other people, not by the computer. There is no universal "standard" for the industry, but for instructional purposes it is helpful if we all follow a similar style. The format below is recommended for expressing your solutions in our class. 
</p>
<p>
The "structured" part of pseudocode is a notation for representing six specific structured programming constructs: SEQUENCE, WHILE, IF-THEN-ELSE, REPEAT-UNTIL, FOR, and CASE. Each of these constructs can be embedded inside any other construct. These constructs represent the logic, or flow of control in an algorithm. 
</p>
<p>
It has been proven that three basic constructs for flow of control are sufficient to implement any "proper" algorithm. 
</p>
<ul>

**SEQUENCE** is a linear progression where one task is performed sequentially after another. <br>
**WHILE** is a loop (repetition) with a simple conditional test at its beginning. <br>
**IF-THEN-ELSE** is a decision (selection) in which a choice is made between two alternative courses of action.

</ul>
<p>
 Although these constructs are sufficient, it is often useful to include three more constructs: 
</p>
<ul>

**REPEAT-UNTIL** is a loop with a simple conditional test at the bottom.<br>
**CASE** is a multiway branch (decision) based on the value of an expression. CASE is a generalization of IF-THEN-ELSE. <br>
**FOR** is a "counting" loop.
    
</ul>
<p>

**SEQUENCE** 
</p>
<p>
Sequential control is indicated by writing one action after another, each action on a line by itself, and all actions aligned with the same indent. The actions are performed in the sequence (top to bottom) that they are written.  
</p>
<p>
Example (non-computer)  
</p>
<ul>
    
Brush teeth <br>
Wash face <br>
Comb hair <br>
Smile in mirror
    
</ul>
<p>
Example 
</p>
<ul>
READ height of rectangle<br>
READ width of rectangle<br>
COMPUTE area as height times width
</ul>
<p>
Common Action Keywords 
</p>
<ul>
    <p>
    Several keywords are often used to indicate common input, output, and processing operations. 
    </p>
    <ul>
        <p>
        Input: READ, OBTAIN, GET<br>
        Output: PRINT, DISPLAY, SHOW<br>
        Compute: COMPUTE, CALCULATE, DETERMINE<br>
        Initialize: SET, INIT<br>
        Add one: INCREMENT, BUMP
        </p>
    </ul>
</ul>
<p>

<div style="text-align: center; display: flex; justify-content: center; margin-top: 30px">

[Next](home.md)                        
[Previous](if-then-else.md)

</div>

<div style="text-align: center; text-decoration: underline; text-decoration-color: #3486E3; margin-top: 150px;" markdown="1">

[Home](home.md)   
[What is Pseudocode?]   
[If-Then-Else](if-then-else.md)  
[While](while.md)  
[Case](case.md)
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

