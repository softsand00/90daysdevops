# Day 4 Task: Basic Linux Shell Scripting for DevOps Engineers

## 1. What is Kernel?
A kernel is the core part of an operating system. 
It manages the system's resources, such as the CPU, memory, and hardware devices, and allows software programs 
to communicate with the hardware. Think of it as a bridge between your computer's hardware and software.

## 2. What is Shell?
A shell is a user interface that allows you to interact with the operating system. It's where you type commands to run programs, manage files, 
or perform other tasks. Think of it as a translator that takes your instructions and tells the operating system what to do.

## 3. What is Linux Shell Scripting?
Linux shell scripting is the process of writing a series of commands in a file (a script) that the shell can execute one by one. It's like creating a recipe for the 
computer to follow, automating tasks that you would normally do manually in the command line. This makes it easier to manage repetitive tasks,
run complex sequences of commands, or even create small programs.

## 4. Explain in your own words and with examples what Shell Scripting means for DevOps
In DevOps, shell scripting is like creating a set of automated instructions that help manage and streamline the development and operations processes

## 5. What is #!/bin/bash? Can we write #!/bin/sh as well?
#!/bin/bash and #!/bin/sh are both > shebang < lines used at the beginning of a shell script to specify which shell interpreter should be used to execute the script
* Bash (Bourne Again SHell) is a popular and powerful shell that provides advanced features and functionalities compared to other shells.
* sh is the original Unix shell, and it's more basic compared to Bash. However, it is widely supported and used for portability across different Unix-like systems.

## 6. Write a Shell Script that prints I will complete #90DaysOfDevOps challenge
   Create a file
   echo "I will complete #90DaysOfDevOps challenge "
   
## 7. Write a Shell Script that takes user input, input from arguments, and prints the variables.
   #!/bin/bash

# Take input from command-line arguments
arg1=$1
arg2=$2

# Prompt the user for input
echo "Enter a value for user_input1:"
read user_input1

echo "Enter a value for user_input2:"
read user_input2

# Print the values
echo "Command-line Argument 1: $arg1"
echo "Command-line Argument 2: $arg2"
echo "User Input 1: $user_input1"
echo "User Input 2: $user_input2"

## Provide an example of an If-Else statement in Shell Scripting by comparing two numbers.
Step one -Create a file like filename.sh<br>
Step two - check file permission by command - ls -l filename.sh
step three - Change the file permission by command - chmod 700 filename.sh
step four - To run file - ./ifelse.sh
Code :
#!/bin/bash

echo "Enter a value for user_input1:"
read num1

echo "Enter a value for user_input2:"
read num2

if [ $num1 -gt $num2 ]; then
    echo "The number 1 is greater."
else
    echo "The number 2 is greater or equal."
fi
