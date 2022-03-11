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
- The bug likely is when that when there is an extra `closeParen`, it only takes into account the link that comes before the first `closeParen` and not the link before the last `closeParen`. I think in order to fix this bug, I need to change the `findCloseParen` method to `findLastCloseParen` in line 35. I think adding a method `findLastCloseParen` may also be helpful as well.
## Test 2
![Image](https://snipboard.io/CS34g2.jpg)
### Bug
![Image](https://snipboard.io/bRxVAt.jpg)