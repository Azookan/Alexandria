Parser is a last-resort program to strictly read files affected by type B corruption. We say that the corruption is of type B if Lentil is unable to recover it. Parser's methods are mutating, so it cannot be used on minorly corrupted files which Lentil can handle. As a protective measure, therefore, Parser prevents the user from reading files which are not of a type B corruption (such as files which are not corrupted to begin with, or files with type A corruption).

Syntax usage: run parser on <filename>

Parser often returns output in the form of a grid pack. A grid pack is a grid with letters on one axis, numbers on another axis, and squares that are filled in with numbers. More formally, a grid pack is a 5-tuple (A, B, L, f, g) where:

A = set of valid letters
B = set of valid integers
L = the null set, or set of invalid letter-number combinations
f = function mapping from A to a statement
g = function mapping from B to a statement

Consider any item inside the set of valid-letter combinations. This item can be represented as a coordinate pair of some letter x and some number y, written as (x,y).

We define a solution to (x,y) as an integer so that both f(x) and g(y) are satisfied. We say that a grid pack is decoded when for every valid combination (x,y) in a grid pack, we have found its solution. Convert each solution via a1z26 and unscramble the solutions to form a phrase, which is called the decoding. As an example, see the file test3. The decoding of test3's grid pack should be 'abc'.

Note that there can be multiple solutions, and thus, multiple decodings. Often, however, only one decoding is acceptable.