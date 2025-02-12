### ---- Task 0 :

	Command used to create an alias :
	alias ls ='rm *'

### ---- Task 1 :

	Command used to print a hello user, where user is the current Linux user : 
	echo hello $USER

### ---- Task 2 :

	Command used to add a directory to the PATH, where the directory should be last directory the shell looks into when looking for a program : 
	export PATH="$PATH:/action"

### ---- Task 3 :

	Command used to count the number of directories in the PATH :
	echo $(printf $PATH | tr ':' '\n' | wc -w)

### ---- Task 4 :

	Command used to list environment variables :
	printenv

### ---- Task 5 : 
	
	Command used to list all local variables and environment variables, and functions :
	set | less

### ---- Task 6 :

	Command used to create a new local variable :
	BEST=School

### ---- Task 7 :

	Command used to create a new global variable : 
	export BEST=School

### ---- Task 8 :

	Command used to print the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line :
	echo $((${TRUEKNOWLEDGE +128))
	 
### ---- Task 9 :

	Command used to print the result of POWER divided by DIVIDE, followed by a new line :
	echo $((${POWER} / ${DIVIDE}))

### ---- Task 10 :

	Command used to display the result of BREATH to the power LOVE : 
	echo $(($BREATH ** $LOVE)) | cat

### ---- Task 11 :

	Command used to converts a number from base 2 to base 10 : 
	echo $((2#$BINARY))

### ---- Task 12 :

	Command used to print all possible combinations of two letters, except oo :
	echo {a..z}{a..z} | tr ' ' '\n' | grep -v oo

### ---- Task 13 :

	Command used to print a number with two decimal places, followed by a new line :
	printf "%.2f\n" $NUM

### ---- Task 14 : 

	Command used to converts a number frome base 10 to base 16 :
	printf "%x\n" $DECIMAL

### ---- Task 15 :

	(article)

### ---- Task 16 : 

	Command used to encode and decode text using the rot13 encryption. Assume ASCII :
	tr 'A-Za-z' 'N-ZA-Mn-za-m'	

### ---- Task 17 :

	Command used to print every other line from the input, starting with the first line :
	paste - - | cut -f1
	

### ---- Task 18 : 

	Command used to add the two numbers stored in the environment variables WATER and STIR and prints the result :
	printf '%o\n' $(( 5#$( echo $WATER | tr water 01234) + 5#$( echo $STIR | tr stir. 01234 ) )) | tr 01234567 bestchol	






