# AP18110010279-CD-LAB
CSE-306 Compiler Design Lab

# Week 1: Language recognizer

#      Write a program in C that recognizes the following languages.
1.     Set of all strings over binary alphabet containing even number of 0’s and even number of 1’s.
2.     Lab Assignment: Set of all strings ending with two symbols of same type.

# Week 3: Introduction to LEX tool

#      Implement the following programs using Lex tool
1.     Identification of Vowels and Consonants
2.     count number of vowels and consonants
3.     Count the number of Lines in given input
4.     Recognize strings ending with 00. 
5.     Recognize a string with three consecutive 0’s.

# Week-4 

1)  Implement lexical analyzer using LEX for recognizing the following tokens:
.   A minimum of 10 keywords of your choice

.   Identifiers with the regular expression : letter(letter | digit)*

.   Integers with the regular expression: digit+

.   Relational operators: <, >, <=, >=, ==, !=

.   Ignores everything between multi line comments (/* …. */)

.   Using files for input and output

2) Construct Recursive Descent Parser for the grammar using C program
    G = ({S, L}, {(, ), a, ,}, {S -> (L) | a ; L -> L, S | S}, S) and verify the acceptability of the following strings:

    (i)(a,(a,a))

    (ii)(a,((a,a),(a,a)))

    You can manually eliminate Left Recursion if any in the grammar.

    A reference C program for the grammar given below is attached. 

    E -> TE’

    E’+TE’ | ͼ

    T -> FT’

    T’ -> *FT’ | ͼ

    F -> (E) | i