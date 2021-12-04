# PLC_final_assesment
codes for practical for PLC final assessment

#### Disclaimer: the code is open source but please do not copy for university assignments as you might get into trouble for academic malpractice

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

![DivZero output](div0.png)


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
START assignment<br>
ASSIGN_KEY<br>
INT_CODE<br>
IDENTIFIER<br>
assign_op<br>
INTEGER<br>
Enter expr<br>
Enter term<br>
Enter factor<br>
div_op<br>
Exit factor <br>
INTEGER <br>
MathERROR: Zero Division <br>


*Type mismatch*

![Typemis output](typemis.png)


*Output:*
<br>
(tf2) PS D:\OneDrive\Documents\PLC\final assessment\question3> python .\front.py <br>
('assign', 'ASSIGN_KEY') <br>
('int', 'INT_CODE') <br>
('i', 'IDENTIFIER') <br>
('=', 'assign_op') <br>
('2', 'INTEGER') <br>
('+', 'add_op') <br>
('3.0', 'FLOAT') <br>
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
add_op <br>
Exit factor <br>
Exit term <br>
FLOAT <br>
Enter term <br>
Enter factor <br>
delimiter <br>
Exit factor <br>
Exit term <br>
Exit expr <br>
TypeError: assignment not possible <br>


*Positive case with type casting*

![poscase output](poscase.png)


*Output:*
<br>
(tf2) PS D:\OneDrive\Documents\PLC\final assessment\question3> python .\front.py <br>
('assign', 'ASSIGN_KEY') <br>
('float', 'FLOAT_CODE') <br>
('i', 'IDENTIFIER') <br>
('=', 'assign_op') <br>
('2', 'INTEGER') <br>
('+', 'add_op') <br>
('3.0', 'FLOAT') <br>
('/', 'div_op') <br>
('2', 'INTEGER') <br>
('*', 'mul_op') <br>
('true', 'BOOLEAN') <br>
(';', 'delimiter') <br>
START <assignment> <br>
ASSIGN_KEY <br>
FLOAT_CODE <br> 
IDENTIFIER <br>
assign_op <br>
INTEGER <br>
Enter expr <br>
Enter term <br>
Enter factor <br>
add_op <br>
Exit factor <br>
Exit term <br>
FLOAT <br>
Enter term <br>
Enter factor <br>
div_op <br>
Exit factor <br>
INTEGER <br>
Enter factor <br>
mul_op <br>
Exit factor <br>
INTEGER <br>
Enter factor <br>
delimiter <br>
Exit factor <br>
Exit term <br> 
Exit expr <br>
the expected type and actual type are matching <br>
END assignment
