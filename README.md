# DESIGN _AND_DEVELOPMENT_OF_LOW-POWER_AND_HIGH-SPEED-MEMORY_DEVICES
<h2>I. Abstract :</h2>
Recently, speed and power 
consumption are becoming the most important part 
of semiconductor industries. This project is focusing 
on the designing of low-power and high-speed 
memory devices. starting with the working operation 
of a standard conventional static random access 
memory SRAM 6T cell. In this work, the techniques 
to minimize the power consumption of SRAM 6T 
cell with the minimum delay during its read 
operation is analyzed and designed. It is evident 
from the results that the SRAM cell which acts as a 
cache memory is better in performance with 
minimum power.
<br>Keyword- SRAM

<h2>II. Introduction :</h2>
Static Random Access memory takes a large area 
due to the number of transistors for a single bit. The cell 
generally employs a minimum number of the transistor to 
employ high packaged density. As long as power is being 
provided, Static Random Access memory (SRAM) is a 
static form of random access memory (RAM), keeps data 
bits in its memory. The SRAM is quite similar to a latch in 
which two inverters are connected in cross-coupled. 
The cell requires six transistors per bit. The power 
dissipation and propagation delay when reading and writing 
the value into the SRAM cell are two design considerations 
for SRAM. Dynamic power dissipation is the power lost
during read and write operations. It aids in figuring out how 
long portable gadgets' batteries will last. The reading and 
writing delay determines the SRAM's speed. To read data 
from memory, a sense amplifier is utilized. Its job is to 
detect the low-power signals from a bit line that corresponds 
to a data bit (1 or 0) recorded in a memory cell and amplify 
the small voltage swing to identifiable logic levels so the 
data can be properly understood. In addition, the precharge 
circuit is also analyzed prior to allowing a main contactors 
to close, a precharge circuit permits the current to flow in a 
controlled manner while the voltage level increases to the
very close to the source voltage. All the simulations are 
done in cadence virtuoso 180nm technology. 

<h2>III. Design :</h2>
A. Conventional SRAM 6T Cell-
<br>
<br>The design of an SRAM 6T cell is similar to a latch in 
which two CMOS inverters are connected back to back (M1-
M2 and M3-M4) with two secondary nmos transistors (M5-
M6) are connected to the paired bit line BL and bit line bar 
BLB.[5] These two transistors are connected to the word line 
to perform the access of read and write operation as shown in 
Fig.<br>
<br>
<br>

![Screenshot-1](https://github.com/user-attachments/assets/ced1966a-2fa8-4b69-80e5-5edb422c35e9)

<br>
<br>
<br>
<h2>III. Working operation :</h2>
The SRAM cell performs three operation
<br>
1- Write operation
<br>
2- Read operation 
<br>
3- Hold operation
<br>
<br>
<br>
 Write operation -
<br>When word line (WL) is high, the data should be 
written on Q is 0 and QB is 1 and the word line is enabled 
1 to access the lines BL and BLB. The BL and BLB act 
as input. The BLB is connected to the ground because QB 
is 1. There will be some voltage difference, the voltage will decrease for transistors M1 and M2. If the voltage is 
less than the threshold voltage of M2 then M2 is turned off 
and M1is turned on. That means output Q will be 1. So 
input Q is 0 and output Q=1 means data is written.
<br>
<br>
<br>

Read operation -
WL is high, t memory should hold some value. 
Now Q is 1 and QB is complementing 0. [6] Now 
memory has some value stored and to read BL and BLB 
now act as output lines and these lines will be precharged 
by voltage VDD at both nodes Q and QB. Now there is 
no voltage difference at node Q =1 and T5 so there will 
be no discharge but on another side QB = 0 and the 
voltage is VDD and there is a voltage difference so there 
will be discharge at node QB and node voltage at BLB 
will start discharging. Now the values stored in BL and 
BLB will be sent to the sense amplifier which helps as a 
comparator and it says if BLB decreases then the output 
will be 1 it means we successfully read from the memory 
because the memory has a value of 1 and getting read 1 
as output.


