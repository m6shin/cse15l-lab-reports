# CSE 15L Lab Report 3
## Streamlining ssh Configuration
## `.ssh/config` File
![Image](https://snipboard.io/kTfPjN.jpg)
- I edited my `.ssh/config` file using VSCode.
- I added the bottom block of text with `Host ieng6` as the header. Because of this, now I can log into my account with just `ssh ieng6`
## New `ssh` Login Alias
![Image](https://snipboard.io/mroSdO.jpg)
- My new alias is `ieng6`.
- Because my new alias is `ieng6` I do not have to remember my full account name and that I can use `ssh ieng6` to log into my CSE 15L account. 
## `scp` Command
![Image](https://snipboard.io/EiDfUy.jpg)
- I used the `scp` command to copy the file WhereAmI.java onto my account.
- When using `scp`, I used `scp WhereAmI.java ieng6:~/`. 
- Prior to this, I would have had to use `scp WhereAmI.java cs15lwi22adu@ieng6.ucsd.edu:~/` in order to copy a file onto my account.