Hello,

We have installed the xtb version 6.4.1 (afa7b- size "threshold", but encounters memory problems in the case of larger molecules. 
This happens for instance in the example of a pi-stacked dimer containing 704 atoms at all.
Below you can find the partial submission script and the error message provided by the system. 

I was wandering if you could provide with any suggestions/help on how to fix this problem.

Thanking you in advance for your time and attention!

​Partial submission code:

module load xtb

ulimit -s unlimited​ (this line was added to fix the problem, no improvement) ​

xtb t15H-dimer.xyz --opt tight >t15H-dimer.out
​

Error message

​forrtl: severe (174): SIGSEGV, segmentation fault occurred

Image              PC                Routine            Line        Source
xtb                0000000002FC382D  Unknown               Unknown  Unknown
xtb                00000000031D8320  Unknown               Unknown  Unknown
xtb                000000000302BAAD  Unknown               Unknown  Unknown
xtb                000000000302B700  Unknown               Unknown  Unknown

xtb                00000000009A7906  xtb_disp_coordina         396  coordinationnumber.f90

xtb                000000000313B283  Unknown               Unknown  Unknown
xtb                00000000030ECDC3  Unknown               Unknown  Unknown
xtb                00000000030EBF4B  Unknown               Unknown  Unknown
xtb                000000000313B639  Unknown               Unknown  Unknown
xtb                00000000031D4B14  Unknown               Unknown  Unknown
xtb                0000000003243B79  Unknown               Unknown  Unknown
