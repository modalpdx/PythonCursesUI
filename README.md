# PythonCursesUI

The curses UI portion of a capstone project from OSU CS419, Winter 2016.
The bits that sent emails with appointment deletion attachments were
removed because I did not write them. This repo only contains my
Python-curses UI for the project.

To run this, download all of the files into a directory and run the setup
script to get a sample database:

```
python setupdb.py
```

This will create an appt.db file in the directory containing sample
entries for Feb. 28, 2016 - April 2, 2016. Those dates have obviously
passed, so you will need to navigate to one of those dates to see the
entries. All days without database entries will show "No appointments..."

##Keys:

General navigation (yes, basic Vi key navigation works):

- Arrow-up or k moves up 
- Arrow-down or j moves down
- Arrow-left or h moves left
- Arrow-right or l moves right
- D selects the highlighted appointment for deletion
- Q quits the UI

Calendar/date-picker:

- C pulls up the calendar/date-picker
- Arrow-up or k moves backward through months
- Arrow-down or j moves forward through months
- Arrow-left or h moves backward through days
- Arrow-right or l moves forward through days
- T shoots you to today's date
- ENTER chooses the date
- Q quits the calendar/date-picker

Deletion popup:

- Y confirms deletion
- Q quits the deletion popup


##Disclaimer:

As with all school code, this is presented as-is. There are undoubtedly
bugs (I can name a few). I will be the first to admit that this code is
not DRY and it is due for a major refactoring. Still, I wanted to post
this to make it available for review. Future revisions will clean things
up nicely.

If you're in school now and you're looking for a shortcut, please feel
free to read my code for ideas but do not copy it into your own source
tree as-is, and definitely do not take credit for it. Don't be naughty...

Version 1.0: Initial checkin
