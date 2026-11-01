# Markdown Syntax: Part 3

## 5.1 - Callouts

Callouts highlight information in a box, such as a tip, warning, or summary. ==🟡They are an Obsidian feature==, not standard Markdown.

### Basic Syntax

==🟢Start a blockquote with a callout type such as `[!info]`==. Keep `>` at the beginning of each line.

```markdown
> [!info]
> This is an information box.
```

> [!info]
> This is an information box.
### Types and Titles

The type determines the default color and icon. Your theme may change their appearance.

==🟢Common types include `[!note]`, `[!tip]`, `[!warning]`, `[!example]`, and `[!abstract]`==.

==🟢Add text after the type== to set a custom title.

```markdown
> [!warning] Before You Start
> Save your work first.
```

> [!warning] Before You Start
> Save your work first.

==🟡Without a custom title, Obsidian uses the type name.==

### Content Inside Callouts

==🟢Callouts support formatting, links, and lists.== Use a line containing only `>` to separate paragraphs.

```markdown
> [!tip] Debugging
> Read the **error message**.
>
> Check [[3-markdown-syntax-pt1]] for formatting examples.
```

> [!tip] Debugging
> Read the **error message**.
>
> Check [[3-markdown-syntax-pt1]] for formatting examples.
### Foldable Callouts

==🟢Add `-` immediately after the type to start collapsed, or `+` to start expanded.== Click the title to toggle it.

```markdown
> [!example]- Show Example
> This content starts hidden.
```

> [!example]- Show Example
> This content starts hidden.

## 5.2 - Horizontal Rules

Horizontal rules visually separate sections of a note. ==🟢Place three or more hyphens (`---`), asterisks (`***`), or underscores (`___`) on their own line.==

```markdown
This is the first section.

---

This is the second section.
```

==🟢Leave a blank line before and after the rule.== Without a blank line before `---`, the preceding text may become a heading instead.

All three styles produce a horizontal line:

```markdown
---

***

___
```

---

***

___

## 5.3 - Tables

Tables organize information into rows and columns. ==🟢Use pipes (`|`)== to separate columns ==🟢and a row of hyphens== to separate the header from the data.

### Basic Syntax

```markdown
| Language   | Main Use        |
| ---------- | --------------- |
| JavaScript | Web development |
| Python     | Automation      |
```

| Language   | Main Use        |
| ---------- | --------------- |
| JavaScript | Web development |
| Python     | Automation      

The first row contains column headings. ==🟡Each cell in the separator row needs at least three hyphens.==

Spaces help keep the source readable, but columns do not need to have equal widths.

### Column Alignment

==🟢Add colons (`:`)== to the separator row ==🟢to set the alignment==:

- `:---` aligns left.
- `:---:` centers the content.
- `---:` aligns right.

```markdown
| Topic    | Status      | Exercises |
| :------- | :---------: | --------: |
| Headings | Complete    |         2 |
| Tables   | In progress |         1 |
```

### Formatting Inside Cells

==🟢You can use inline formatting and links== inside table cells.

```markdown
| Item    | Description                    |
| ------- | ------------------------------ |
| `const` | Declares a **constant binding** |
| Help    | [Obsidian](https://obsidian.md) |
```

To display a literal pipe inside a cell, escape it with a backslash: `\|`.

## 5.4 - Escaping Characters

Markdown uses characters such as `*`, `#`, and `>` for formatting. To display a formatting character literally, ==🟢place a backslash (`\`)== before it. This is called escaping.

### Basic Syntax

```markdown
\*This text is not italic.\*
\# This line is not a heading.
\> This line is not a blockquote.
```

The backslash prevents formatting and is not displayed in the rendered text.

### Escaping List Markers

==🟢Escape the hyphen== to prevent a bullet list. For a numbered list, ==🟢escape the period== after the number.

```markdown
\- This is not a list item.
1\. This is not a numbered list item.
```

### Escaping vs. Code

==🟡Use escaping when you want special characters to appear as normal text. Use inline code or code blocks when showing syntax or code.==

```markdown
Use \* for emphasis.
Use `*` for emphasis.
```

Both examples display an asterisk, but the second uses code styling. Inside inline code and fenced code blocks, Markdown formatting characters are already displayed literally, so you do not need to escape them.

## 5.5 - Comments

Comments let you leave reminders or editing notes that are visible while editing but hidden in Reading view. ==🟢Obsidian uses `%%` to mark comments==. This syntax is specific to Obsidian.

### Inline Comments

==🟢Wrap text in `%%`== to add a comment within a line.

```markdown
JavaScript is a programming language. %%Add an example later.%%
```

In Reading view, only the sentence outside the comment is displayed.

### Block Comments

==🟢Place `%%` on separate lines== to create a comment spanning multiple lines.

```markdown
%%
Review this section.
Add a code example.
%%
```

### Closing Comments

==🟡Always close a comment with another `%%`==. An unclosed block comment can hide the rest of your note in Reading view.

Comments remain in the `.md` file. They are not private or deleted; anyone who can access the file can read them.

## Navigation

> [!abstract] 🧭 Navigation
> **← Previous:** [[4e-markdown-syntax-exercise|Markdown Syntax: Part 2 - Exercise]]
>
> **Next →:** [[5e-markdown-syntax-exercise|Markdown Syntax: Part 3 - Exercise]]
