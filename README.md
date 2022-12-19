# Floor-Square-Root-Calculator
A ps of Digisim(Udyam 22) involving the formation of circuit for calculation of floor of the square root of a 10 bit integer input.
The exact problem statement was as follows-
You have to design a circuit which is capable of calculating the square root of
a 10-Bit binary input and producing a 5-Bit binary output. The output should
be the integer value and if the input is not a prefect square, then the output
should be the integer which is just less than the actual square root value.

*Concepts of digital electronics used.
*Proteus skills used.

There were various constraints relating to the formation of circuit while considering the cost and also some specific components mentioned.
The subcircuits of the circuit are as follows-
*A 5 bit counter.
*A 5 by 5 bit multiplier.
*A 10 bit comparator.
*A 5 bit register.

The actual method which I followed was that we can start counting the values from 0 through the counter and then keep on squaring and checking if the square is less than the 10 bit given input as soon as the value gets equaled or surpasses it the counter stops and the register gives an output.
I have used and indicating logic probe to show when the computation is completed i.e when that number changes to 1 from 0 then that means the computation is completed and the output of the register at that moment is the square root of the given input.

One important point to not in this approach is that the ic used for counter when given the same clock for register and for counting, there is a difference in the values of the counter and register of one(as given in the datasheet of the ic) hence when were checking if the square has surpasses or not then it was always checking one number ahead hence if the number got equal to it then the clock stopped but the rest computation carried on for that value and it reported as the square root otherwise if it directly surpasses then the value less one is reported hence accomplishing the task.


I am also attaching the pdf files of the main circuit as well as the sub circuits in case someone just wants to look at the circuit.
