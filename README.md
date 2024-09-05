# Bitwise-operators

>The purpose of Bitwise Operators is that "To perform Operations on Integer Data in the form of Bit by Bit".
=>The Bitwise Operators are applicable only on Integer Data but not floating point values bcoz floating point values not able to provide Certainity where as Integer Values provides Certainity.
=>The Exexution Process of Bitwise Operators  is
			i) Bitwise Operators Converts Integer Data into Binary Data.
			ii) Biwise Operator is applied on Binary Data and Performs Bitwise Operation and Result available in Binary Format.
			iii) By Default Python Programming displays the result of Bitwise Operator in the form of Decimal 
			     Number System bcoz Python is High Level Language.
=>Internally, The Bitwise Operators Performs the Operations on Binary Data in the form Bit by Bit and hence they 
   named Bitwise Operators.
=>In Python Programing, we have 6 Bitwise Operators. They are given in the following Table
--------------------------------------------------------------------------------------------------------------------------------------------------------
		SLNO		SYMBOL			MEANING
--------------------------------------------------------------------------------------------------------------------------------------------------------
		1.			<<				Bitwise Left Shift Operator
		2.			>>				Bitwise Right Shift Operator
		3.			|				Bitwise OR Operator
		4.			&				Bitwise AND Operator
		5.			~				Bitwise Complement Operator
		6.			^				Bitwise XOR Operator
-----------------------------------------------------------------------------------------------------------------

=======================================================
				1. Bitwise Left Shift Operator ( << )
			=======================================================
Syntax:	varname = Given Number << No. of Bits
--------------------
Explanation:
--------------------
The Execution Process of Bitwise LeftShift Operator ( << ) is that "It Moves Number of Bits Towards Left Side By Adding Number of Zeros (Number of Zeros=Depending No. Of bits we Flipped-off) at Right Side.
-------------------------------
Examples
-------------------------------
>>> a=10
>>> b=a<<3
>>> print(b)------------80
>>> print(4<<3)-------32
>>> print(9<<2)-------36
>>> print(10<<0)-----10
>>> print(10.3<<2)-----------TypeError: unsupported operand type(s) for <<: 'float' and 'int'
>>> print(4<<-1)-------------ValueError: negative shift count
========================================x======================================================

04/09/2024

Bitwise OR Operator ( | )
==================================================
=>Syntax:		Value1 | Value2
=>The Functionality of Bitwise OR Operator ( | ) is described with following truth table.
			----------------------------------------------------------------
				Value1	Value2	    Value1 | Value2
			----------------------------------------------------------------
				0		1				1
				1		0				1
				0		0				0			
				1		1				1	
			----------------------------------------------------------------

Example-2
-----------------------------
a=10---------------->0000 1010
b=4----------------->0000  0100
------------------------------------------
c=a|b--------------->0000 1110
print(c)------------->14
------------------------------------------
>>> a=10
>>> b=10
>>> print(a|b)------10
------------------------------------------
Example-3
------------------------------------------
>>> s1={10,20,30}
>>> s2={15,10,25}
>>> s3=s1.union(s2)
>>> print(s3,type(s3))--------{20, 25, 10, 30, 15} <class 'set'>
------------------OR---------------
>>> s1={10,20,30}
>>> s2={15,10,25}
>>> s3=s1|s2  # Bitwise OR (|) Operator
>>> print(s3,type(s3))----------{20, 25, 10, 30, 15} <class 'set'>
>>> s1={1.2,2.3,4.5}
>>> s2={1.2,2.3,4.6}
>>> s3=s1|s2  # Bitwise OR (|) Operator
>>> print(s3,type(s3))----------{1.2, 2.3, 4.5, 4.6} <class 'set'>
>>> 1.2|2.3--------------------------TypeError: unsupported operand type(s) for |: 'float' and 'float'
----------------------------------------
>>> s1={"Python","Django"}
>>> s2={"C","HTML","C++"}
>>> s3=s1|s2   # Bitwise OR (|) Operator
>>> print(s3,type(s3))-----------{'C++', 'HTML', 'C', 'Python', 'Django'} <class 'set'>
>>> "Python"|"Java"-------------TypeError: unsupported operand type(s) for |: 'str' and 'str'
------------------------------------------------------------

