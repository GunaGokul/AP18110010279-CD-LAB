# AP18110010279-CD-LAB
CSE-306 Compiler Design Lab

# Week 1: Language recognizer

#      Write a program in C that recognizes the following languages.
1.     Set of all strings over binary alphabet containing even number of 0’s and even number of 1’s.
2.     Lab Assignment: Set of all strings ending with two symbols of same type.

# Week-2

1. Implement lexical analyser using C for recognizing the following tokens:
• 24 keywords (given in the following program)
• Identifiers with the regular expression : letter(letter | digit)*
• Integers with the regular expression: digit+
• Relational operators: <, >, <=, >=, ==, !=
• Ignores everything between multi line comments (/* .... */)
• Storing identifiers in symbol table.


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

# Week-5

1) Write a C program to compute the FIRST and FOLLOW functions for all non-terminals in a given grammar G. Assume that G is not left recursive. 

The input format and output formats were discussed in the lab session and also in the below Input format is given. 

Input format:  First read the number of productions and each production A -> B will be given as string A-B where A is a non-terminal and B is a string containing grammar symbols. The non-terminal in the head of the first production is the start symbol of the grammar. Further, a production A -> \epsilon is given as A-^. 

The last date to submit the assignment: 19 Oct 2020 at 10 PM. 


# Week-6

Lab Assignment: Implement Predictive Parser using C for the Expression Grammar
    E à TE’

    E’à +TE’ | ε

    T à FT’

    T’à *FT’ | ε

    F  à (E) | d

In the lab session, we have discussed the program (attached with this email) for the grammar 
    S -> aBa
    B -> bB | ε
 
with the assumption that the parse table is : 

|   | A      | B     | $ |
|---|--------|-------|---|
| S | S->aBa |       |   |
| B | B->E   | B->bB |   |
 

While implementing the algorithm for the above grammar in the assignment, first you construct the parse table by using the algorithm discussed in the class. This algorithm requires the computation of FIRST and FOLLOW functions. You have implemented this in the previous lab assignment. 

The due date for the submission: 03  Nov 2020 10:00 PM. 

# Week-7

1. non-recursive Predictive Parser for
   S -> aBa
   B -> bB | epsilon

2. non-recursive Predictive Parser for
    E → TE’
    E’→ +TE’ | epsilon  let A be E'
    T → FT’             let B be T'
    T’→ *FT’ | epsilon  
    F → (E) | d

# Week-8

1. . Shift Reduce Parser for
    E->E+E
    E->E*E
    E->(E)
    E->d

2. Shift Reduce Parser for
    S –> 0S0 | 1S1 | 2

# Week-9

1. E -> E+T |T
T-> T*F | F
F -> (E) | d

2. E -> E+E | E-E | E*E | E/E | -E | (E) | digit


