---
layout: post
title: Vim Config
date: 06-01-2025
categories:
  - tools
tags:
  - tools
  - vim
---
# MY VIM CONFIG...

```text
├── init.lua
├── kitty.sh
├── lazy-lock.json
├── lazyvim.json
├── LICENSE
├── lua
│   ├── config
│   │   ├── autocmds.lua
│   │   ├── keymaps.lua
│   │   ├── lazy.lua
│   │   └── options.lua
│   └── plugins
│       ├── copilot.lua
│       ├── dashboard.lua
│       ├── disable.lua
│       └── example.lua
├── README.md
└── stylua.toml
```
## Basic Movement
* j: Move cursor down.
* k: Move cursor up.
* l: Move cursor right.

## Modes
* `Esc`: and `jj` Normal Mode
* i: Insert text before the cursor
* I: Insert text at the beginning of the line
* a: Append text after the cursor
* A: Appenjd text at the end of the line
* v: Visual Mode (character-wise)
* V: Visual Mode (line-wise)
* Ctrl+v: Visual Mode (block-wise)
* :: Command-line Mode
* r: Replace a single character
* R: Replace mode (continuous replace)

## Word Movements
* w: Move to the start of the next word.
* W : Move to the start of the previous word.
* b: Move to the start of the current/previous word.

## Line Movements
* 0: Move to the start of the line.
* ^: Move to the first non-blank character.
* $: Move to the end of the line.
* %: Jump to the matching brace or bracket.
##  Screen Movements
* H: Move to the top of the screen.
* M: Move to the middle of the screen.
* L: Move to the bottom of the screen.
* zz: Center the current line. I use it very often
* zt: Move the current line to the top. (Also this one)

##  Paragraph and Block Movements
* {: Start of the current paragraph/block. 
* }: End of the current paragraph/block.

## File Movements
* gg: Start of the file.
* G: End of the file.
* :\line_number\: Go to a specific line.

## Jump Movements
* gd: Go to definition.
* ctrl-o: Previous location.
* ctrl-i: Next location.
* 'm: Jump to mark 'm' (set with mm). I don’t use it too much
* [g, ]g: Navigate diagnostics. Quite helpful, I use it all the time
* F2_key: Rename occurrences. 

## Scrolling
* ctrl-u: Scroll up (half-screen).
* ctrl-d: Scroll down (half-screen). somehow this doesn’t work
* ctrl-b: Scroll up (full screen).
* ctrl-f: Scroll down (full screen).

## Search
* /word: Search for a 'word'.
* ge: Replace word under cursor. This is command that I created

## Editing
* diw: Delete current word.
* yiw: Copy the current word.

## cpy_paste
* u : undo
* p: paste copied by yiw (pastes after the cursor)
* shift+p: paste before the cursor

## Fold
* zf: Fold at current indent level.
* za: Toggle current fold.

 ## NerdTree
* CTRL+e: Toggle neo-tree.

## Window Resizing
* ++: Increase window width.
* —: Decrease window width.

## Window Creation
:new: Create new buffer horizontally
:vnew: Create new buffer vertically

## Window Switch
CTRL+w+ (One of the h-j-k-l): Switch the cursor between buffers

## Buffers
* gb: List buffers.
* bd: Delete current buffer.
* bd!: Delete current buffer without saving changes.
* b buffer_number: Go to a specific buffer.

## Session Commands
* mks!: Create a session.
* vim  -S: Load a session.

## File Operations
* :w: Save file.
* :q: Quit without saving.
* :q!: Force quit without saving.
* :wq: Save and quit.Y
