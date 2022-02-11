# CSE 15L Lab Report 2
## 1. Code Change 1
- Screenshot of code change difference:
-![Image](https://snipboard.io/IZRnA1.jpg)
- Link for [test file](https://github.com/m6shin/markdown-parse/blob/main/newer-test-file3.md)
- Symptom
- ![Image](https://snipboard.io/TCKOiF.jpg)
- Prior to fixing this bug, the failure-inducing input `newer-test-file3.md`  was causing the symptom of an infinite while loop. There was text after the links, which caused the program to continue running the while loop continuously forever. After the code change, the file printed out the correct link.
## 2. Code Change 2
- Screenshot of code change difference:
-![Image](https://snipboard.io/ymbvoQ.jpg)
- Link for [test file](https://github.com/m6shin/markdown-parse/blob/main/newer-test-file1.md)
- Symptom
![Image](https://snipboard.io/WBKftJ.jpg)
- Prior to fixing this bug, the failure-inducing input `newer-test-file1.md` was causing the symptom of that it was not adding images to the list of links. The output initially said that it needed to have a `public static void main` method or the class needed to extend `javafx.application.Application`. After the code change, it showed each current index value before and after and also printed out the correct link.
## 3. Code Change 3
- Screenshot of code change difference:
- ![Image](https://snipboard.io/L5FcU2.jpg)
- Link for [test file](https://github.com/m6shin/markdown-parse/blob/main/newer-test-file2.md)
- Symptom
![Image](https://snipboard.io/KDrtEP.jpg)
-  Prior to fixing this bug, the failure-inducing input `newer-test-file2.md` was an `StringIndexOutOfBoundsException`. The error may have came from the assumption that the file would end with a link as `currentIndex = closeParen + 1`. However, if there’s text after the last link, `currentIndex` won’t ever be greater than `markdown.length()`, so it won’t exit the while loop. These changes that we made (adding if else statements and deleting `toReturn`) helped resolve the symptom and printed the correct link.