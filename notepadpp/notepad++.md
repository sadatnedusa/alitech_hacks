# How can I Bookmark multiples selected lines (to use with F2 after)

- Example of Bookmark into Notepad++
- The Blue Circle showing in below snap is Bookmark

![image](https://github.com/user-attachments/assets/38c248ef-5824-4ba6-b7dd-81ab81c2e501)

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

   - https://community.notepad-plus-plus.org/topic/20458/how-can-i-mark-multiples-selected-lines-to-use-with-f2-after/2

---
# Remove empty lines from Notepad ++

Open Notepad++. 
  - Press Ctrl+H
    - Search Menu -> ![image](https://github.com/user-attachments/assets/4af863c6-5ba8-44f9-8d5c-c77c9e986ce5)

  - Select Regular Expression
    - ![image](https://github.com/user-attachments/assets/4f43cb61-2c48-441f-b25e-fbfdf0c1534c)

  - Enter **^[ \t]*$\r?\n** into Find what:, leave Replace empty.
    - This will match all lines starting with white space and ending with carriage return (in this case a Windows crlf)
    - ![image](https://github.com/user-attachments/assets/4581c842-02b2-47f2-986e-14d7aaf72f54)

    - Click the *Find Next* to confirm only empty lines shown.
    - Accordingly, click on *Replace All* as needed
