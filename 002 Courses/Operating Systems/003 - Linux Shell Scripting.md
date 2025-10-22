# Basic Scripting

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

``` bash
ls -l simple.sh
chmod +x simple.sh
./simple.sh
```

`ls -l simple.sh`- used to list the detailed information for the file simple.sh
`chmod +x simple.sh`- make the simple.sh executable which is indicated by the 'x' when you list the file.
`./simple.sh`- run the executable

``` bash
echo 5 | ./simple.sh hello world
```

The script would produce similar output but would not pause to read a number from the keyboard.

---
# Advance Scripting

```bash
# if-then-else statements
if [ test ]
then
commands-if-test-is-true
else
commands-if-test-is-false
fi
```

`-s file`- true if file exists and is not empty
`-f file`-  true if file is an ordinary file
`-d file`- true if file is a directory
`-r file`- true if file is readable
`-w file`- true if file is readable
`-x file`- true if file is executable
`$X -eq $Y`-true if X equals Y
`$X -ne $Y`-true if  not equal to Y
`$X -lt $Y`-true if X less than Y
`$X -gt $Y`-true if X greater than Y
`$X -le $Y`-true if X is less than or equal to Y
`$X -ge $Y`-true if X is greater than or equal to Y
`"$A" = "$B"`-true if string A equals string B
`"$A" != "$B"`-true if string A is not equals string B
`$X ! -gt $Y`-true if string X is not greater than Y
`$E -a $F`-true if expressions E and F are both true
`$E -o $F`-true if either expression E or expression F is true


