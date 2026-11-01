# Markdown Syntax: Part 3 - Exercise

Recreate the note shown in the reference image using Markdown. This exercise practices the five topics covered in [[5-markdown-syntax-pt3]]: callouts, horizontal rules, tables, escaping characters, and comments.

## Instructions

1. Create a new vault named `5e`.
2. Inside the vault, create a note named `exercise-sol-5e` (the file will be `exercise-sol-5e.md`). Reproduce the text, structure, and formatting shown in the reference image. No additional images or notes need to be copied into this vault.
3. Add `# Release Notes Practice` as Heading 1 in the Markdown source. Use Heading 2 for Release Reminders, Release Summary, and Literal Characters.
4. Under Release Reminders, create a `warning` callout titled `Before Deployment`. Its body should read `Create a backup before updating.`, with only the word `backup` in bold. Then create a foldable `example` callout titled `Show Command` that starts collapsed. Its hidden body must read `Run npm run build before deployment.`, with `npm run build` formatted as inline code. Expand it to check the body, then collapse it again to match the image.
5. Add two horizontal rules: one between Release Reminders and Release Summary, and one between Release Summary and Literal Characters. Use any of the horizontal-rule styles covered in the lesson, with blank lines around them.
6. Create the Release Summary table with the three headers and three data rows shown in the image. Explicitly align Module to the left, Status to the center, and Warnings to the right using the separator row. Preserve the text and numbers from the reference.
7. Under Literal Characters, reproduce the following as four separate normal paragraphs. Use backslash escaping, not inline code, code blocks, headings, or lists. The visible asterisks must not make the sentence italic. Use an ordinary hyphen (`-`) for the third paragraph, regardless of its appearance in the image.

   ```text
   *Do not format this sentence.*
   # Not a heading
   - Not a list item.
   1. Not a numbered list item.
   ```

8. Add an inline comment, `%%Check the release date.%%`, at the end of the introductory paragraph, on the same source line. After the final paragraph, add a block comment containing these two lines, with opening and closing `%%` on separate lines:

   ```text
   Review the warning message.
   Confirm the module statuses.
   ```

9. Switch to Reading view and compare your note with the reference image. The comments must be hidden, the example callout must start collapsed, and the final sentence must remain visible outside the comments and callouts.

The image shows Reading view, so the comments and collapsed callout body are intentionally invisible. Follow the written instructions for these requirements. Focus on Markdown structure rather than exact font sizes, colors, spacing, callout icons, or table borders, which depend on your theme.

Try writing the note yourself first. If you get stuck, refer to [[5-markdown-syntax-pt3]], then continue the exercise.

## Reference Image

![[5e-markdown-syntax-reference.png|408]]

## Grading

When you finish, give an AI agent read access to your `5e` solution vault and ask it to grade your work. The agent can read the solution directly, so you do not need to upload it separately.

Send the following two files together with the prompt below. Replace the vault path placeholder with the full path to your solution vault.

### Files to Submit

- `5e-markdown-syntax-reference.png`
- `5e-markdown-syntax-exercise.md`

### Prompt

```text
Grade my Markdown exercise by inspecting the solution vault you have access to:
Vault path: <full path to my 5e vault>

Read exercise-sol-5e.md from that vault. Do not modify any files.

Use these two attached files:
- 5e-markdown-syntax-reference.png: the rendered reference image.
- 5e-markdown-syntax-exercise.md: the exercise instructions, including requirements invisible in the image.

Give a score out of 100, with up to 20 points for each category:
1. Callouts: a warning callout titled Before Deployment with the correct body and bold backup; a foldable example callout titled Show Command, collapsed by default, with the prescribed hidden body and inline-code command. Inspect the source to verify the hidden body and folding marker.
2. Horizontal rules: two valid rules in the prescribed positions, correctly separated from surrounding content. Accept all horizontal-rule styles taught in the lesson.
3. Tables: correct headers, data, and explicit left/center/right alignment for Module/Status/Warnings. Do not require evenly spaced source columns or exact rendered borders or widths.
4. Escaping characters: the four prescribed literal paragraphs use backslash escaping correctly and remain normal text. Preserve visible punctuation without creating italics, a heading, or a list. Do not accept code styling as a substitute for this exercise. The third paragraph uses an ASCII hyphen even if the image appears to show a longer dash.
5. Comments: the prescribed inline comment occurs on the introductory paragraph's source line; the prescribed two-line block comment occurs after the final paragraph with separate opening and closing delimiter lines. All comments are closed, hidden in Reading view, and leave the visible note content intact.

Also check the H1 title (Release Notes Practice), the three H2 headings, and visible text against the instructions and image. Report any general structure or text errors separately; deduct only within a relevant category, and do not penalize the same error twice. The filename does not replace the H1 title.

Accept equivalent valid Markdown and Obsidian syntax except where the instructions explicitly require backslash escaping or a particular callout type, default folding state, or table alignment. Do not deduct points for theme-dependent font sizes, colors, spacing, icons, or borders. Where the image and written instructions differ, follow the written instructions. Do not penalize the hidden comments or hidden callout body for being absent from the rendered image.

Only claim to have verified files, settings, or rendered output that you actually inspected. If you cannot access the solution vault or inspect the reference image, report the limitation rather than treating an unverified item as a mistake. Do not grade the learning notes' navigation as part of the solution.

Report each category's score and explain any deductions. For each mistake, quote the relevant source, explain the issue, and show a minimal correction. Do not rewrite the entire note. Finish with the total score and the main things I should practice next. Give your feedback in Turkish.
```

## Navigation

> [!abstract] 🧭 Navigation
> **← Previous:** [[5-markdown-syntax-pt3|Markdown Syntax: Part 3]]
>
> **Next →:** Currently Null
