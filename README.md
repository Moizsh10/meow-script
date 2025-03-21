
# ᓚᘏᗢ
**Name:** meow

**Author:** Moizuddin Shah

**Date:** 12-11-2024

**Description:**

Adds a silly little cat to your terminal!

This script will print "meow" in the terminal when invoked alongside an emoticon of a cat. The type of meow and emoticon printed to the terminal are randomly selected. The script also has a couple options to print out ASCII art of cats to the terminal window as well.

## Help
Print some variation of \"meow\" onomatopeia alongside an emoticon of a cat in the terminal when invoked. Text and emoticon are randomly selected.

**Syntax:** meow [--freeman | {-h | --help} | {-l | large} | --shirley | {-v | --void} | {-V | --version}]

**options:**

--freeman

&emsp;Display ASCII art of Freeman and exit.

-h, --help

&emsp;Print this help and exit.

-l, --large

&emsp;Display a random, large ASCII art of a cat and exit.

--shirley

&emsp;Display ASCII art of Shirley and exit.

-v, --void

&emsp;Display ASCII art of a silly black cat and exit.

-V, --version

&emsp;Print the software version and exit. 

# Demo

[demo](https://dappercat.neocities.org/media/project_demos/meow_script_demoV2_5.gif)

# Installation

There's a couple things you need before you can use this script. First you have to ensure that your terminal configuration file has a PATH variable that leads to a directory where you have your scripts installed or want to install your scripts. As an example:

```
$ mkdir -p "$HOME/bin"
$ echo 'PATH="$HOME/bin:$PATH"' >> "$HOME/.bashrc"
$ source "$HOME/.bashrc"
```

Here, three things are happening/have been done

1. We created a directory named ``bin``
2. We wrote/added a line to the end of `.bashrc` (The BASH config file) file which exists in the ``$HOME`` directory. This line defines the PATH and tells `.bashrc` to look within the ``bin`` directory for any executable scripts if we run a command in the terminal before searching in other environments
3. We told BASH to re-read its configuration file to apply the changes we just made!

Then, to install you will simply extract the contents of the release and copy the `meow` script and the `cat_ASCII_art/` folder into the directory where you're keeping your scripts and make the script executeable by running

```
chmod +x meow
```

Now you can call the script and have silly little cat in your terminal!

## Adding More ASCII Art
The ASCII art used by the script is stored in the `cat_ASCII_art/` folder that should be in the same directory that you placed the `meow` script file. If you wanted to add more ASCII art to be randomly displayed when you use the `-l` or `--large` command you can easily do so by adding the ASCII art to the `cat_ASCII_art/` directory. The only things you need to do is ensure that the file you store the art in is a `.txt` file that starts with `large_cat_` (e.g. `large_cat_silly_cat.txt`). You don't need to worry about editing the script as it will be able to read how many files are in the folder and randomly select one to display.

