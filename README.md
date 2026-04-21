#   My LLVM Fork

##  Description

The purpose of this fork is to automatically collect loop info from the LLVM loop unroll pass. This will allow for feature generation for my dataset. 

After building the whole project, use:

`cmake --build build --target opt -j8`

when making changes to the opt stage.

Here is a list of the loop features that I am collecting from llvm during the loop-unroll opt pass: 

```
loop depth
has parent loop
loop location
loop range
canonical iv
se iv exists
is guarded
is rotated
is loop simplify form
is annotated parallel
num blocks
num subloops
num exit blocks
num exiting blocks
has dedicated exits
num header phis
total instructions
num loads
num stores
num branches
num calls
num phis
num int ops
num float ops
num icmps
num fcmps
initial loop size
load density
store density
branch density
call density
phi density
int op density
float op density
icmp density
fcmp density
tripcount
tripmultiple
breakouttrip
num getelementptrs
getelementptr density
loopinstructionordering
```
