Tags: #CommandLine #Techniques

Being a master of the command line is a must for a developer. In this chapter, all of the notes about how to master the command line will exist. 

For more information about the command line (Link to be pasted soon) click this.

---
# Creating an empty file 

Tags: #CreateAFile

When creating a file in the command line, you must first access the directory to where you will create the file using the **cd** command and after that you can use this command to create an empty file.

```Command Line/PowerShell
type nul >> nameOfFile
```

After hitting the enter key, you can check by using the **dir** command if the file is successfully created in the directory.

---
# Launching a code project using the command line in visual studio code

Tags: #VSCode

Surprisingly you can launch your project in vs code using the command line! with a simple line you can access a project or a single file using these commanss.

```command line
code . // To access all the files in the current directory
code filenameHere // To access a certain file
```
