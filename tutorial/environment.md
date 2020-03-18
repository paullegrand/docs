# 0. Set Up Your Environment

We’ll start by installing Craft CMS directly on your computer in a local _development environment_.

Craft is a web application that needs to run on web server, and a local development environment provides that web server’s software on your personal workstation. This way, we can work with Craft freely and privately without the need to set up a hosting account.

To get up and running, we’ll need to get familiar with three tools:

1. The console utility that’s built into your operating system.
2. A local web server that meets [Craft’s minimum requirements](https://docs.craftcms.com/v3/requirements.html).
3. A code editor.

## Get to know your console

Every operating system comes with a text-based command line interface (CLI) for inputting commands. This provides a powerful way of doing lots of things beyond the graphical user interface you already know.

::: tip
If you’ve time traveled from the past, your operating system may _only_ have a command line interface. Our GUIs are going to blow your mind.
:::

We’ll be installing Craft with an application called [Composer](https://getcomposer.org/) that’s only available from the console—but don’t worry, it’s worth it!

### Find your OS console

TODO: add default icons and terminal screenshots from each OS

- On MacOS, the default console is Terminal.app.
- On Windows, the default console is called Command Prompt.
- On Ubuntu Linux, the default console is called Terminal.

There are other applications you can use like [Hyper](https://hyper.is/) (cross-platform) and [iTerm2](https://www.iterm2.com/) (Mac), but your system’s console will work just fine!

### Run a command

Once you’ve launched your console, you’ll be greeted by an empty prompt that’s ready for input.

Later on we’ll refer to “running” commands, in a format that look like this:

```bash
echo "hello world"
```

In this example, you would copy+paste or type `echo "hello world"` exactly as you see it above, then hit <kbd>return</kbd> or <kbd>enter</kbd> to execute the command. The result, or output, will be printed and you’ll be returned to the empty prompt.

The `echo` console command just repeats back whatever you pass to it. Here’s what you'd see after running that command:

```bash
echo "hello world"
hello world
```

Try it! Copy and paste `echo "hello world"` into your terminal and hit <kbd>return</kbd> or <kbd>enter</kbd>. If your console says “hello world” back, you know everything you need to run a terminal command!

### Navigate directories

We’ll eventually want to run commands alongside your site’s code, so you’ll need to know how to get there.

Every time you use the console, your commands will be executed from a specific folder on your system even when they’re not doing anything to files in that folder. This folder is called the _working directory_. You can change the working directory, much like you would using a file browser, using terminal commands.

To output the current working directory:

- Run `pwd` on Mac or Linux.
- Run `cd` on Windows.

This will print the current path you’re working in.

::: tip
The `pwd` command stands for “print working directory”, and `cd` stands for “current directory”. Commands like this are shortened so they’re quicker to type.
:::

To list the files in the current directory:

- Run `ls` on Mac or Linux.
- Run `dir` on Windows.

To move _up_ one directory, run `cd ..` on any platform.

To move _down_ into a specific directory, like `Documents`, use `cd Documents` on any platform.

To start at the topmost directory on your disk, use `cd /` on any platform.

To start from your user directory, use `cd ~` on Mac or Linux and `cd %HOMEPATH%` on Windows.

You can always use these commands to see where you’re at or move to a different folder on your machine.

Once you’re able to pick a folder and navigate to it, you’re all set!

## Choose a code editor

The files Craft installs on your computer are all stored in plain text.

There are a few benefits to plain text files, one being they’re extremely portable: you don’t need any special software to open and edit them, so anyone working with your site’s code could use whatever application they’d prefer. We’ll start editing a few of these files to configure our site, and others later to customize what it looks like.

While you could get away with using TextEdit.app, Notepad, or Text Editor, it’s a good idea to use a code editor because it’ll make things easier later on. Code editors...

- make it easy to work with multiple files
- add color coding and helpful tools depending on the file type you’re working with
- handle invisible characters like spaces and returns carefully, which can cause annoying problems across operating systems
- usually include convenient features and plugins for, as you might expect, working with code

An excellent, popular code editor is [Visual Studio Code](https://code.visualstudio.com/), which is available for free on MacOS, Windows, and Linux.

More advanced PHP developers tend to use [PhpStorm](https://www.jetbrains.com/phpstorm/), which is a more complex and specialized commercial Integrated Development Environment (IDE) specifically geared toward PHP development.

There are plenty of other options you’re free to use, just know that the rest of our steps and screenshots in this tutorial will assume you’re using VS Code.

## Set up a development environment

The word “environment” refers to the software that’s needed to work with Craft CMS, which is detailed in [Craft’s minimum requirements](https://docs.craftcms.com/v3/requirements.html).

Like your workstation, a web server can run different operating systems and applications. Web servers, however, are configured with an operating system and software for running websites. There are common combinations of web software referred to as “stacks”. (You’ve probably heard of a “full stack developer”, which means someone has experience with each of the software components in a particular stack.)

Craft can run on a number of different stacks, but the main ingredients are...

- **PHP**: the programming language in which Craft is written.
- **A database**: the place where content and most information is stored, sort of like a collection of Excel files used by code that can work with lots of data quickly. Commonly MySQL or PostgreSQL.
- **A web server**: the software that listens for requests made by your web browser, hands them off to a web application (like Craft), and gives a response back to the browser. Commonly Apache or nginx.

The best way to get working quickly is to use a pre-packaged web stack that runs on your operating system. The good news is that you’ve got plenty of options no matter what OS you’re using. The bad news is that the _best_ option depends on your OS and whatever software you’ve already installed.

Choose one of the following guides to set up a development environment on your OS.

::: warning
You won’t be able to set a web root until we get to installing Craft—skip that part and we’ll come back to it.
:::

TODO: write environment setup guides for each (must include creating a database + what settings Craft needs + how to run console commands + checking System Report requirements)

### MacOS, Windows, and Linux

- [Craft Nitro](#)
- [Laravel Homestead](#)
- [Vagrant](#)
- [DDEV](#)
- [Lando](#)

### MacOS

- [MAMP](#)
- [Laravel Valet](#)

### Windows

- [WAMP](#)
- [AMPPS](#)
- [XAMPP](#)

Once you’ve set up your local development environment, we’re ready to install Craft CMS!
