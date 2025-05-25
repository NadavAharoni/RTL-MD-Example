# RTL-MD-Example
A small repo to demonstrate right-to-left languages MarkDown

The following section header is in Hebrew, it says: this is an example of Hebrew in a Markdown document.  
Since the first character is in Hebrew, the whole paragraph is right-to-left.

Hebrew and English can appear in the same paragraph, and consecutive words in English will be rendered correctly left-to-right.


# דוגמא לעברית במסמך Markdown

טקסט רגיל

עברית ו-English יכולות להופיע באותה פסקה. גם מספר מילים באנגלית יופיעו בסדר הנכון word1 word2 word3.

# Overriding Paragraph Direction

If a paragprah starts with an English (or any other left-to-right language) the paragraph will be left-to-right.  The direction can be overriden using div.
The following:

```
<p dir="rtl">
Java היא שפה מונחית עצמים
</p>
```

Results in a right-to-left paragraph, despite starting with "J".

<p dir="rtl">
Java היא שפה מונחית עצמים
</p>

The paragprah translates to "Java is an object oriented language".







גם C++ היא שפה מונחית עצמים
