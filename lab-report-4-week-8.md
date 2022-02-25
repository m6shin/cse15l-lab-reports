# CSE 15L Lab Report 4
- [My markdown-parse repository](https://github.com/m6shin/markdown-parse)
- [The markdown-parse repository that I reviewed](https://github.com/ericwpei/markdown-parse.git)
## Snippet 1
### Markdown:
```
`[a link`](url.com)

[another link](`google.com)`

[`cod[e`](google.com)

[`code]`](ucsd.edu)
```
- Expected output: `[%60google.com, google.com, ucsd.edu]`
### JUnit Test for Snippet 1
![Image](https://snipboard.io/eGahNm.jpg)
### My Test Output for Snippet 1
![Image](https://i.snipboard.io/DnvkFG.jpg)
-  Here is the part of the JUnit output that shows the test failure.
### Reviewed Repository Test Output for Snippet 1
![Image](https://snipboard.io/7pzq4R.jpg)
- Here is the part of the JUnit output that shows the test failure.
## Snippet 2
### Markdown:
```
[a [nested link](a.com)](b.com)

[a nested parenthesized url](a.com(()))

[some escaped \[ brackets \]](example.com)
```
- Expected output: `[a.com, a.com(()), example.com]`
### JUnit Test for Snippet 2
![Image](https://snipboard.io/TZ8ILg.jpg)
### My Test Output for Snippet 2
![Image](https://i.snipboard.io/AqHDR0.jpg)
- Here is the part of the JUnit output that shows the test failure.
### Reviewed Repository Test Output for Snippet 2
![Image](https://snipboard.io/pmVKZW.jpg)
- Here is the part of the JUnit output that shows the test failure.
## Snippet 3
### Markdown:
```
this title text is really long and takes up more than 
one line

and has some line breaks](
    https://www.twitter.com
)

[this title text is really long and takes up more than 
one line](
    https://ucsd-cse15l-w22.github.io/
)


[this link doesn't have a closing parenthesis](github.com

And there's still some more text after that.

[this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/



)

And then there's more text
```
- Expected output: `[https://ucsd-cse15l-w22.github.io/]`
### JUnit Test for Snippet 3
![Image](https://snipboard.io/9i3KVf.jpg)
### My Test Output for Snippet 3
![Image](https://snipboard.io/nl48LG.jpg)
- Here is the part of the JUnit output that shows the test failure.
### Reviewed Repository Test Output for Snippet 3
![Image](https://snipboard.io/4GpC57.jpg)
- Here is the part of the JUnit output that shows the test failure.