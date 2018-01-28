This project belongs to Raunak Rishav. (netid: rr853)


Part 0:
- The wire Diagram for the Demultiplexer is in this folder as Demultiplexer (.jpeg file)


Part 1:
-(Part 1 -> a) The wire Diagram for the Multiplexer is in this folder as Multiplexer (.jpeg file)
-(Part 1 -> b) The wire Diagram for the Encoder is in this folder as Encoder (.jpeg file)
-(Part 1 -> a) The URL of the website for the required adder (SN54LS181 Microcontroller) data sheet is: "http://www.ti.com/lit/ds/symlink/sn54ls181.pdf"
	       The data sheet is in the folder as sn54ls181(Datasheet) (.pdf file)

Extra Credit:
-(Extra Credit -> a) Babylonian Method to find the algorithm.

Algorithm:

Make a guess, here I have assigned the number itself as the guess value.
Divide the original number by the guess.
Set an error limit (Here I have set the error limit as 0.0000001)
Now subtract the quotient (from step 2) from the guessed number.
Now check if the number from the step 4 is greater than the error.
if it is, then set the guessed number as (sum of the last guessed number and the quotient from step 2) divided by 2.
Iterate steps 4 - 6 until the value from step 3 is less then the error value.
Once this condition is met, you will get the squre-root of the desired number. 

Source:
https://en.wikipedia.org/wiki/Methods_of_computing_square_roots
https://www.deltacollege.edu/dept/basicmath/Babylonian.htm


-(Extra Credit -> b) Here is the code(can also be found in the folder as squareroot.txt): 
 
float babylonianRoot(double toFind){
  float error = 0.0000001
  float num = toFind;
  while((num - toFind/num) > error){
    num = (num + toFind/num)/2;
  }
  
  return num;
}


-(Extra Credit -> c) The Y86-64 code is attached in the folder as squareroot (Y86-64)

Thank you,
Raunak