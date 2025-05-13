# OverTheWire Bandit

This repository contains my notes and solutions for the OverTheWire Bandit wargame. The goal is to practice basic Linux and command line skills by completing levels that each require finding a password to unlock the next.

## How to Use

1. **SSH Login**: Follow the instructions to SSH into the server for each level.
2. **Explore**: Use commands like `ls`, `cat`, `find`, and others to explore the server and locate files.
3. **Find Password**: Each level has a password hidden in a file. Find it and use it to progress to the next level.
4. **Repeat**: Continue the process until you reach the final level.

## Game Levels

- **Level 0**: Start with `ssh bandit0@bandit.labs.overthewire.org -p 2220` and password `bandit0`.
- **Level 1-2**: Use `cat ./-` to find the password.
- **Level 2-3**: Handle spaces in filenames using `cat spaces\ in\ this\ filename`.
- **Level 3-4**: Explore `inhere` and find hidden files with `ls -a`.
- **Level 4-5**: Use the `find` command to locate files of a specific size.
- **Level 5-6**: Use `find` to locate a file with specific properties.
- **Level 6-7**: Use `find` with user and group specifications to locate the next password.

## Useful Commands

- `ls` - List directory contents.
- `cat [filename]` - Display file contents.
- `find [path] [criteria]` - Search for files.
- `cd [directory]` - Change directory.
- `exit` - Exit SSH session.

## Notes

Each level has specific commands to use. Check the notes in each level for the password and steps to move forward.


