Download Link: https://assignmentchef.com/product/solved-cs2208b-lab-no-4
<br>
The objective of this lab is:

o To practice ARM assembly programming

If you would like to leave, and at least 30 minutes have passed, raise your hand and wait for the TA.

Show the TA what you did. If, and only if, you did a reasonable effort during the lab, he/she will give you the lab mark.

<strong>==================================================================================== </strong><strong>PROBLEM SET </strong>

Before you start practicing this lab, you need to review and fully understand how to use <em>the Keil ARM Simulator</em>, as well as tutorial 6<em> (Tutorial_06_ARM_Addressing_Modes.pdf).</em>




<ol>

 <li>Translate the following tasks into a single ARM instruction:</li>

</ol>




<ol>

 <li>Add 32 times of the content of registers r0 and the content of r1 only if N is clear. Store the result in register r2</li>

</ol>




<ol>

 <li>Subtract the content of register r3 from 0x990, put the results in register r4 only if C is set and Z is clear.</li>

</ol>




<ol start="6">

 <li>Clear the 2<sup>nd</sup> least significant byte of the content of register r5, i.e., store (00000000)<sub>2</sub> in it, and put the results in register r6. The result of the instruction must affect the value of the<em> Current Program Status Register</em> (CPSR).</li>

</ol>




Test your answers by putting them in a program, which starts by assigning values to r0 and r1 and then comparing them together to set/clear the flags in such a way to test both cases of (a), (b), and (c). Note that, you will need two sets of r0 and r1 values for each case.




Hint: you may want to consider Table 3.2 in the textbook.




<ol start="2">

 <li>Encode <em>by hand</em> the instructions that you suggested in Question 1, i.e., generate the 4 byte machine language of each ARM instruction. Verify your answers using Keil’s simulator.</li>

</ol>

<strong><u>Hint 1</u></strong>: you may want to consider Figure 3.26 in the textbook.

<strong><u>Hint 2</u></strong>: the Op-Code of the ADD instruction is (0100)<sub>2</sub>, the Op-Code of the SUB instruction is (0010)<sub>2</sub>, the Op-

Code of the RSB instruction is (0011)<sub>2</sub>, the Op-Code of the AND instruction is (0000)<sub>2</sub>, and the Op-Code of the BIC instruction is (1110)<sub>2</sub>.

<strong><u>Hint 3</u></strong>: the code for the LSL shift type is (00)<sub>2 </sub>




<ol start="3">

 <li>Convert the GCD algorithm given in this flowchart into</li>

</ol>




<ol>

 <li><strong><em>Traditional </em></strong>assembly, where only branches can be conditional,</li>

</ol>

i.e., do not utilize the ARM conditional execution feature.




<ol>

 <li>ARM assembly, where all instructions are conditional, thus improving code density.</li>

</ol>




PS: The only instructions you need are CMP, B and SUB.




Test your code by assigning various values to r0 and r1.

Copyright © 2016 Mahmoud El-Sakka.