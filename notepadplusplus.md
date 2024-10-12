# How can I mark multiples selected lines (to use with F2 after)
---

Select all N lines with shift-and-arrows or dragging the mouse
Ctrl+M (or Search > Mark) to bring up the Mark dialog
Fill out the Mark dialog:
Find what: \R
enable ☑ Bookmark line (this turns on bookmarking)
enable ☑ In Selection (the block should still be selected from step 1)
set Search Mode to ☑ Regular expression
click Mark All
At this point, F2 (Next bookmark) should take you to the next bookmarked line

If the last line of your selection happened to be the last line in the file, with no EOL sequence, that expression might miss the last line. You can either then manually bookmark that line (Ctrl+F2 or click in the bookmark column of the GUI), or you could change the expression to something like \R|^.*\Z …


https://community.notepad-plus-plus.org/topic/20458/how-can-i-mark-multiples-selected-lines-to-use-with-f2-after/2
