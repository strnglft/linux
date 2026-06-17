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

## level 4 -> 5
**goal:** find the password in the only human-readable file in the inhere directory
**command used:** 'cd inhere' to change directories, 'file ./-file0*' to list file types using '*' as wildcard. 'cat ./-file07' to read contents
**what I learned:** rather than relying on file extensions, linux CLI will list the constitutive components of a file 

## level 5 -> level 6
**goal:** locating password somewhere in 'inhere' directory in a file that is human-readable, 1033 bytes in size, and not executable
**command used:** 'ls' to list storage, 'cd inhere' to change directories, 'ls' to list storage. 'find -size 1033c' to locate file, 'cat ./maybehere07/.file 2' to extract password
**what I learned:** 'find' has various flags that can be used to isolate individual file characteristics
