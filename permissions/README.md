### ---- Task 0 : 

	Command used to switch the current user to the user betty : 
	su betty

### ---- Task 1 : 

	Command used to prints the effective username of the current user :
	whoami

### ---- Task 2 :

	Command used to prints all groups the current user is part of :
	groups

### ---- Task 3 :

	Command used to change the owner of a file :
	chown betty hello

### ---- Task 4 :

	Command used to create an empty file :
	touch

### ---- Task 5 :

	Command used to add execute permission to the owner of a file :
	chmod u+x hello

### ---- Task 6 :

	Command used to add execute permission to the owner of a file + groups, and add read permission to the others : 
	chmod ug+x,o+r hello

### ---- Task 7 :

	Command used to add execute permission to the owner of a file + groups + others (everybody): 
	chmod ugo+x hello

### ---- Task 8 :

	Command used to add all permission to the others and not permission at all to the owner and groups :
	chmod 007 hello

### ---- Task 9 :

	Command used to set sprecifics permissions to a file :
	chmod 753 hello

### ---- Task 10 :

	Command used to copy same permissions 'from' a file 'to' an other file : 
	chmod --reference=olleh hello

### ---- Task 11 : 

	Command used to add execute permission to all subdirectories of the current directory for the owner, the group owner and all other users. 
	Regular files should not be changed :
	chmod -R +X .

### ---- Task 12 : 

	Command used to create a directory with permissions in the same time :
	mkdir -m 751 my_dir

### ---- Task 13 : 

	Command used to change group owner of a line : 
	chown root:school hello

### ---- Task 14 :

	Command used to change user owner et group owner in a same time for all directories and files : 
	chown -R vicent:staff /tmp

### ---- Task 15 : 
	
	Command used to change the owner and the group owner of a file with symbolic link to vincent and staff respectively :
	chown -h vincent:staff _hello

### ---- Task 16 : 

	Command used to change the owner of a file to vincent only if it is owned by user guillaume :	
	chown --from=guillaume vincent hello 




