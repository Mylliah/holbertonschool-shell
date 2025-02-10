###---- Task 0 :

	Command used to print "Hello, World", followed by a new line to the standard output :
	echo 'Hello, World'

###---- Task 1 : 

	Command used to print a confused smiley :
	echo "\"(Ôo)'"

###---- Task 2 :

	Command used to print the content of a distant directory :
	cat /etc/passwd

###---- Task 3 :

	Command used to print the content of two distants directories : 
	cat /etc/passwd /etc/hosts

###---- Task 4 :

	Command used to print the last 10 lines of a file :
	tail /etc/passwd

###---- Task 5 :

	Command used to print the first 10 lines of a file : 
	head /etc/passwd

###---- Task 6 :

	Command used to display the third line of a file : 
	head -3 iacta | tail -1

###---- Task 7 :

	Command used to create a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line :
	echo -e "Best School" >> "\\*\\\\'\"Best School\"\\'\\\\*$\\?\\*\\*\\*\\*\\*:)"	

###---- Task 8 : 

	Command used to write into a file the result of a command :
	ls -la > ls_cwd_content

###---- Task 9 :

	Command used to duplicates the last line of a file : 
	tail -1 iacta >> iacta

###---- Task 10 : 
	
	Command used to delete all the regular files with a .js extension that are present in the current directory and all its subfolders : 
	find . -type f -name "*.js" -delete

###---- Task 11 :

	Command used to count the numer of directories and sub-directorues in the current directory :
	find -type d ! -path . | wc -l    OU   find . -mindepth 1 -type d | wc -l

###---- Task 12 :

	Command used to display the 10 newest files in a current directory : 
	ls -t | head

###---- Task 13 :

	Command used to take a list of words as input and prints only words that appear exactly once : 
	sort list | uniq -u

###---- Task 14 : 

	Command used to display lines containing a pattern from the file /etc/passwd
	grep 'root' /etc/passwd

###---- Task 15 :

	Command used to display the number of lines that contain a pattern in a file :
	grap 'bin' /etc/passwd | wc -l

###---- Task 16 :

	Command used to display lines containing a pattern and 3 lines after them in a file :
	grep -A 3 'root' /etc/passwd

###---- Task 17 : 

	Command used to display all the lines in a file that do not contain a pattern :
	grep -v 'bin' /etc/passwd






