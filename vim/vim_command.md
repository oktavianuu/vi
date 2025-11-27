## Navigating the Modes
- `Esc` -> Normal Mode, for moving, deleting, copying and pasting (this is the default mode)
- `i, a, o, etc.` -> Insert Mode, for typing/inserting text.
- `v, V,, or Ctrl + v` -> Visual Mode, selecting a block of text.

### Normal Mode: Movement (The Vim Language)
Movement commands are the most freq command we'll use. We can think them as verbs that can combined with other actions such as delete, change or copy.
|Command|Action|Description|
|---|---|---|
|`h, j, k, l`|Move|Left, Down, Up, Right (Home Row)|
|`w`|Word|Move to the start of the next word|
|`e`|End|Move to the end of the current word|
|`b`|Back|Move to the start of the previous word|
|`0`|Start|Move to the beginning of the line
|`^`|Start|Move to the first non-blank char of the line|
|`$`|End|Move to the end of the line|
|`gg`|Go to|Go to the very first line of the file|
|`G`|Go to|Go to the very last line of the file|
|`10gg` or `:10`|Go to line 10|Move to a specific line number|

### Normal Mode: Editing and Actions (Verbs)
These "verbs" are often used with a number or a movement command ("noun"). The pattern is:
**[Number]** + **Action** + **[Movement/Object]**
|Command|Verb/Action|Example Combination|Result|
|---|---|---|---|
|`d`|Delete (cut)|`dw`|Delete word|
|`c`|Change (delete and enter insert mode)|`c$`|Change (delete) to end of line, then type|
|`y`|Yank (copy)|`yyp`|Yank (copy) the current line, then paste it below|
|`p`|Put (paste)|`p`|Paste after the cursor|
|`P`|Put (paste)|`P`|Paste before the cursor|
|`x`|Delete|`x`|Delete the char under the cursor|
|`.`|Repeat|`.`|Repeat the last editing command|
|`u`|Undo|`u`|Undo the last change|
|`Ctrl+r`|Redo|`Ctrl+r`|Redo the undone change|

### Insert Mode: Getting In
We use these commands from **Normal Mode** to start typing text.
|command|Action|
|---|---|
|`i`|Insert before the cursor (Standard)|
|`a`|Append after the cursor|
|`o`|Open a new line below and insert|
|`O`|Open a new line above and insert|
|`I`|Insert at the beginning of the line|
|`A`|Append at the end of the line ($)|

### Command-Line Mode: Saving and Exiting
|Command|Action|
|`:w`|Write (save)|
|`:q`|Quit (Exit)|
|`:wq`|Write and Quit (Save and Exit)|
|`:x`|Write and Quit (same as `:wq`)|
|`:q!`|Quit without saving (force quit)|
|`:e filename`|Edit (Open) a new line named filename)\

### Command-Line Mode: Search and Replace 
|Command|Action|
|---|---|
|`/pattern`|Search for pattern forward in the file|
|`?pattern`|Search for pattern backward in the file|
|`n`|Move to the next match|
|`N`|Move to the previous match|
|`:%s/old/new/g`|Subtitute globally: replace all occurences of old with new in the entire file|
|`:%/old/new/gc`|Subtitute globally with confirmation (`c`)|

