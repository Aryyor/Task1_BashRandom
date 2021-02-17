# Task1_BashRandom
This is a Bash Script that returns an output of numbers 1-10 in random order with each number appearing only once.
To build this Batch Scripts, we can make use of the built-in random number generator in Bash $ echo $RANDOM

- $RANDOM is a bash function which returns a signed 16-bit interger (from 0 to 32767).

- Since the task limits the random number generation from 1 to 10, we introduce a modulo to limit the generated random interger. For instance, the below modulo only returns int between 1-10
$ echo $(( $RANDOM % 10 + 1))
