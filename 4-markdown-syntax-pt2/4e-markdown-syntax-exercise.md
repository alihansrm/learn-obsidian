# Markdown Syntax: Part 2 - Exercise

Recreate the note shown in the reference image using Markdown. This exercise practices the four topics covered in [[4-markdown-syntax-pt2]]: task lists, links, images, and blockquotes. It also uses headings and basic text formatting from Part 1.

## Instructions

1. Create a new vault named `4e`.
2. Copy `3-markdown-syntax-pt1.md` and `3e-markdown-syntax-reference.png` from your learning vault into the new vault. These provide the internal link destination and the image used in this exercise.
3. Inside the new vault, create a note named `exercise-sol-4e` (the file will be `exercise-sol-4e.md`). Copy the text from the reference image and reproduce its structure and formatting using Markdown.
4. Add `# My Developer Study Plan` as Heading 1 in the Markdown source. Use Heading 2 for Tasks, Useful Links, Reference Image, and Study Reminders.
5. Under Tasks, create four checkbox items. Mark the first two as complete and leave the last two incomplete. Use task-list syntax; you do not need to add separate strikethrough formatting to completed tasks.
6. Under Useful Links, create a bulleted list with these three links in order:
    - An external link labeled **MDN Web Docs**, pointing to `https://developer.mozilla.org`.
    - An internal link to `3-markdown-syntax-pt1`, using the note name as its displayed text.
    - Another internal link to the same note, with **Review Part 1** as its custom displayed text.
7. Under Reference Image, show the source filename as inline code and embed `3e-markdown-syntax-reference.png` at a width of 220 pixels, keeping its proportions. Use the image file itself; do not recreate the contents of the small thumbnail. The large `4e-markdown-syntax-reference.png` image is the exercise reference, not the image to embed in your solution.
8. Under Study Reminders, create one blockquote containing two separate paragraphs, with the word `documentation` in bold. Then create a separate blockquote containing `When something fails:` and a nested blockquote beneath it. Keep the final sentence, `Small steps make progress easier to track.`, outside all blockquotes.
9. Switch to Reading view and compare your note with the reference image. Test the links and check that the embedded image appears.

Focus on the Markdown structure rather than exact font sizes, colors, or spacing, which depend on your theme. Link icons, checkbox styling, and the appearance of completed tasks may also differ. You can open the reference image to inspect it at a larger size.

Try writing the note yourself first. If you get stuck, refer to [[4-markdown-syntax-pt2]], then continue the exercise. The copied Part 1 note is only a link destination; you do not need to make all of its own links work in the exercise vault.

## Reference Image

![[4e-markdown-syntax-reference.png|408]]

## Grading

When you finish, give an AI agent read access to your `4e` solution vault and ask it to grade your work. The agent can inspect your solution, internal link destination, and embedded image directly from the vault, so you do not need to upload those files separately.

Send the following two files together with the prompt below. Replace the vault path placeholder in the prompt with the full path to your solution vault.

### Files to Submit

- `4e-markdown-syntax-reference.png`
- `4e-markdown-syntax-exercise.md`

### Prompt

```text
Grade my Markdown exercise by inspecting the solution vault you have access to:
Vault path: <full path to my 4e vault>

Read exercise-sol-4e.md from that vault. Inspect the internal link destination and embedded image files there as needed. Do not modify any files.

Use these two attached files as the reference and instructions:
- 4e-markdown-syntax-reference.png: the reference image to recreate.
- 4e-markdown-syntax-exercise.md: the exercise instructions.

Compare my solution's Markdown source with the reference image and instructions. Give a score out of 100 using these categories:
1. Structure and basic formatting (10 points): correct H1 title (My Developer Study Plan), four H2 sections, text content, inline-code filename, and bold documentation. The H1 must appear in the Markdown source; the filename alone does not satisfy this requirement.
2. Task lists (20 points): four correctly written checkbox items with the first two complete and the last two incomplete. Do not require separate strikethrough markup for completed tasks.
3. Links (25 points): a bulleted external link labeled MDN Web Docs pointing to https://developer.mozilla.org, a normal internal link to 3-markdown-syntax-pt1, and a second internal link to the same note with Review Part 1 as its custom text. Accept a trailing slash on the external URL.
4. Images (25 points): embed 3e-markdown-syntax-reference.png rather than the full exercise reference, specify a width of 220 pixels, and preserve its proportions. Check the embed syntax and target filename. Do not expect the thumbnail's contents to be recreated as text.
5. Blockquotes (20 points): one blockquote with two separate paragraphs, then a separate blockquote containing a nested quote. The final sentence must be outside the quotes.

Accept equivalent valid Markdown and Obsidian syntax, including valid relative paths. Do not deduct points for theme-dependent font sizes, colors, spacing, link icons, or checkbox styling. Where the image and instructions differ, follow the written instructions. Do not interpret bold emphasis in the instructions as a requirement unless explicitly stated.

Check that the internal links and image embed resolve to existing files inside the solution vault. Inspect the embedded image to confirm it is the intended reference. The copied Part 1 note is only a link destination; do not grade its content or require its own links to resolve. Only claim to have verified files, settings, or rendered output that you actually inspected. If rendering depends on an Obsidian setting you cannot verify, state that limitation rather than assuming the setting. If you cannot access the vault or inspect an image, report the limitation instead of treating an unverified item as a mistake. Do not grade navigation sections from the learning notes as part of the solution.

Report each category's score and briefly explain any deductions. For each mistake, quote the relevant part of my solution, explain the issue, and show a minimal correction. Do not rewrite the entire note. Finish with the total score and the main things I should practice next. Give your feedback in Turkish.
```

## Navigation

> [!abstract] 🧭 Navigation
> **← Previous:** [[4-markdown-syntax-pt2|Markdown Syntax: Part 2]]
>
> **Next →:** [[5-markdown-syntax-pt3|Markdown Syntax: Part 3]]
