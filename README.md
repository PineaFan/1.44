# 1.44
### A Floppy Disk Enforcer

## Features
*When -D is passed for Destructive mode:*
- Truncate any filenames over 8 characters
- Truncate any file extensions over 3 characters
- Remove all invalid characters from filenames
- Corrupts any file if it's called "CON", "LPT1", etc. and deletes it
- Turns all filenames into lowercase
- Corrupts any file if it brings the total size of the disk over 1.44MB
- **The order of corruption is random**

*In normal and destructive modes:*
- Warn for invalid filenames
- Warn for invalid file extensions
- Warn if invalid characters are present in filenames
- Stops if the total file size exceeds 1.44MB

*Then*
- Find any file called autorun.*
- Finds its #! and checks the command
- Executes the command with the file as an argument
