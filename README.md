notebook
========

A command-line note-keeping app that uses Git for backups.

**ALL RIGHTS RESERVED**, unless otherwise noted.

<!--
`README.md` readme file.
Copyright 2022 Hal W. Canary III

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
-->

Install:
--------

Instructions (for Unix/Posix/Linux/MacOS systems):

1.  Clone this repository.  Run setup program.

    ```
    git clone git@github.com:HalCanary/notebook.git
    notebook/setup
    ```

2.  Make sure `~/bin` is in your `PATH` environemnt variable.

3.  Make sure that the `VISUAL` environemnt variable is set to the path of your
    favorite text editor.

4.  Make a place to securely push your repository to, then set that as remote

    ```
    cd .../notebook
    git remote add origin YOUR_REPOSITORY_URL
    ```

Make a note:
------------

Just execute the following from the command line:

```
note
```

This will edit a file in the `notebook/YYYY/MM/` directory (creating the
directory if needed) called `notes-YYYY-mm-dd_Www.txt`.  For example:
`notebook/2022/11/notes-2022-11-11_Fri.txt`.

Backup notes to your secure backup:
-----------------------------------

Just execute the following from the command line:

```
notebook-update
```

This will create a commit of any changes to the notebook directory.
