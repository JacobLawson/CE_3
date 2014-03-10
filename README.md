### CE_3
====

So... this CE is about making a moore and mealy vhdl design of a four floor elevator.

The CE began with the design of the Moore machine. 
The provided template from the ECE 281 sharepoint was used to help complete the rest of the code. Afterwards,
the testbench was created with use of the knowledge provided in the handout. The testbench is not self checking, 
and it was created by adjusting the periods in which up_down, stop, and reset in order to match up with the given picture.
The testbench output for the Moore machine can be seen below.

![alt text] (http://i57.tinypic.com/s4mecl.png)

The testbench was assumed to be correct for two reasons. Firstly, it matched up with the given picture, which the handout said we should shoot for. Secondly, I went through the testbench itself, and it can clearly been seen that the transition of the states goes as follow. 1st floor due to reset, then 2nd floor for about 3 clock periods (defined in this testbench as 20 ns), then 3rd floor for about 3 clock periods, then the 4th floor for about 3 clock periods, then it goes down to the 1st floor by passing all of the other floors in sequence without stopping. In short, the waveform matches the testbench design criteria and given picture, so I assumed the output and design was functional.
