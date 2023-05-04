---
title: "Shell Scripting Made Easy: A Comprehensive Guide for Beginners"
seoTitle: "Master Shell Scripting: A Beginner's Guide to Automating Linux and UNI"
seoDescription: "Learn the basics of shell scripting with this beginner-friendly guide, covering essentials like variables, conditionals, and loops to automate tasks"
datePublished: Thu May 04 2023 15:40:12 GMT+0000 (Coordinated Universal Time)
cuid: clh9an1h1000g09mecalg0di4
slug: shell-scripting-made-easy-a-comprehensive-guide-for-beginners
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1683214762246/2090a9c5-155f-4fb6-b57c-d91681702de1.jpeg
tags: bash, bash-script, kubesimplify, wemakedevs, devsintechblogs

---

# Introduction

Shell scripting is like crafting your very own command-line magic to make things happen in a terminal. It's an awesome way to automate tasks on Linux or UNIX systems. In this easy-peasy guide, we'll dive into the world of shell scripting, learn what it's all about, how it functions, and how you can jump right in. Let's get started!

# Prerequisite

Ready to dive into the world of shell scripting and create some command-line magic? Before we get started, make sure you're familiar with Linux or UNIX systems, comfy using the command line, and know your way around a text editor like Vim, Nano, or Emacs. Oh, and a little programming know-how will come in handy too. Let's jump right in!

![a diagram of a computer application](https://cdn.hashnode.com/res/hashnode/image/upload/v1683199428631/154efbcd-46b5-4ea3-9895-3fb84daeb56b.jpeg align="center")

Here you can see where the shell is working in our Operating System.

There are popular shells in Linux

1. C Shell (csh)
    
2. Kron Shell (ksh)
    
3. Z Shell(zsh)
    

# **Shebang #!**

This `#!` is called shebang. It is a special sequence of characters that are used in the first line of a script file to indicate the interpreter that should be used to execute the script. For example, the shebang line `#!/bin/bash` at the beginning of a Bash script tells the system to use the Bash interpreter to run the script.

This `#!/bin/bash` means that after this line while the program is in the bash script so you have to make sure that this is a Bash shell.

# Hello World

So this is the first program in every language that I have learnt so the program is

```bash
#!/bin/zsh
# This is a comment!
echo "Hello World!"
```

The first line (#!/bin/zsh) is the shebang line, which indicates that the script should be run using the Zsh shell interpreter.

The second line (# This is a comment!) is a comment. Comments are lines in the code that are not executed by the interpreter and are used to add explanatory notes to the code.

The third line (echo "Hello World!") is the actual command that is executed when the script is run. The echo command is used to print the string Hello World! to the terminal.

When you run this script, it will simply print the string <mark>Hello World! </mark> to the terminal.

# Variables

If you know the basics of programming then you have an idea about variables so I'm not going to detail about what is variable.

In Bash, you can define a variable by simply writing its name followed by an equal sign and the value you want to assign to it. For example, to create a variable named `my_var` with the value `hello`, you would write:

```bash
my_var="hello"
echo $my_var
```

Output :

`hello`

# **Conditionals**

You can use **conditional statements** in your shell script to decide what to do in response to a condition or test.

### If Statement

The `if` statement is used for conditional branching, where different code paths are executed depending on whether a condition is true or false.

The basic syntax for the `if` statement in Bash is as follows:

```bash
if [ condition ]
then
   # code to be executed if condition is true
fi
```

### If and else Statements

This is also similar to the if statements described above, but it additionally allows for a condition to be performed if the condition is not true. If the condition is false, the command or combination of commands () between else and fi will be run.

```bash
if [ <condition/test> ]
then
      <command1>
else
      <command2>
fi
```

### If elif else

This is used to work on different conditions statements.

```bash
if [ <condition1> ]
then
      <command1>
elif [ <condition2> ]
then
      <command2>
elif [ <condition3> ]
then
      <command3>
elif [ <condition4> ]
then
      <command4>
else
      <command>
fi
```

Loops For

```bash
for item in LIST #Starting for loop
do
COMMANDS #Write commands
done
```

Do while

```bash
do
   command1
   command2
   commandN
done
```

# Conclusion

In conclusion, shell scripting is a powerful tool for automating tasks on Linux and UNIX systems. By understanding the basics of shell scripting, such as variables, conditionals, and loops, you can create your own command-line magic and simplify complex tasks. With practice and dedication, you'll soon become proficient in this valuable skill.

And it's a wrap-up 🙂. I hope you have learned something from this blog. If it's helpful to you then do like ❤, follow🤝 me on [**Hashnode**](https://kelvin-parmar.hashnode.dev/), [**Twitter**](https://twitter.com/Kelvinparmar12), and [**GitHub**](https://github.com/kelvinparmar) subscribe to my Hashnode newsletter so that you don't miss any future posts. Thanks for reading and have a great day!