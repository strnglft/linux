# OverTheWire: Bandit

## level 0 -> 1
**goal:** find the password stored in a file called 'readme' in the home directory
**command used:** 'ls' to list files, 'cat readme' to read the file
**what I learned:** 'cat' is more appropriate than 'nano' for reading files without editting them

## level 1 -> 2
**goal:** find the password stored in a file called '-' in the home directory
**command used:** 'ls' to list files, 'cat ./-' to read the contents of the file
**what I learned:** 'cat -' supplies a flag instead of denoting a direct file path to interact with

## level 2 -> 3 
**goal:** find the password stored in a file called '--spaces in this filename--'
**command used:** 'ls' to list files, 'cat ./"--spaces in this filename--" to read contents
**what I learned:** using "" will target literal text in strings


## level 3 -> 4
**goal:** find the password stored in a hidden file called "...Hiding-From-You"
**command used:** 'cd inhere' to change directories, 'ls -a' to list hidden items, 'cat ./"...Hiding-From-You"' to read contents
**what I learned:** '-a' flag for 'ls' shows all hidden contents.
