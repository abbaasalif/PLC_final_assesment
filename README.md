# PLC_final_assesment
codes for practical for PLC final assessment

Question 3
here to change your input edit the input.txt where you can enter a assign statement in the following format

assign "datatype" "IDENTIFIER" = Expression ;

**Scenarios:**

*Boolean Coercion*

![Boolean output](bool.png)


*Output:*
(tf2) PS D:\OneDrive\Documents\PLC\final assessment\question3> python .\front.py
('assign', 'ASSIGN_KEY')
('int', 'INT_CODE')
('i', 'IDENTIFIER')
('=', 'assign_op')
('true', 'BOOLEAN')
(';', 'delimiter')
START <assignment>
ASSIGN_KEY
INT_CODE
IDENTIFIER
assign_op
INTEGER
Enter <expr>
Enter <term>
Enter <factor>
delimiter
Exit <factor>
Exit <term>
Exit <expr>
the expected type and actual type are matching
END <assignment>

