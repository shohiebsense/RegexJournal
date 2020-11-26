# RegexJournal
Learn Regex

## Format  
``/[regex_expressions]/[flags] ``

## Flags
1. Global. Search all, not search only for first  
``g``  
2. Case Insensitive  
``i``  
3. Multiline  
``m``  
4. Singleline  
``s``  
5. Unicode  
``u``
6. Sticky  
``y``  

## Regex Expressions
1. \+  
Quantifier. One or more preceeding token. Example:
``/e+/g``  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/1..png?raw=true)  
``e or more than 1 e``  

2. \?
Optional. Matches 0 or 1 of the preceding token, effectively making it optional.
``/ea?/g``  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/3.png?raw=true)  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/2.png?raw=true)  

3. \*  
Combination of \+ and \?. Matches 0 or more of the preceding token.  
``/re*/g  ``  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/4.png?raw=true)  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/5.png?raw=true)  


4. \.  
Matches any character except linebreaks.  
``/.at/g  ``  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/6.png?raw=true)  

5. \w  or [A-Za-z0-9_]  
Matches any word character (alphanumeric & underscore). Only matches low-ascii characters (no accented or non-roman characters).  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/7.png?raw=true)  

6. \s  
Whitespace. Matches any whitespace character (spaces, tabs, line breaks).  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/8.png?raw=true)  

7. \S
Not Whitespace. Matches any character that is not a whitespace character (spaces, tabs, line breaks).  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/9.png?raw=true)  

8. \W  or [^A-Za-z0-9_]  
Not Word.  Matches any character that is not a word character (alphanumeric & underscore).  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/10.png?raw=true)  

9. \w{4,}
Word + Quantifier. {4,} Match 4 or more of the preceeding token.  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/11.png?raw=true)  

10. \w{4,5}
Word + Quantifier. {4,} Match 4 and 5 of the preceeding token.  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/12.png?raw=true)  

11. [a-zA-Z]  
Character Set. Matches a character in the range "a" to "z" case sensitive. "A" to "Z" case sensitive.  
``/[a-zA-Z]at/g  ``  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/13.png?raw=true)  

12. (t|T)  
Or.  
``/(t|T)he/g``  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/14.png?raw=true)  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/15.png?raw=true)  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/16.png?raw=true)  

13. ^  
Beginning. 
``^[TtIc]``  
``/^[TtIc]/gm``  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/17.png?raw=true)  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/18.png?raw=true) 

14. $  
End.  
``\.$/g``  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/19.png?raw=true) 

15. ?<=  
Positive Lookbehind. Matches a group before the main expression without including it in the result.  
``(?<=[tT]he).{1,}/g``  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/20.png?raw=true)  

16. \d
Digits.  
``/^(0[8]|62)[0-9]{8,10}$/gm  ``  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/21.png?raw=true)  
``/^(08|62)\d{8,11}$/gm ``  
![example](https://github.com/shohiebsense/RegexJournal/blob/main/22.png?raw=true)  

### Source
https://www.youtube.com/watch?v=rhzKDrUiJVk
