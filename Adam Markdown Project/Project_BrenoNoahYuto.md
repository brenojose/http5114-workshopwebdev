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

**IF-THEN-ELSE** 
<p>
Binary choice on a given Boolean condition is indicated by the use of four keywords: IF, THEN, ELSE, and ENDIF. The general form is: 
</p>
</p>
<ul>
    <p>
    IF condition THEN     
    </p>
    <ul>
        sequence 1
    </ul>
        <p>
        ELSE    
        </p>
    <ul>
        <p>
        sequence 2        
        </p>
    </ul>
    <p>
    ENDIF
    </p>
</ul>
<p>
The ELSE keyword and "sequence 2" are optional. If the condition is true, sequence 1 is performed, otherwise sequence 2 is performed. 
</p>
<p>
Example 
</p>

<ul>

`IF HoursWorked > NormalMax THEN` <br>
<ul>

`Display overtime message`
</ul>

`ELSE`
<ul>

`Display regular time message`
</ul>

`ENDIF`
</ul>

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

**REPEAT-UNTIL**

This loop is similar to the WHILE loop except that the test is performed at the bottom of the loop instead of at the top. Two keywords, REPEAT and UNTIL are used. The general form is:

<ul style= "list-style: none;">
<li>REPEAT</li>
<ul style= "list-style: none;">
<li>sequence</li>
</ul>
<li>UNTIL condition</li>
</ul>

The "sequence" in this type of loop is always performed at least once, because the test is peformed after the sequence is executed. At the conclusion of each iteration, the condition is evaluated, and the loop repeats if the condition is false. The loop terminates when the condition becomes true.

**FOR**

This loop is a specialized construct for iterating a specific number of times, often called a "counting" loop.  Two keywords, FOR and ENDFOR are used. The general form is:

<ul style= "list-style: none;">
<li>FOR iteration bounds</li>
<ul style= "list-style: none;">
<li>sequence</li>
</ul>
<li>ENDFOR</li>
</ul>

In cases where the loop constraints can be obviously inferred it is best to describe the loop using problem domain vocabulary.

Example

<ul style= "list-style: none; margin-bottom:15px;">
<li>FOR each month of the year (good)</li>
<li>FOR month = 1 to 12 (ok)</li></ul>
<ul style= "list-style: none;">
<li>FOR each employee in the list (good)</li>
<li>FOR empno = 1 to listsize (ok)</li>
</ul>

<p>
  
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


&nbsp;

**INVOKING SUBPROCEDURES**


Use the CALL keyword. For example:

<ul>
CALL AvgAge with StudentAges<br>
CALL Swap with CurrentItem and TargetItem<br>
CALL Account.debit with CheckAmount<br>
CALL getBalance RETURNING aBalance<br>
CALL SquareRoot with orbitHeight RETURNING nominalOrbit<br>
</ul>
<p>
&nbsp;

**EXCEPTION HANDLING**
</p>

<ul>
BEGIN
    <ul>statements</ul>
    EXCEPTION
    <ul>WHEN exception type
        <ul>statements to handle exception</ul>
        WHEN another exception type
        <ul>statements to handle exception</ul>
    </ul>
END
</ul>

___
**<p style="text-align: center;">Sample Pseudocode</p>**

"Adequate"  

FOR X = 1 to 10  
  FOR Y = 1 to 10  
    IF gameBoard[X][Y] = 0  
      Do nothing  
    ELSE  
      CALL theCall(X, Y) (recursive method)  
      increment counter  
    END IF  
  END FOR  
END FOR

"Better"

Set moveCount to 1  
FOR each row on the board  
  FOR each column on the board  
    IF gameBoard position (row, column) is occupied THEN  
      CALL findAdjacentTiles with row, column  
      INCREMENT moveCount  
    END IF  
  END FOR  
END FOR

(Note: the logic is restructured to omit the "do nothing" clause)

___
<br>
"Not So Good"
<br><br>

FOR all the number at the back of the array  
  SET Temp equal the addition of each number  
  IF > 9 THEN  
    get the remainder of the number divided by 10 that index  
    and carry the "1"  
  Decrement one  
Do it again for numbers before the decimal  
<br>
 

"Good Enough (not perfect)"

SET Carry to 0  
FOR each DigitPosition in Number from least significant to most significant

COMPUTE Total as sum of FirstNum[DigitPosition] andSecondNum[DigitPosition] and Carry
  
  IF Total > 10 THEN  
    SET Carry to 1  
    SUBTRACT 10 from Total  
  ELSE  
    SET Carry to 0  
  END IF  

STORE Total in Result[DigitPosition]

END LOOP  

IF Carry = 1 THEN  
  RAISE Overflow exception  
END IF

___
<br>
"Pretty Good"  This example shows how pseudocode is written as comments in the source file. Note that the double slashes are indented.
<br><br>

public boolean moveRobot (Robot aRobot)  
{  
  //IF robot has no obstacle in front THEN  
    // Call Move robot  
    // Add the move command to the command history  
    // RETURN true  
  //ELSE  
    // RETURN false without moving the robot  
  //END IF  
}  

Example Java Implementation

<li>source code statements are interleaved with pseudocode.</li> 
<li>comments that correspond exactly to source code are removed during coding.</li><br>


public boolean moveRobot (Robot aRobot)  
{  
  //IF robot has no obstacle in front THEN  
  if (aRobot.isFrontClear())  
  {  
    // Call Move robot  
    aRobot.move();  
    // Add the move command to the command history  
    cmdHistory.add(RobotAction.MOVE);  
    return true;  
  }  
  else // don't move the robot  
  {  
    return false;  
  }//END IF  
}  

<div style="text-align: center; text-decoration: underline; text-decoration-color: #3486E3 " markdown="1">

[Examples of vague pseudocode](https://users.csc.calpoly.edu/~jdalbey/SWE/pdl_vague.html)

</div>

___
Document History

<style>
table {
  width: 100%;
}

th, td {
  border: 1px solid black;
}
</style>

| Date           | Author| Change |
| :---------------- | :------ | :---- |
| 12/2/03        |   JD  | Added Exception Handling and more examples |
| 2/21/03           |   JD   | Added "problem domain vocabulary"paragraph.<br>Modified FOR loop explanation. |









