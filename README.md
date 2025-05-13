# OverTheWire-Bandit
walkthrough notes 

LEVEL 0 
connect to SSH: "ssh bandit0@bandit.labs.overthewire.org -p 2220"
password: bandit0 

LEVEL 0-1 
ls -> found file "readme" 
cat readme 
password found: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
exit 
login at "ssh bandit1@bandit.labs.overthewire.org -p 2220"
use password above 
**Repeat the process of exiting and logging in via SSH to progress to the next level, using the appropriate level numbers.**

LEVEL 1-2 
ls 
"-" file found
cat ./- 
password: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx
* ./ means current directory, telling system look here for this folder "-"

LEVEL 2-3 
ls 
file found: "spaces in this filename" 
cat spaces(I used tab) which autocompleted command to "cat spaces/ in/ this/ filename" 
password: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
* Spaces in filenames: To handle spaces in filenames, use backslashes (\) to escape each space, or use quotes (" ").

LEVEL 3-4 
ls 
cd inhere
ls -a 
cat ...Hiding-From-You
password: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ

LEVEL 4-5
ls 
cd inhere
cat ./-file07 (password found) **use up/down arrow keys to not retype command a million times** 
password =: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw 

LEVEL 5-6
ls 
cd inhere
uff, need a more effective way to search 
cd .. 
"find inhere/ -type f -size 1033c ! -executable" -> **inhere/maybehere07/.file2**
follow this path and open file 
password: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
*Find quick-sheet 
  find [where_to_search] [criteria] [actions]
  Most useful flags:
          type f → Only look for files (not folders)
          name "pattern" → Match file names (wildcards like *.txt work)
          size 1033c → Exact size in bytes (c = bytes, k = kilobytes, M = megabytes)
          readable → File is readable
          ! -executable → File is not executable (! = NOT)
          exec COMMAND {} \; → Run a command (like cat) on the result

LEVEL 6-7 


