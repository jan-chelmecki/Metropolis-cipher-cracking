# Metropolis cipher cracking

This is a student project implementing a Markov chain attack on a simple substitution cipher (i.e. one for which the key is some permutation of the alphabet).

It was inspired by the lecture notes Probability and Computing by Ryan O'Donnell (Fall 2009 version, page 147 in the pdf), link here:

https://www.cs.cmu.edu/~odonnell/papers/probability-and-computing-lecture-notes.pdf

As the message is short, the naive letter frequency approach does not help to crack the cipher. We proceed by definining a quality score for each possible key (permutation)
and performing a random walk in the space of all permutations in order to select from a stationary distribution tailored to favorise those keys that decipher a message
into a string whose bigram frequencies are similar to that of the English language.
