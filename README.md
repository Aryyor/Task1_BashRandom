# Task1_BashRandom
This is a Bash Script that returns an output of numbers 1-10 in random order with each number appearing only once.

1. BUILD INSTRUCTIONS
Pre-Requisite 
A personal computer that can be 
- Unix/Linux
- Windows
- macOS
with pre-built command line interface environment e.g. Command Prompt or Windows Powershell (Windows), Terminal (macOS), Shell/Console or Terminal (Linux/Unix)

Text editor to save the code as a script.


2. DESCRIPTION:
To build this Batch Scripts, we can make use of the built-in random number generator in Bash $ echo $RANDOM

- $RANDOM is a bash function which returns a signed 16-bit interger (from 0 to 32767).
- Since the task limits the random number generation from 1 to 10, we introduce a modulo to limit the generated random interger. For instance, the below modulo only returns int between 1-10:

$ echo $(( $RANDOM % 10 + 1))


3. USAGE:Some Uses of Bash Scripts for random number generation
- To build games (e.g. a toss of the dice, picking a random card from a deck)
- To create sample data


4. LIMITATIONS/BUGS
- The code uses an in-built random number generator called 'RANDOM'. RANDOM returns a non-uniform random output, therefore, the behaviour is random . For instance, doing arithmetic on random numbers can dramatically affect the randomness of the output. 
-
- Any computer-generated sequences of "random" numbers are refered to as "pseudorandom". This is because true "randomness," insofar as it exists at all, can only be found in certain incompletely understood natural phenomena such as radioactive decay.
- 
- This Script cannot be used to generate encryption key, passwords or anything related to security.
