## Navigation
- `j` -> scroll down
- `k` -> scroll up
- `gg` -> go to first page
- `G` -> go to last page
- `nG` -> go to n page (e.g., 50g goes to page 50)
- commands: we can enter `:` just like in vim and `LaTeX`  where we can type command like `:bmark` for bookmarking and `offset <number>` to set a page number.
- `J` or `Space` -> next page
- `K` or `shift + space` -> previous page
- `/` -> Open the search bar at the bottom
- `n` -> next result
- `N` -> previous result
- `f` -> follow links, highlights all links with a number, then press the number to follow the link.
- `:` enter command like `:bmark`, `:blist`, `:quit`

## pdf with zathura
- `Tab` -> Toggle the table of content
- `j` & `k` -> move the cursor down (j) or up (k) through TOC
- `l` & `right arrow` -> expand sections
- `h` & `left arrow` -> collapse entry to hide sub-sections
- `space` / `enter` -> jump to section
- `Tab` -> second tab will return to normal mode
- `L` -> expand all
- `H` -> collapse all sections

## window and zooming setting
- `s` -> adjust window width
- `a` -> adjust window best-fit
- `=` -> zoom actual size
- `+` -> zoom in
- `-` -> soom out
**Setting specific zoom level**
- press `:` and type `zoom <percentage>` and enter, example `:zoom 150`

## Document Navigation and Information
**These commands help you quickly jump within a document or see important metadata.**
- `open` -> `:open ~/Documents/report.pdf`, opens a new doc in the current window.
`goto` -> `goto 42`, jump to page 42


## Bookmarks and History
**Quickmarks**
- `m<char>` -> set quickmark, Press `m` then any letter or number (a-z or 0-9)will saves current page and position to that key.
- `'<char>` -> go to quickmark, Press `'` (single quote) then the corresponding letter or number to instantly jump back to that spot.
- (backtick) -> go to last spot , jumps us between the last two positions we're viewing 
**Example usage**
1. We're on a page discussing Python classes, we press `m` then `p` (`m p`).
2. We jump ahead to a chapter on data science, then we press `<backtick> p` to instantly return to the python classes page.

**Named Bookmarks** 
- `:bmark <name>` -> save bookmark, saves the current page with a custom, memorable name.
- `:blist` -> list bookmarks, shows all saved bookmarks for current documen. We can select one to jump to it.
- `:bdelete <name>` -> Delete Bookmark, Deletes a previously saved bookmark.
**Usage example**:
1. We are on a complex diagram in our programming book. We press `:` and type `:bmark chapter_5_diagram` then press enter.
2. The next day, we open the same pdf, press `:` and type `blist`, we see our named bookmark and jumpt stright to it.

## Jump List and History 
Jump list tracks our movement within a doc, while the history tracks the doc we've opened.
**Jump List (Movement History within a document)**
This works like the forward/back buttons in a web browser. Every time we jump to a new location (e.g., following a link, using a bookmark, or jumping to a page number), zathura records it.
- Ctrl + o -> Jump Back, moves us back to the previous position in the jump list.
- Ctrl + i, -> Jump Forward, moves us forward to the next position in the jump list.
**Document History**
- `:history` -> show history, display a list of recently opened file. We can select one to open it immediately.
## printing and exiting
- `q` -> closes the current doc window
- `Q` -> Closes the current doc without prompting for unsaved changes.

