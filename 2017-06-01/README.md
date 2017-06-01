# Our Inaugural Meetup

## Outline

Some tips for everyone, regardless of their current exposure to Vim.

As for a file we can use to play with, we can use [oo-in-js.md](oo-in-js.md). It has a bit of code and text in it so we can play with both scenarios.


### Why Vim?

* Developer efficiency
* No need for a mouse - hands stay on the home row keys
* Already installed on *nix and Mac systems
* Available when you SSH into a machine


### Beginner

The basic commands in each mode. Many of these should also be available in vim-mode of most other editors (Atom, Visual Studio [Code], Sublime Text, etc).

* `:help`
* `:Tutor` Do this! _(only in Vim)_
* Opening and closing the editor
  - Open: `vim`
  - Quit: `:q` (closes vim/buffers)
  - Quit all buffers `:qa` (closes all tabs)
* Saving files and dismissing edits
  - Save buffer and quit: `:wq`, `:x` or `ZZ` 
  - Quit without saving: `:q!`
* Modes: Normal/command, Edit/insert, Visual
* Moving around quickly in normal mode (line-based and document)
  - Left: `h`
  - Down: `j`
  - Up: `k`
  - Right: `l`
  - Backward and forward by sentence: `(` and `)`
  - Backward and forward by paragraph: `{` and `}`
  - Go to the matching parenthesis or curly bracket: `%`
* Moving in and out of normal and edit modes
  - From edit mode to normal mode: `<ESC>` (and `Ctrl-[`)
  - After the cursor: `a`
  - At the end of the line: `A`
  - Before the cursor: `i`
  - At the beginning of the line: `I`
  - On a new line after the current line: `o`
  - On a new line before the current line: `O`
* Editing
  - `d` delete the characters from the cursor position up the position given by the next command (for example d$ deletes all character from the current cursor position up to the last column of the line).
  - `c` change the character from the cursor position up to the position indicated by the next command.
  - `x` delete the character under the cursor.
  - `X` delete the character before the cursor (Backspace).
  - `y` copy the characters from the current cursor position up to the position indicated by the next command.
  - `p` paste previous deleted or yanked (copied) text after the current cursor position.
  - `P` paste previous deleted or yanked (copied) text before the current cursor position.
  - `r` replace the current character with the newly typed one.
  - `s` substitute the text from the current cursor position up to the position given by the next command with the newly typed one.
  - `.` repeat the last insertion or editing command (x,d,p…). **Huge** productivity gain in normal mode: `.`
* Undo and redo (normal mode): `u` is undo and `Ctrl-r` is redo (can use repeatedly)

[This](https://blog.interlinked.org/tutorials/vim_tutorial.html) is another pretty good resource that is worth checking out.


### Intermediate

The next step after the basics. The lesser used features?

#### Marks

http://vim.wikia.com/wiki/Using_marks

Basic use

* To mark a location in a document, use `m` followed by a lower case letter (e.g. `ma`) in normal mode.
* To navigate to an `a` mark
  + `'a` will go to the line the mark was made on
  + `` `a`` will go to the exact location the mark was made


### Advanced

Use of plug-ins and using vimscript.

* The [Easy motion](https://github.com/easymotion/vim-easymotion) plug-in
