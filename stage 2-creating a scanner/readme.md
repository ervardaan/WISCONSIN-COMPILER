link: https://pages.cs.wisc.edu/~hasti/cs536/assignments/p2/p2.html

For this assignment you will use JLex to write a scanner for a language called base, which is based on a small subset of a C++like language. Features of base that are relevant to this assignment are described below. You will also write a main program (P2.java) to test your scanner. 
# working with JLEX

A lexical analyzer breaks an input stream of characters into tokens. Writing lexical analyzers by hand can be a tedious process, so software tools have been developed to ease this task.

Perhaps the best known such utility is Lex. Lex is a lexical analyzer generator for the UNIX operating system, targeted to the C programming language. Lex takes a specially-formatted specification file containing the details of a lexical analyzer. This tool then creates a C source file for the associated table-driven lexer.

The JLex utility is based upon the Lex lexical analyzer generator model. JLex takes a specification file similar to that accepted by Lex, then creates a Java source file for the corresponding lexical analyzer.
