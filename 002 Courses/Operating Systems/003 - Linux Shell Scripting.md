``` bash
# In a text file "simple.sh"
#!/bin/sh
# this is a comment
echo "The number of arguments is $#"
echo "The arguments are $*"
echo "The first is $1"
echo "My process number is $$"
echo "Enter a number from the keyboard: "
read number
echo "The number you entered was $number"
```

`#` - denotes that start of a comment
`#!` -
-  a special combination that tells LINUX to use the Bourne shell (sh)  to interpret the script.
- (called shebang) must be the first two characters of the script.
`$1, $2, $3 etc.` - arguments passed to the script can be accessed  through this commands.
`$*` - stands for all the arguments
`$#` - stands for the number of arguments
`$$`- process number of the shell executing the script
`read number` - assigns keyboard input to the variable number
