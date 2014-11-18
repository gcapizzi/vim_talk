```c

     ________ ++     ________
    /VVVVVVVV\++++  /VVVVVVVV\
    \VVVVVVVV/++++++\VVVVVVVV/
     |VVVVVV|++++++++/VVVVV/'
     |VVVVVV|++++++/VVVVV/'
    +|VVVVVV|++++/VVVVV/'+
  +++|VVVVVV|++/VVVVV/'+++++
+++++|VVVVVV|/VVV___++++++++++
  +++|VVVVVVVVVV/##/ +_+_+_+_
    +|VVVVVVVVV___ +/#_#,#_#,\
     |VVVVVVV//##/+/#/+/#/'/#/
     |VVVVV/'+/#/+/#/+/#/ /#/
     |VVV/'++/#/+/#/ /#/ /#/
     'V/'  /##//##//##//###/
              ++
```

        a step by step introduction


# STEP 1

BASIC USAGE / INSERT MODE

- move with h, j, k, l (or arrow keys :)
- enter the INSERT mode with i, a
- go back to normal mode with <Esc>
- delete lines with dd
- copy lines with yy
- paste with p
- open a file with :e (:tabe to open in a new tab)
- save with :w
- quit with :q
- add ! to ignore unsaved changes


# STEP 2

VISUAL MODE

- enter the VISUAL mode with v
- make any movement to select text
- go back to normal mode with <Esc>
- delete with d
- copy with y (paste with p)
- change (delete and go to INSERT) with c
- indent with <, >
- try also VISUAL LINE mode (V) and VISUAL BLOCK mode (Ctrl-v)


# STEP 3

MORE MOTIONS!

- words: w, W, e, E, ge, gE, b, B
- sentences: (, )
- paragraphs: {, }
- to specific char: f, t
- start/end of file: gg, G
- specific line: [count]G
- start/end of line: ^, $, 0
- matching delimiter: %
- search: /, ?, n, N, *, #

(See `:help Q_lr`)


# STEP 4

OPERATORS + MOTIONS = AWESOME

- operators and motions are orthogonal
- you can combine them in every possible way
- once you learn a new operator/motion, you can combine it with the ones you
  already know immediately

Some examples:

- dw deletes from the cursor to the beginning of the next word
- y} copies from the cursor to the end of the current paragraph
- ct) changes from the cursor to the first closing paren


# STEP 5

TEXT OBJECTS (i/a)

- word: w
- sentence: s
- paragraph: p
- method: m
- inner words: v (with plugin)
- XML/HTML tag: t
- delimited text: '', "", (), [], {}, <>

(See `:help text-objects`)


# STEP 6

OTHER TRICKS

- .
- insert at the beginning/end of line with I, A
- start inserting on a new line below/above: o, O
- change/delete till the end of line with C, D
- delete the char under the cursor with x, X
- replace the char under the cursor with r
- join the current line and the next with J
- undo/redo with u, Ctrl-r
- complete words with Ctrl-n, Ctrl-p


# STEP 7

EX COMMANDS

`:[range]{command}`

- find and replace with :s
- filter by a shell command with :!
- :g, :v
- :y, :d, :m, :<, :>

(See `:help ex-cmd-index`)


# RESOURCES

- `vimtutor`
- [vimcasts.org](http://vimcasts.org)
- [github.com/tpope](http://github.com/tpope)
- [github.com/gcapizzi/vimpeppers](http://github.com/gcapizzi/vimpeppers)
- [Graphical vi-vim Cheat Sheet and Tutorial](http://www.viemu.com/a_vi_vim_graphical_cheat_sheet_tutorial.html)
- [Seven habits of effective text editing](http://www.moolenaar.net/habits.html)
- [operator, the true power of Vim](http://whileimautomaton.net/2008/11/vimm3/operator)
- [Your problem with Vim is that you don't grok vi.](http://stackoverflow.com/questions/1218390/what-is-your-most-productive-shortcut-with-vim/1220118#1220118)
- [A Vim Tutorial and Primer](http://danielmiessler.com/study/vim)
- [Coming Home to Vim](http://stevelosh.com/blog/2010/09/coming-home-to-vim)
- [Vim: revisited](http://mislav.uniqpath.com/2011/12/vim-revisited)
