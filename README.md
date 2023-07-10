# Booth_Multiplier
In this repository I have uploaded various formats of the radix-4 booth multiplier which is one of the efficient multipliers, I have implemented the Multiplier in BASYS 3 board,
Implementation of signed 8-bit, 16-bit, 32-bit radix-4 recoded array multiplier, input a and b registers are taken as signed type 
and the generated output is a signed number. The signed number is first represented using 2’s complement 
form as a first step then the sign of multiplicand is extended to the MSB  bit and a 0 bit at LSB of the multiplier is 
appended to apply booth encoding algorithm as per the below table. 
 
 ![image](https://github.com/udayapeddirajub/Booth_Multiplier/assets/86663239/a40dc3dd-bf2c-479a-b1fa-320725ccb80e)

 
d1, d2, d3 and d4 are the four partial products that are generated as per the control bits from the booth encoder 
then all four partial products are added as per the shift and add scheme then we’ll obtain the final product output in 
signed 2’s complement form. The design can be optimized by using efficient adders and further recoding from the 
encoded data of the booth encoder i.e. we can just consider the recoding for +1,+2 and 0. 
For Unsigned multiplication, we just need to remove the 2’s compliment generator and sign extension in the initial 
stage. 