->Bitwise AND Operator (&)
==================================================
=>Syntax:		Value1 & Value2
=>The Functionality of Bitwise AND Operator (&) is described with following truth table.
			----------------------------------------------------------------
				Value1	Value2	    Value1 & Value2
			----------------------------------------------------------------
				0		1				0
				1		0				0
				0		0				0
				1		1				1
			----------------------------------------------------------------

Example-2
-----------------------------
>>>a=10-------------  0000 1010
>>>b=4--------------- 0000 0100
			-------------------------
>>>c=a&b----------  0000  0000
>>>print(c)---------0
-------------------------------------------------
>>>"Apple" & "mango"-------------TypeError: unsupported operand type(s) for &: 'str' and 'str'
>>> print(5&4)-------------------4
>>> print(4&5)-------------------4
---------------------------------------------------------
Example-3
---------------------------------------------------------
>>> s1={10,20,30}
>>> s2={15,20,35}
>>> s3=s1.intersection(s2)
>>> print(s3,type(s3))--------------{20} <class 'set'>
------------------OR------------------------		
>>> s1={10,20,30}
>>> s2={15,20,35}
>>> s3=s1&s2  # Bitwise & (AND) Operator
>>> print(s3,type(s3))---------{20} <class 'set'>
-------------------------------------
>>> s1={"Apple","mango","Kiwi"}
>>> s2={"Guava","Orango","mango"}
>>> s3=s1.intersection(s2)
>>> print(s3,type(s3))---------------{'mango'} <class 'set'>
-----------------------------------
>>> s1={"Apple","mango","Kiwi"}
>>> s2={"Guava","Orango","mango"}
>>> s3=s1&s2  # Bitwise & (AND) Operator
>>> print(s3,type(s3))-------------------{'mango'} <class 'set'>
------------------------------------------
>>> s1={1.2,2.3,4.5}
>>> s2={2.3,3.3,4.4}
>>> s3=s1.intersection(s2)
>>> print(s3,type(s3))---------{2.3} <class 'set'>
>>> s1={1.2,2.3,4.5}
>>> s2={2.3,3.3,4.4}
>>> s3=s1&s2  # Bitwise & (AND) Operator
>>> print(s3,type(s3))-----------{2.3} <class 'set'>
>>> 2.5&3.4-------------------------TypeError: unsupported operand type(s) for &: 'float' and 'float'
-----------------------------------------
>>> lst=[10,20,30,40]
>>> tpl=(10,15,25,56)
>>> lst&tpl---------------TypeError: unsupported operand type(s) for &: 'list' and 'tuple'

5. Bitwise Complement Operator ( ~ )
   ================================================================

>Syntax:      varname= ~Given Number
=>The execution process of Bitwise Complement Operator ( ~ ) is that " It Inverts the given bits".
=>Inverting the bits is nothing but 1 becomes 0 and 0 becomes 1
=>The formula for Bitwise Complement Operator ( ~ ) is given bellow
				 ~Given Number =  - ( Given Number + 1)
----------------------------------------------------------------------------------------------------------------------------------------------------------------
Example1:
--------------------
>>> a=10
>>> print(~a)--------------      -11
>>> a=100
>>> print(~a)-----------------   -101
-----------------
>>> a=-123
>>> print(~a)-----------------  122

Q) Prove that  ~15 is -16
=============================================================================================
Proof : Given  ~15 =  -16
		Here -16 is the Opposite counter part of 16
 >Given Number  15 and Whose Binary Part is   0000  1111
=> ~15 ----------------- ~(0000  1111) =   1111 0000 (Which is the Binary form of -16)
---------------------------------------------------------
=>Here -16 is the Opposite counter part of 16
=>All Negative Number stored in Main Memory in the form 2's Complement (2's complement= 1's complement+1)
-------------------------------------------------------
=>Here we Take 16 and whose Binary form is   0001 0000
	(1's Complement of any Number= 1 becomes 0 and 0 becomes 1)
=>1's Complement of 16 is----------------------------1110  1111
=>2's Complement of 16 is----------------------------1's Complement of 16 + 1
								=>	1110  1111
									0000  0001    Binary Addition ( (0+0=0, 1+0=1, 0+1=1 , 1+1= 0 with carry 1 )
									------------------
									1111	 0000  (Which is the Binary form of -16)
=============================================x=================================================
