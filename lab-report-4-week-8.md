# CSE 15L Lab Report 4
- [My markdown-parse repository](https://github.com/m6shin/markdown-parse)
- [The markdown-parse repository that I reviewed](https://github.com/ericwpei/markdown-parse.git)
## Snippet 1
- Expected output: `[%60google.com, google.com, ucsd.edu]`
### JUnit Test for Snippet 1
![Image](https://snipboard.io/eGahNm.jpg)
### My Test Output for Snippet 1
![Image](https://i.snipboard.io/DnvkFG.jpg)
-  Here is the part of the JUnit output that shows the test failure.
### Reviewed Repository Test Output for Snippet 1
![Image](https://snipboard.io/7pzq4R.jpg)
- Here is the part of the JUnit output that shows the test failure.
- I think that there will need to be a big code change for the program to account for all related cases that use inline code with backticks. This is because the way my `MarkdownParse.java` file is right now, is not meant to account for links with backticks on them.
## Snippet 2
- Expected output: `[a.com, a.com(()), example.com]`
### JUnit Test for Snippet 2
![Image](https://snipboard.io/TZ8ILg.jpg)
### My Test Output for Snippet 2
![Image](https://i.snipboard.io/AqHDR0.jpg)
- Here is the part of the JUnit output that shows the test failure.
### Reviewed Repository Test Output for Snippet 2
![Image](https://snipboard.io/pmVKZW.jpg)
- Here is the part of the JUnit output that shows the test failure.
-  I think that there will need to be a big code change for the program to account for  nest parentheses, brackets, and escaped brackets. This is because none of the tests that we ran for `MarkdownParse.java` had nest parentheses for instance. To account for all these would take a substantial amount of new code.
## Snippet 3
- Expected output: `[https://ucsd-cse15l-w22.github.io/]`
### JUnit Test for Snippet 3
![Image](https://snipboard.io/9i3KVf.jpg)
### My Test Output for Snippet 3
![Image](https://snipboard.io/nl48LG.jpg)
- Here is the part of the JUnit output that shows the test failure.
### Reviewed Repository Test Output for Snippet 3
![Image](https://snipboard.io/4GpC57.jpg)
- Here is the part of the JUnit output that shows the test failure.
- I think a small line change is good enough to account for newlines in brackets and parentheses. I think an if else statement can deal with these line breaks as I do not think these newlines are as complicated as nest parentheses for instance.