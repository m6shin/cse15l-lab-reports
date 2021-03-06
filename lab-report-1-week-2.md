# CSE 15L Lab Report 1
## 1. Installing VScode
![Image](https://i.snipboard.io/ksPA7d.jpg)
- Before Lab 1, I already had VScode downloaded from when I took CSE 11 last fall.
- To download VScode on the computer, one goes to this [link](https://code.visualstudio.com/) and downloads it from there.
## 2. Remotely Connecting
![Image](https://snipboard.io/X4wZa7.jpg)
- In order for me to log onto my account, I needed to find my CSE 15L account using this [link](https://sdacs.ucsd.edu/~icc/index.php) and change the password.
- It also took me awhile to figure out that when typing out my password on the terminal, it will not show for security. I initially thought that there was something wrong with my account when I typed it into the terminal.
## 3. Trying Some Commands
![Image](https://snipboard.io/ySOv0R.jpg)
- The main commands that I tried were `cd ~`, `cd`, `ls -lat`, and `ls -a`.
- What I learned was that `cd ~` does not do anything while in home directory and ls makes a long list.
- Additionally, I tried finding the directory but an error popped up and said that something was wrong with my syntax.
## 4. Moving Files with scp
![Image](https://snipboard.io/XdjNc4.jpg)
- In order to use `scp`, I first copied the code from WhereAmI.java and then I had to login again using the command `scp`.
- When i changed the code in WhereAmI.java and copied it into the remote server, it took me about 1.2 seconds for the code to run.
## 5. SSH Keys
![Image](https://snipboard.io/2h7pG5.jpg)
- In order for me to set up ssh, I needed to use the command `ssh-keygen` and then save it on the computer.

![Image](https://snipboard.io/Svmanw.jpg)
- Since I use Windows to set up ssh, I needed to follow directions on this [link](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_keymanagement#user-key-generation) and open my Powershell as the administrator to set up the ssh-agent. After setting up `ssh`, I am able to log into my CSE 15L account without my password.
## 6. Optimizing Remote Running
![Image](https://snipboard.io/gXTyYu.jpg)
- I found out that the command `ssh (account name) ls` will list the home directory on the remote server.
- Also, semicolons can help a person run multiple lines. For instance, I used the command `cp WhereAmI.java OtherMain.java; javac OtherMain.java; java WhereAmI` to perform multiple java and javac commands.
- Logging in, changing the code, and running the file took me about 2 minutes with 8 keystrokes from pressing the up arrow four times for past commands, copying and pasting another command once, using a semicolon, and pressing enter once to run the code.