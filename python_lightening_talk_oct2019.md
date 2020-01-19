<style>
.container{
    display: flex;
}
.col{
    flex: 1;
}
</style>

# VIM for Python Development
### Lessons from 90 days of usage

#### Bala Juluri

---
## My reasons for trying VIM

- Development on remote Linux machines
- Development on small form Linux systems (Raspberry Pi's)
- Start really quick 

Note:
This will only display in the notes window.
---
# Quick Intro to vim 

- Generic Text Editor widely used.
- Lots of features.
- Can be set as an Python IDE. 
- Heavily relies on key-presses as commands.
- Brutal Learning Curve.


### Not so friendly cheatsheet
<img src = "lib/images/vim_cheat_sheet_for_programmers_screen.png">


## Things are simpler after understanding 

- Modes 
    - Modes allow to split editing tasks
- VIM's Grammer 
    - Grammer allows to compose complex commands from simple commands 


### Modality in VIM
<center>
<img src = "/lib/images/vim-modes_simple.svg.png" height = 400>
</center>

---
## Elements of VIM's Grammer

 
<div class = "container">
<div class="col">
<h3>Motions</h3>

|command| motion |
|---------|--------|
| w | One word|
| j | One line Down |
| $ | End of Line |    
| } | End of Paragraph|    
| ) | End of Sentence|
| ]]| Next class |
| ]m| Next method|

</div>

<div class="col">
<h3>Text Objects</h3>

|command| text object|
|---------|--------|
| p | paragraph|
| " | text in quotes|
| t | text in tags|    
| ( | text in brackets|
| { | text in braces|

</div>

<div class="col">
<h3>Modifiers</h3>
<h4>Act on text objects</h4>

|command| text object|
|---------|--------|
| a | around a text object|
| i | inside a text object|

</div>

<div class="col">
<h3>Operators</h3>
   
|command| Operation|
|---------|--------|
| d | delete |
| p | paste |
| c | change (delete + insert)|    
| y | yank/copy|    


</div>

</div>
---

### VIM's Grammar Rules

<pre class = "fragment">
RULE 1 : Repeat Motions     {Count}{Motion}
          
            command:             3        w 
                          move   3      words 
</pre>

<pre class = "fragment">
RULE 2: Operator with a Motion {Operator} {Motion} 

            command:                 d        3w
                            delete      while moving 3 words
</pre>

<pre class ="fragment">
RULE 3: Operate on text object:   {Operator} {Modifier} {Text object} 

 command:                          y          i             "
                                  yank/copy inside       quoted strings
</pre>                           

---
### Pros
- Grammar enables fast navigation and editing. 
- Fast startup time. Low RAM usage. Preinstalled on many linux systems.
- Plethora of Plugins (Code completion, Highlightening, Linting, Refactoring etc ...)
- No Crashes 
- Customization to extreme.
- Good documentation.
- Free

---
### Cons
- Initial frustration with changing modes
- Initial big dip in productivity
- Extremely steep learning curve 
    - registers, buffers, quickfix, location lists, 
     macros, marks, tabs, windows, sessions, key mappings
     and many more concepts
- Setting up an IDE environment takes time and could be frustrating especially on Windows

---
### Carrying vim with me to other tools 
- Jupyter notebooks: jpyter-vim-binding
- Bash/zsh shell: set -o vi in ~/.bashrc or ~/.zshrc
- Chrome/firefox : cvim
- Pycharm : idea vim plugin


--- 
### Some TIPS that I found useful:

- Install Neovim rather than vim for easier python integration. 
    - my notes are here: 
- VIMTUTOR
- Start with some popular vimrc files and go from there.
    - I used fisa.vim
- Watch Leeren's video on youtube
    - Navigating Python Code with fuzzy find file browsing
    - splitting windows
    - saving sessions

---
# THANK YOU!
## HAPPY HOLIDAYS!
