# Numbers Part 1

<pre>
This is a way to convert the numbers into different bases.
Binary ( base 2) - octal ( base 8 ) - hexadecimal ( base 16 ) are the important bases that we use.

Numbers in 10 base :
	An-1An-2An-3......A0.A-1A-2........A-m+1Am
	=> Sigma n-1...0 ( Ai * 10^i ) + Sigma -m...-1 ( Ai * 10^i )

::>> in general we can put anything insted of 10.

10 to r :
	Just divide until you reach zero and write backwards.
	For float part => multiply until you reach zero ( each time write int part ) read forwards.
	Ex 0.78125 = ? (16)
		0.78125 * 16 = 12.5 => 12 = C
		0.5 * 16 = 8.0 => 8
	== 0.C8 (16)

Note: Be carefull that in converting the floating parts into different base, you might get a repeated part number.
just like 10/3 in base 10.

We have another algorithem to change into binary:
	1. Number -= 2 ^ int (log2(number))
	2. write 2 ^ int (log2(number))
	3. Do it again till you get zero
	4. Now sum up the write ones

A short way to convert binary to octal or hexadecimal:
	1. start from float point
	2. for left side divide 3 bit 3 bit till end ( if last one was not 3 bits, just add zeros )
	3. sum up each three bits to 10 base and put them next to each
	4. for floating part just go to right by dividing 3 bit 3 bit ( again do for last 3 bits )
	5. convert and sum them up

:: for hexadecimal do this 4 bits 4 bits
</pre>
