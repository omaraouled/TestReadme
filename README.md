# my_ls: A simplified version of the Unix ls command
This project implements a custom my_ls command in C that replicates the basic functionality of the standard ls command.

## Features
•	Lists directory contents.
•	Supports long listing format (-l) to display file permissions, owner, group, size, and last modification time.
•	Shows hidden files (-a).

### Compiling and Running
1.	Compile the code using: gcc -o my_ls my_ls.c
2.	Run the program with various options:
      •	./my_ls: List current directory contents.
      •	./my_ls -l: List current directory contents with long format.
      •	./my_ls -a: List current directory contents including hidden files.
  	
#### Code Structure
The code is organized into two main parts:
1.	Helper Functions:
      •	print_error: Prints an error message and exits the program.
      •	print_file_info: Formats and prints detailed information about a file based on its stat structure.
2.	Main Function:
      •	Parses command-line arguments for options (-l, -a) and the target directory.
      •	Calls list_directory to handle directory listing with the specified options.

