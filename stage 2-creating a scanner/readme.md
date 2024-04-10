link: https://pages.cs.wisc.edu/~hasti/cs536/assignments/p2/p2.html

For this assignment you will use JLex to write a scanner for a language called base, which is based on a small subset of a C++like language. Features of base that are relevant to this assignment are described below. You will also write a main program (P2.java) to test your scanner. 
# working with JLEX

A lexical analyzer breaks an input stream of characters into tokens. Writing lexical analyzers by hand can be a tedious process, so software tools have been developed to ease this task.

Perhaps the best known such utility is Lex. Lex is a lexical analyzer generator for the UNIX operating system, targeted to the C programming language. Lex takes a specially-formatted specification file containing the details of a lexical analyzer. This tool then creates a C source file for the associated table-driven lexer.

The JLex utility is based upon the Lex lexical analyzer generator model. JLex takes a specification file similar to that accepted by Lex, then creates a Java source file for the corresponding lexical analyzer.

# JLEX SPECIFICATIONS
JLex Specifications
A JLex input file is organized into three sections, separated by double-percent directives (``%%''). A proper JLex specification has the following format.
user code
%%
JLex directives
%%
regular expression rules
The ``%%'' directives distinguish sections of the input file and must be placed at the beginning of their line. The remainder of the line containing the ``%%'' directives may be discarded and should not be used to house additional declarations or code.

The user code section - the first section of the specification file - is copied directly into the resulting output file. This area of the specification provides space for the implementation of utility classes or return types.

The JLex directives section is the second part of the input file. Here, macros definitions are given and state names are declared.

The third section contains the rules of lexical analysis, each of which consists of three parts: an optional state list, a regular expression, and an action.
