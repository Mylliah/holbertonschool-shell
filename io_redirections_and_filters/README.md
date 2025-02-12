### ---- Task 0 :

	Command used to print "Hello, World", followed by a new line to the standard output :
	echo 'Hello, World'

### ---- Task 1 : 

	Command used to print a confused smiley :
	echo "\"(Ôo)'"

### ---- Task 2 :

	Command used to print the content of a distant directory :
	cat /etc/passwd

### ---- Task 3 :

	Command used to print the content of two distants directories : 
	cat /etc/passwd /etc/hosts

### ---- Task 4 :

	Command used to print the last 10 lines of a file :
	tail /etc/passwd

### ---- Task 5 :

	Command used to print the first 10 lines of a file : 
	head /etc/passwd

### ---- Task 6 :

	Command used to display the third line of a file : 
	head -3 iacta | tail -1

### ---- Task 7 :

	Command used to create a file named exactly \*\\'"Best School"\'\\*$\?\*\*\*\*\*:) containing the text Best School ending by a new line :
	echo -e "Best School" >> "\\*\\\\'\"Best School\"\\'\\\\*$\\?\\*\\*\\*\\*\\*:)"	

### ---- Task 8 : 

	Command used to write into a file the result of a command :
	ls -la > ls_cwd_content

### ---- Task 9 :

	Command used to duplicates the last line of a file : 
	tail -1 iacta >> iacta

### ---- Task 10 : 
	
	Command used to delete all the regular files with a .js extension that are present in the current directory and all its subfolders : 
	find . -type f -name "*.js" -delete

### ---- Task 11 :

	Command used to count the numer of directories and sub-directorues in the current directory :
	find -type d ! -path . | wc -l    OU   find . -mindepth 1 -type d | wc -l

### ---- Task 12 :

	Command used to display the 10 newest files in a current directory : 
	ls -t | head

### ---- Task 13 :

	Command used to take a list of words as input and prints only words that appear exactly once : 
	sort list | uniq -u

### ---- Task 14 : 

	Command used to display lines containing a pattern from the file /etc/passwd
	grep 'root' /etc/passwd

### ---- Task 15 :
 
	Command used to display the number of lines that contain a pattern in a file :
	grap 'bin' /etc/passwd | wc -l

### ---- Task 16 :

	Command used to display lines containing a pattern and 3 lines after them in a file :
	grep -A 3 'root' /etc/passwd

### ---- Task 17 : 

	Command used to display all the lines in a file that do not contain a pattern :
	grep -v 'bin' /etc/passwd

### ---- Task 18 :

	Command used to display all lines of a file starting with a letter :
	grep '^[[:alpha:]]' /etc/ssh/sshd_config

### ---- Task 19 :

	Command used to replace all specifics characters A and c input to z and e respectively :
	tr 'A' 'Z' | tr 'c' 'e'

### ---- Task 20 :

	Command used to remove all specifics letters from input :
	tr -d 'C' | tr -d 'c'

### ---- Task 21 :

	Command used to reverse its input :
	rev

### ---- Task 22 :
	
	Command used to display all users and their home directories, sorted by users :
	cat /etc/passwd | cut -d ':' -f1,6 | sort -t ':' -k1

### ---- Task 23 :

	Command used to find all empty files and directories in the current directory and all sub-directories.
	->Only the names of the files and directories should be displayed (not the entire path)
	->Hidden files should be listed
	->One file name per line
	->The listing should end with a new line
	cat /etc/passwd | cut -d ':' -f1,6 | sort -t ':' -k1

### ---- Taske 24:

	Command used to list all the files with a .gif extension in the current directory and all its sub-directories.
	->Hidden files should be listed
	->Only regular files (not directories) should be listed
	->The names of the files should be displayed without their extensions
	->The files should be sorted by byte values, but case-insensitive (file aaa should be listed before file bbb, file .b should be listed before file a, and file Rona should be listed after file jay)
	->One file name per line
	->The listing should end with a new line
	find . -empty -printf '%f\n'
	find . -type f -name "*.gif" | rev | cut -d/ -f1 | cut -d . -f 2- | rev | LC_ALL=C sort -f

### ---- Task 25 :

	Command used to decode acrostics that use the first letter of each line.
        The 'decoded' message has to end with a new line :	
	cut -c1 | tr -d '\n' | cut -f1

### ---- Task 26 :

	Command used to parse web servers logs in TSV format as input and displays the 11 hosts or IP addresses which did the most requests.
        ->Order by number of requests, most active host or IP at the top	
	tail -n +2 | cut -d$''' ''' -f1 | sort --ignore-case | uniq -c | sort --ignore-case -nr | head -11 | rev  | cut -d''' ''' -f1 | rev






