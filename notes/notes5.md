# The Basics of Nano

Nano is by default included in most Linux distributions. However, if necessary, the installation process can be completed in two steps.

1. First, open the terminal and update the apt repositories with the command:

sudo apt update
2. Then, install Nano by running the command:

Debian/Ubuntu:

sudo apt install nano
CentOS/Fedora:

yum install nano
With this, you have successfully installed the text editor.

How to Open, Create, and Edit Nano Files
There are several ways to open the text editor.

As it is a command-line editor, the first step is to open the terminal. The easiest way to access the terminal is the Ctrl+Alt+T shortcut.

Create a New File
To open a new blank Nano file, run the command: nano

When you decide to exit (Ctrl+X), it will ask whether to save or discard the file.

do you want to save of discard file

If you press y to save the file, it will ask you to name the file. Type in a name and press Enter.

In this example, the name is file1.php.

example of saving a file

Open an Existing File
To open an existing file, add the file name to the command. For example, if the file is called file1.php, the command will be:

nano file1.php
However, to open a file in another directory, you must include the path in which the file is located:

nano /path/to/file1.php
It is also possible to open a file and directly go to a specific line or column.

nano +line,column file1.php
Edit Files in Nano
What makes Nano so attractive is that it has an easy graphical user interface (GUI), allowing users to directly interact with the text. There is no need to switch to an edit mode, like in Vim.

You can directly write, edit and navigate through content and receive immediate on-screen feedback.

Nano Command Keyboard Shortcuts
Control Characters and Keys
There are keyboard combinations for each function in Nano. Control shortcuts (used with the Ctrl button) are represented by a carat (^) followed by a symbol.

For example, the shortcut to Exit out of the Nano text editor is Ctrl+X (displayed as ^X).

In addition, there are combinations that require the Meta key (usually the Alt button). They are represented by the letter M followed by a symbol.

For example, the shortcut to Undo an action in a text is Alt+U (displayed as M-U).

The two bottom lines in the text editor will display some of the most commonly used shortcuts, as seen in the image below.

viewing the shortcuts available at the bottom of the screen

To see all valid shortcuts, press Ctrl+G (displayed as ^G) or F1. This will open Nano’s help text and list all possible keystrokes.

screenshot of the main nano help page with all text commands

Note: Do not use the Shift button in Nano. All shortcuts use unmodified numbers and lowercase letters.

When dealing with a large file, it is helpful to know how to quickly navigate through the text. Nano allows you to do this either by using the arrow keys or keyboard shortcuts.

Useful keyboard shortcuts for navigating include:

move forward one character: Ctrl+F (^F)
move back one character: Ctrl+B (^B)
move forward one word: Ctrl+Space (^Space)
move back one word: Alt+Space (M-Space)
move to the previous line: Ctrl+P (^P)
move to the next line: Ctrl+N (^N)
move to the next page: Ctrl+V (^V)
move to the previous page: Ctrl+Y (^Y)
move to the beginning of the line: Ctrl+A (^A)
move to the end of the line: Ctrl+E (^E)
Search a Text File
To search for a particular word or part of a text inside the editor, use the “where is” option with the Ctrl+W shortcut (^W). This will open a search prompt where you can type in the text you want to find. To continue to the next result, use Alt+W (M-W).

The search bar can also find specific line numbers. Press Ctrl+T (^T) while in it and the line number you want to find.

Regex Searches
You can also search with regex (regular expressions). These represent a search pattern defined by a sequence of characters. To do so, use the Alt+R shortcut (M-R).

Replace Text
To replace text in the file, first open the search bar with Ctrl+W (^W) and then press Ctrl+R (^R). It will open a search bar to type in what you want to replace, as seen in the image below.

example of replacing text inside nano

After you have selected the search item, it will ask what you want to replace it with.

selecting text to be replaced

Select, Copy, Cut and Paste Text
To select part of a file, navigate to the beginning of the text, press the Alt+A shortcut (M-A) and use the arrow keys to move over the text you wish to select.

Next, you can copy the selected text with the Alt+6 combination (M-6) or cut with Ctrl+K (^K). If you use these shortcuts without selecting any text prior, it will copy or cut the entire line of text.

To paste text, use Ctrl+U (displayed as ^U).

Insert Another File Into the Current One
While editing a file in Nano, it is possible to insert the entire contents of another file into the current one with the Ctrl+R (^R) shortcut.

This command will open the bottom bar in which you must write the path and file name you wish to import.

inserting contents of another file command

Spell Check in Nano
Nano also offers a spell checking feature. However, to enable it you must install the spell package.
To install the spell package, run the following command in the terminal:

sudo apt install spell
After installing the package, you can spell check in the text editor by pressing Ctrl+T (^T). It will select the misspelled word and ask for a correct replacement.

In the image below, the words underlined are misspelled.

spell checking in nano, replacement errors

Save a File
To save a file, use the Ctrl+O (^O) keyboard combination. It will ask you to enter a file name or confirm the name of an existing file.

Once it is saved, the status bar will indicate the number of lines that the file has.

display of the number of text lines saved

It can also create a backup of a file if you need to store temporary copies of the same file. To do this, use the Alt+B command (M-B). Pressing the keys once will enable backup and doing it again will disable it.

Exit
To exit out of Nano, press Ctrl+X (Nano displays it as ^X).

# The Basics of Vim
In Vim, you can save a file without your hands leaving the keyboard, and sometimes without even leaving the home keys. From Vim’s insert mode, hit Escape and then :w. That’s all. More on that later.
* The first thing you’ll want to learn is how to move around a file. When you’re in command mode, you’ll want to remember the following keys and what they do:
h moves the cursor one character to the left.
j moves the cursor down one line.
k moves the cursor up one line.
l moves the cursor one character to the right.
0 moves the cursor to the beginning of the line.
$ moves the cursor to the end of the line.
w move forward one word.
b move backward one word.
G move to the end of the file.
gg move to the beginning of the file.
`. move to the last edit.

* A longer list of the commands you’ll definitely want to know starting out:

d starts the delete operation.
dw will delete a word.
d0 will delete to the beginning of a line.
d$ will delete to the end of a line.
dgg will delete to the beginning of the file.
dG will delete to the end of the file.
u will undo the last operation.
Ctrl-r will redo the last undo.

* The commands you most need to start out:

v highlight one character at a time.
V highlight one line at a time.
Ctrl-v highlight by columns.
p paste text after the current line.
P paste text on the current line.
y yank text into the copy buffer.

To write the file you’re editing, enter w. (So, you’ll have :w.) That will write the file to the existing filename. If you don’t have a filename or want to write out to a different filename, use :w filename.

To quit Vim after you’ve finished, hit :q. Since Vim is your friend, it won’t just pop out on you if you haven’t saved your file. It will say “no write since last change,” and suggest that you add ! to override.