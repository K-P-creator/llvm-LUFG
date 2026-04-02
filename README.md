#   My LLVM Fork

##  Description

The purpose of this fork is to automatically collect loop info from the LLVM loop unroll pass. This will allow for feature generation for my dataset. 

There will also be a custom mode implemented eventually, that will override tryToUnrollLoop() to use my MLP for the the decision.

Modified files here include

llvm/lib/Transforms/Scalar/LoopUnrollPass.cpp

*not actually modified yet, but it will be!
