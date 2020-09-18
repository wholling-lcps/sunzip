# Schoology Unzip Utility
A Python script that extracts all Java sources and Zip archives from the latest
revision submitted by each student in the bulk download of student submissions
offered by Schoology for each assignment.

You can specify extra files to copy into each student's revision in the
destination path (default is the current directory), which can be useful for
test files or jKarel maps.

## Usage
**Command Line Interface**

```
usage: sunzip [-h] [-d DESTINATION] [-e [EXTRA_FILES [EXTRA_FILES ...]]] [-g] [zipfile]

A script for extracting and organizing code submissions in Schoology

positional arguments:
  zipfile               The name of the archive that contains the revisions of
                        all student submissions

optional arguments:
  -h, --help            show this help message and exit
  -d DESTINATION, --destination DESTINATION
                        where to put the extracted revisions
  -e [EXTRA_FILE [EXTRA_FILE ...]], --extra-file [EXTRA_FILE [EXTRA_FILE ...]]
                        Additional files to be copied (e.g., test files, jKarel maps)
  -g, --gui             Use a graphical interface
```

**GUI**

On Windows, you can also run the included batch script to launch the GUI.  It
assumes that it shares a directory with the Python script and that Python was
added to your %PATH% during installation.

A message box will appear when the extraction is complete.

## Limitations
Currently, the script uses a built-in set of dialogs for browsing files and
folders in the GUI.  These
