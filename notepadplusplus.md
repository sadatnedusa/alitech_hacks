# How can I mark multiples selected lines (to use with F2 after)
---

1. Select all N lines with shift-and-arrows or dragging the mouse.
2. Press `Ctrl+M` (or go to **Search** > **Mark**) to bring up the Mark dialog.
3. Fill out the Mark dialog:
   - **Find what**: `\R`
   - Enable ☑ **Bookmark line** (this turns on bookmarking).
   - Enable ☑ **In Selection** (the block should still be selected from step 1).
   - Set **Search Mode** to ☑ **Regular expression**.
   - Click **Mark All**.

4. At this point, `F2` (Next bookmark) should take you to the next bookmarked line.

5. If the last line of your selection happens to be the last line in the file, with no EOL sequence, that expression might miss the last line. You can either manually bookmark that line (`Ctrl+F2` or click in the bookmark column of the GUI), or you could change the expression to something like `\R|^.*\Z`.


https://community.notepad-plus-plus.org/topic/20458/how-can-i-mark-multiples-selected-lines-to-use-with-f2-after/2
