# 0x16. C - Simple Shell

## Description

This Simple Shell project is a collaboration between Software Engineers Bello Abayomi A. and Adetola Rosemary, both of whom are ALX students. The goal of this project is to create our own UNIX command interpreter (Shell).

The basic function of the Simple shell program, which may be constructed and run from the command line, is to execute instructions read from standard input.

## Shell Compilation
	$ gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
## Shell execute
	./hsh

## Commands on shell process
	cd - Change directory
	env - List the current enviroment variables
	exit - exit the shell
	pwd - Print the absolute pathname

## Files
Description of the files used:

| Files | Description             |
| --------- | ------------------- |
| _calloc.c  | Function that allocates memory |
| _cd.c    | Function that changes to the directory of the process |
| _ex.c    | Function that finds if input is esit, therefore terminates process |
| _fork.c | Function that creates process and executes |
| _getline.c | Function that reads what the user writes |
| _signal.c | Function that handles the SIGINT signal |
| _writerr.c | Function that gets each error |
| checkbin.c | Function that checks if commands exits in the PATH |
| gridfree.c | Function that free an array of arrays |
| parser.c | Function that creates an array of pointers depending on the delimit characters used |
| sshell.c  | Main function that starts the shell |
| shell. h  | Header file with all the functions prototypes |


## Examples

Some of the examples of this shell working process:

cd:

	^_^ pwd
	/home/vagrant/simple_shell
	^_^ cd
	^_^ pwd
	/home/vagrant
	^_^

cd error:

	^_^ cd hola
	./hsh: 1: cd: can't cd to hola
	^_^

exit:

	^_^ exit 123
	vagrant@vagrant-ubuntu-trusty-64:~/simple_shell$ echo $?
	123

exit error:

	^_^cisfun$ exit hola
	./hsh: 2: exit: Illegal number: hola
	^_^

## Authors
- Bello Abayomi A. <ayodeleadetolarosemary@gmail.com>
- Adetola Rosemary <a.bello143@yahoo.com>
