# for heading
## heading 2
### heading 3

- unordered items
1. ordered list
    1. sub list 
    2. sub list 2

*Italic  block*

**Bold text**


***bold and itelic***

>to create a block

>Enter is the line sepratar


| cloumn-1 | column 2 | column3 |
|----------|----------|---------|
| items-1  | item-2   | item3   |
| row-3    | row-4 | row 5|
     
add a image by ![](../img/caller.png)

> [!NOTE]
> Useful information that users should know, even when skimming content.

# alert:
> [!NOTE]
> useful 

![task-06](image.png)  


# Notes for Creating a Markdown File

## What is Markdown?
- **Markdown** is a lightweight markup language used for formatting plain text.
- It is widely used for documentation, README files, and writing on the web.

## Basic Syntax

### Headings
- Use `#` for headings. The number of `#` indicates the level of the heading.
  ```markdown
  # H1
  ## H2
  ### H3
  ```

### Emphasis
- **Bold**: Use `**text**` or `__text__`.
- *Italic*: Use `*text*` or `_text_`.
- ***Bold and Italic***: Use `***text***`.

### Lists
- **Unordered List**: Use `-`, `*`, or `+`.
  ```markdown
  - Item 1
  - Item 2
    - Sub-item
  ```
- **Ordered List**: Use numbers followed by a period.
  ```markdown
  1. First
  2. Second
  ```

### Links
- Inline Link:
  ```markdown
  [Link Text](URL)
  ```
- Reference-style link:
  ```markdown
  [Link Text][id]
  [id]: URL
  ```

### Images
- Inline Image:
  ```markdown
  ![Alt Text](Image_URL)
  ```
- Reference-style image:
  ```markdown
  ![Alt Text][id]
  [id]: Image_URL
  ```

### Code
- Inline code: Use backticks: `` `code` ``
- Block code: Use triple backticks or indent with four spaces:
  ```markdown
  ```
  Code block
  ```
  ```

### Blockquotes
- Use `>` to create blockquotes:
  ```markdown
  > This is a blockquote.
  ```

### Horizontal Rule
- Use three or more `---`, `***`, or `___`:
  ```markdown
  ---
  ```

## Tables
- Use pipes `|` and dashes `-`:
  ```markdown
  | Header 1 | Header 2 |
  |----------|----------|
  | Row 1    | Data 1   |
  | Row 2    | Data 2   |
  ```

## Checklist
- Use `- [ ]` for an unchecked box and `- [x]` for a checked box:
  ```markdown
  - [ ] Task 1
  - [x] Task 2
  ```

## Additional Tips
- Save the file with a `.md` extension.
- Markdown is rendered differently on various platforms; test your file before sharing.
- Use tools like VS Code, Typora, or Obsidian for creating and previewing Markdown files.
