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
