# PLC_final_assesment
codes for practical for PLC final assessment

Question 3
here to change your input edit the input.txt where you can enter a assign statement in the following format

assign "datatype" "IDENTIFIER" = Expression ;

**Scenarios:**

*Boolean Coercion*

![Boolean output](bool.png)


*Output:*
<br>
(tf2) PS D:\OneDrive\Documents\PLC\final assessment\question3> python .\front.py <br>
('assign', 'ASSIGN_KEY') <br>
('int', 'INT_CODE') <br>
('i', 'IDENTIFIER') <br>
('=', 'assign_op') <br>
('true', 'BOOLEAN') <br>
(';', 'delimiter') <br>
START assignment <br>
ASSIGN_KEY <br>
INT_CODE <br>
IDENTIFIER <br>
assign_op <br>
INTEGER <br>
Enter expr <br>
Enter term <br>
Enter factor <br>
delimiter <br>
Exit factor <br>
Exit term <br>
Exit expr <br>
the expected type and actual type are matching <br>
END assignment <br>

*Division by zero*

![Boolean output](div0.png)

<br>
*Output:*
<br>
(tf2) PS D:\OneDrive\Documents\PLC\final assessment\question3> python .\front.py <br>
('assign', 'ASSIGN_KEY') <br>
('int', 'INT_CODE')<br>
('i', 'IDENTIFIER')<br>
('=', 'assign_op')<br>
('2', 'INTEGER')<br>
('/', 'div_op')<br>
('0', 'INTEGER')<br>
(';', 'delimiter')<br>
START <assignment><br>
ASSIGN_KEY<br>
INT_CODE<br>
IDENTIFIER<br>
assign_op<br>
INTEGER<br>
Enter <expr><br>
Enter <term><br>
Enter <factor><br>
div_op<br>
Exit <factor> <br>
INTEGER <br>
MathERROR: Zero Division <br>


