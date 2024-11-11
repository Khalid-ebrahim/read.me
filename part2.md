# How to create a file in the linux using the Terminal?

##### In this article, we will learn to create a file in the Linux/Unix system using the terminal. In the Linux/Unix system, there are the following ways available to creating files.

> 1.  Using the touch command.
> 2.  Using the cat command
> 3.  Using redirection operator
> 4.  Using the echo command
> 5.  Using the heredoc
> 6.  Using the dd command

## 1. Create a file in the Linux/Unix system using the touch command.

###### The touch command is used to create file/files without any content and update the access date or modification date of a file or directory in the Linux system. This is the simplest way to create a file in Linux/Unix using the terminal.

**Syntax**:

##### The general syntax of the touch command is as follows:

`$ touch [option] ... FILE...`

## 2. Create a File in the Linux/Unix system using the cat command.

###### The cat (concatenate) command is used to create, view, concatenate files in the Linux operating system. The touch command is also used to create a file in a Linux system without content whereas the cat creates files with some content. The cat command reads the content of a file and prompts it.

### **Syntax**

### The general syntax of the cat command is as follows:

```
$ cat [option]... FILE...
```

![](https://media.geeksforgeeks.org/wp-content/uploads/20210401081516/2.png)

## 3. Create a file in the Linux/Unix system using a redirection operator.

### In the Linux/Unix system a redirection operator is also used to create a file.

**Example :**

```
$  > file.txt
```

![ ](https://media.geeksforgeeks.org/wp-content/uploads/20210402082202/4.png)

## 4. Create a file in the Linux/Unix system using the echo command.

###### The echo command is also used to create a new file in the Linux system.

###### Create a new file without contents in the Linux system using the echo command.

###### To create a file without contents, we use the echo command with a redirection operator followed by the file name as shown below.

**Example :**

```
$ echo > file.txt
```

![](https://media.geeksforgeeks.org/wp-content/uploads/20210402081258/0.png)

## 5. Create a file in the Linux/Unix system using heredoc.

###### heredoc stands for here document. The heredoc delimiter is a type of redirection. It allows passing multiple lines of input to a command.

###### The general syntax of heredoc. Important

```
Command << Heredoc_delimiter
multiple lines contents...
heredoc_delimiter
```

###### Create a file with multiple lines of contents using a heredoc delimiter in the Linux system.

###### To create a file using heredoc, we use the cat command with heredoc delimiter in the Linux system as shown below.

**Example :**

```
$ cat  << heredoc_delimiter < file_name
```

![](https://media.geeksforgeeks.org/wp-content/uploads/20210403202038/12.png)

## 6. Create a file in the Linux/Unix system using the [dd command](https://www.geeksforgeeks.org/dd-command-linux/).

###### The dd command is mainly used to converts and copy files. To check more details about the dd command. We can also create a large file using the dd command.

###### Create a large file in the Linux system using the dd command.

###### To create a large file, we use the dd command as shown below.

**Example :**

```
$ dd if = /dev/zero of = file.test bs =1 count =0 seek = 2G
```
