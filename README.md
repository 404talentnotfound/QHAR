basic rules of QHAR:

1: this language is based on a meme image that became an in-joke with my friend. it is in no way shape or form meant to be good, it is an esolang after all.
2: the only allowed characters are the characters in 'qhar' (both upper and lowercase are allowed), and '?!'.
3: no strings because fuck you (read line 11).
4: to make a QHAR program, make a file with the extension '.qhr'. to run that QHAR program, add the exe to your PATH (if you don't know how to, read https://gist.github.com/ScribbleGhost/752ec213b57eef5f232053e04f9d0d54 or look up a tutorial), then open a terminal in the directory of your qhr file and write 'qhar (NAME OF YOUR FILE).qhr'.
5: any file has to end with the string "QHAR?!?!" or it will loop back to the start.

now on to the specifics.

instead of strings you have every allowed character (read rule 2). capital 'Q', 'H', 'A' and 'R' are QHAR's equivilent to numbers 0 through 3, lowercase 'q' 'h' 'a' and 'r' are equivilent to numbers 4 through 7, and finally '?' and '!' are equivilent to numbers 8 through 9. now you may be thinking 'but those are just integers, not strings', well you'd be partially right, however most functions in QHAR only use numbers. but for the functions that you DO want to use strings with, i.e. the print function, you would make a string by writing a number that represents a character on the ascii table (if you can't find the number of your desired character, go to https://www.ascii-code.com/. the DEC section on the table is the number you're looking for).

qar = variable declaration. after the variable declaration keyword, write the name of the variable (remember, rule 2 applies here too), after that write wether you want to make a new variable, subtract from a variable or add to a variable ('!', '!?' or '?!'). if you want to create a new variable, the third argument will be what the value of the variable will be (again, rule 2). for subtraction the third argument will be what you subtract from the value of the variable and vice versa for the addition.

qhar? = user input. the user will be able to input text, that text will be assigned to a new variable.

!! = goto line. after the 2 exclaimation marks, write the line number you want to be repeating from.

?? = if statement. after writing the 2 question marks, write whether you want to check if a value should be equal, less, or more to the following argument. equal to is represented as '!!', less than is represented as '!?', and more than if represented as '?!'. after that the final argument is index of the line of code you're checking. the line of code you're checking has to be a variable declaration. the if statement is checking the status of the variable on the line of code you specified. to check if a variable is equal to an integer, you first have to declare the variable to that integer, then make an if statement where the third argument is the line of code that declares that variable as the integer you want to compare it to.

! = print function. the print function can only print a variable. there are two different modes, 'q' and 'r'. the 'q' mode prints the number assigned to the variable you're printing, and the 'r' mode prints the character with the index of the number assigned to variable you're printing on the ascii table, i.e. a variable assigned to the number 97 in the 'r' mode would print the letter 'a' (which is the 97th character in the ascii table). rather than inputting the name of a variable, you have to print the index of that variable in the script. for example if there's three variables, to print the number assigned to third variable from the top, you would have to say '! q A'.

?!?! = comment lines. the text you put after this will be ignored, has to be on a seperate line and rule 2 still applies however in this case the uppercase characters aren't allowed for limited communication.

good luck...