# Markdown Syntax: Part 2

## 4.1 - Task Lists

Task lists help you track things to do. ==🟢Start each item with `- [ ]`== for an incomplete task ==🟢or `- [x]`== for a completed task.

Leave a space between the brackets for incomplete tasks, and a space after the closing bracket before the task text.

```markdown
- [ ] Read the documentation.
- [ ] Write the code.
- [x] Create the project folder.
```

In Obsidian's Reading view, click a checkbox to mark a task as complete or incomplete.

## 4.2 - Links

Links let you connect your notes to websites or other notes.

### External Links

To link to a website, ==🟢put the link text in square brackets==, followed by ==🟢the URL in parentheses==: `[link text](URL)`.

It is similar to the anchor tag in HTML.

- ==🟡HTML Links: `<a href="URL">link text</a>`==
- ==🟡MD Links: `[link text](URL)`==

```markdown
[Obsidian Help](https://obsidian.md/help)
[MDN Web Docs](https://developer.mozilla.org)
```

The text inside the square brackets is what you see in the note. Clicking it opens the URL.

### Internal Links

In Obsidian, ==🟢wrap a note's name in double square brackets== to ==🟢link to another note== in the same vault. You do not need to include the `.md` extension.

```markdown
[[3-markdown-syntax-pt1]]
```

This format is called a *wikilink*. ==🟡It is supported by Obsidian,== but it is not part of standard Markdown. Type `[[` and start typing a note's name to see suggestions.

### Custom Link Text

Add a pipe (`|`) after the note name ==🟢to change the displayed text without changing the destination.==

```markdown
[[3-markdown-syntax-pt1|Markdown Syntax: Part 1]]
```

This displays **Markdown Syntax: Part 1** and links to `3-markdown-syntax-pt1.md`.

==🟠In Reading view, click an internal link to open the note. While editing, use Ctrl + click on Windows or Cmd + click on macOS.==

==🟠Both `internal links` and `custom link text` link to another note. The only difference is the displayed text.==

## 4.3 - Images

Images let you display screenshots, diagrams, and other visual references inside a note.

### Markdown Images

==🟢Image syntax is similar to link syntax, but starts with an exclamation mark (`!`):==

```markdown
![Alternative text](image-path-or-URL)
```

The alternative text describes the image. The parentheses contain either a local file path or an image URL.

==🟢For an image stored in the same folder as the note:==

```markdown
![Project screenshot](screenshot.png)
```

Unlike a regular link, this displays the image directly inside the note.

### Images in Your Vault

==🟢In Obsidian, add `!` before a wikilink to embed an image from your vault.==

```markdown
![[3e-markdown-syntax-reference.png]]
```

==🟡Without `!`, the wikilink opens the image when clicked. With `!`, it displays the image inside the note.==

==🟠You can also paste an image or drag it into a note.== Obsidian saves it as an attachment and inserts a reference to it.

> [!important] Important
> In Obsidian wikilinks, you can specify the full path from the vault root without adding `./` or a leading `/`. For example:
>
> ```markdown
> [[3-markdown-syntax-pt1/3-markdown-syntax-pt1]]
> ```
>
> The same approach works for image embeds:
>
> ```markdown
> ![[3-markdown-syntax-pt1/3e-markdown-syntax-reference.png]]
> ```
>
> Obsidian calls this an **absolute path in vault**. In ordinary relative file paths, `./` refers to the current folder, not the vault root.

### Resizing Images

In Obsidian, add a pipe (`|`) ==🟢followed by a width in pixels== to control the displayed size.

```markdown
![[3e-markdown-syntax-reference.png|400]]
```

This displays the image at a width of 400 pixels while keeping its proportions. It does not resize the original file.

==🟡The wikilink and resizing syntax shown here are Obsidian features==, rather than standard Markdown.

## 4.4 - Blockquotes

Blockquotes set quoted text apart from the rest of a note. ==🟢Start a line with a greater-than symbol== (`>`) followed by a space.

```markdown
> This is a blockquote.
```

### Multiple Paragraphs

To include multiple paragraphs in the same blockquote, start each line with `>`. ==🟢Use a line containing only `>` to separate the paragraphs.==

```markdown
> Read the error message carefully.
>
> It often tells you where to start debugging.
```

### Formatting Inside Blockquotes

==🟢You can use Markdown formatting inside a blockquote==, such as bold, italic, and inline code.

```markdown
> **Tip:** Use `console.log()` to inspect a value.
```

### Nested Blockquotes

==🟢Add another `>` to create a blockquote inside a blockquote.==

```markdown
> This is the outer quote.
>
> > This is a nested quote.
```

Leave a blank line without `>` before returning to normal text.

## Navigation

> [!abstract] 🧭 Navigation
> **← Previous:** [[3e-markdown-syntax-exercise|Markdown Syntax: Part 1 - Exercise]]
>
> **Next →:** [[4e-markdown-syntax-exercise|Markdown Syntax: Part 2 - Exercise]]
