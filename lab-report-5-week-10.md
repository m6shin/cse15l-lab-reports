# CSE 15L Lab Report 5
## How I found the tests with different results
- I ran the script.sh in the given folder and copied and pasted the result into a result.txt file.
- I ran `script.sh` on my implementation of markdown-parse and copied and pasted the result onto another result.txt file.
- Next, to find the differences, I ran `diff <Path of first result.txt> <Path of second result.txt>` in the terminal.
## Test 1
![Image](https://snipboard.io/jlFfGW.jpg)
- The primary output was from my markdown-parse, and the latter output was from the given markdown-parse. The difference came from the file 497.md. Both of the implementations are wrong since the output from my implementation had had missing `closeParen` and the given implementation had an empty output. Lastly, it seems that the correct output is `[foo\(and\(bar\))]` since it is in the correct link format and it has `closeParen`. 
### Bug
![Image](https://snipboard.io/bRxVAt.jpg)
- The bug likely is when that when there is an extra `closeParen`, it only takes into account the link that comes before the first `closeParen` and not the link before the last `closeParen`. I think that in order to fix this bug, I need to change the `findCloseParen` method to `findLastCloseParen` in line 35. I think adding a method `findLastCloseParen` may also be helpful as well.
## Test 2
![Image](https://snipboard.io/xEf5dq.jpg)
- The primary output was from my markdown-parse, and the latter output was from the given markdown-parse. The difference came from the file 32.md. The given implementation of MarkdownParse.java is right because the output is empty. This is true because if a link contains a space, the space should not be added to the ArrayList, and thus, an empty ArrayList is returned.
### Bug
![Image](https://snipboard.io/bRxVAt.jpg)
- The bug in my code is that my implementation of MarkdownParse.java is not able to detect spaces in a link and will add the string as a result. I think that in order to fix this bug, it is best that an if statement in line 36 needs to be added to check if there is a space in the link using the indexOf method.