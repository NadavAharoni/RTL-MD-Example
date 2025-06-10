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

# דוגמא לרשימות
1. אחד
2. שתיים
3. שלש



# דוגמא ל-span

When writing "C++", the + characters do not have a strong direction, so they are rendered according to the enclosing paragraph, which is right-to-left, so the result looks wrong:

גם C++ היא שפה מונחית עצמים

One way to fix it is to add `&lrm;` after the ++.
The raw text will be:

```
גם C++&lrm; היא שפה מונחית עצמים
```

It will ne rendered as follows (which is what we wanted):

גם C++&lrm; היא שפה מונחית עצמים

&rlm;C++&lrm; ו-Java הן שפות מונחית עצמים


