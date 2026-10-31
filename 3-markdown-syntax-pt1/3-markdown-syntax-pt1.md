# Markdown Syntax: Part 1

## What is Markdown?

Markdown is the plain-text markup language Obsidian uses for its notes. Its extension is `.md`. It is similar to `.txt` but fancier.

Since it uses `.md` files for its notes and they can be opened by any editor, Obsidian is not a must for our notes.

## 3.1 - Headings

Headings help organize a note into sections. To create a heading, ==🟢add a space after one or more # symbols==. The number of # symbols determines the heading level, from 1 to 6.

```markdown
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
```

==Use Heading 1 for the note title, Heading 2 for main sections, and Heading 3 for subsections.==

## 3.2 - Paragraphs and Line Breaks

To create a ==🟢new paragraph==, ==🟢leave a blank line== between two blocks of text.

```markdown
This is the first paragraph.

This is the second paragraph.
```

To start a ==🟢new line within the same paragraph==, ==🟢add two spaces== at the end of a line, ==🟢then press Enter==.

==🟢Alternatively, in Obsidian, just press Enter== if **Strict line breaks** is disabled.

```text
This is the first line.␠␠
This is the second line.
```

Each ␠ above represents a space. Use actual spaces when typing.

## 3.3 - Text Formatting

Text formatting helps emphasize parts of a note. Wrap text in the following symbols to change its appearance:

- Bold: **bold text**                                     ==🟢`(**)`==
- Italic: *italic text*                                     ==🟢`(*)`==
- Bold and italic: ***bold and italic text***     ==🟢`(***)`==
- Strikethrough: ~~strikethrough text~~        ==🟢`(~~)`==
- Highlight: ==highlighted text==                  ==🟢`(==)`==

==Highlighting with `==` is supported by Obsidian==, but it is not part of standard Markdown.

==🟠In Obsidian, place your cursor after the opening `==`, then delete one `=` and retype it to change the text's highlight color.==
Alternatively, right-click and choose Format > Highlight > your desired color (for example, Orange).

==🟠Select some text, then type the character you want to place at the beginning and end of it (such as `=` or `*`), holding Shift if needed to type that character.== This makes it easier to format existing text. This requires **Auto-pair Markdown syntax** to be enabled. If it is disabled, enable it under **Settings > Editor > Auto-pair Markdown syntax**.

## 3.4 - Lists

Use lists to organize related items or describe steps.

### Unordered Lists

Start each item with ==🟢a hyphen (-) followed by a space==.

```markdown
- JavaScript
- TypeScript
- Python
```

### Ordered Lists

Start each item with ==🟢a number followed by a period and a space==.

```markdown
1. Open the terminal.
2. Install the dependencies.
3. Run the project.
```

### Nested Lists

==🟢Indent== an item ==🟢using Tab or four spaces== to place it inside another list item. Use ==🟢Shift + Tab== to move it back one level.

==You can combine unordered and ordered lists== when nesting items.

```markdown
- Frontend
    - HTML
    - CSS
    - JavaScript
- Backend
    1. Node.js
    2. Python
```

## 3.5 - Code

Use inline code for short expressions and code blocks for multiple lines of code or literal text.

### Inline Code

==🟢Wrap text in single backticks== (\`) to display it as inline code.

```markdown
Obsidian stores notes as `.md` files.
Use `console.log()` to print a message.
```

### Code Blocks

==🟢Place three backticks== on a separate line before and after the content to create a code block. Markdown formatting inside the block is displayed as literal text.

````text
```
# This is displayed as text, not as a heading.
```
````

### Syntax Highlighting

==🟢Add a language name immediately after the opening three backticks== to enable syntax highlighting.

````text
```javascript
const message = "Hello!";
console.log(message);
```
````

We use `markdown` for Markdown examples and `text` for plain text without syntax highlighting.

==To show triple backticks inside a code block, wrap the example in four backticks instead of three.==

## Navigation

> [!abstract] 🧭 Navigation
> **← Previous:** Currently Null
>
> **Next →:** [[3e-markdown-syntax-exercise|Markdown Syntax Exercise]]
