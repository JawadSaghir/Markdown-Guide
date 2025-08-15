# Unordered Lists in Markdown

Unordered lists are a simple way to organize items in Markdown without numbering. They use symbols like dashes (`-`), asterisks (`*`), or plus signs (`+`) to mark list items. This guide explains how to create unordered lists, nest them, and follow best practices for compatibility.

## Creating an Unordered List

To create an unordered list, start each item with a `-`, `*`, or `+`, followed by a space and the item text. All three symbols produce the same result: a bulleted list.

**Example**:
```markdown
- Apple
- Banana
- Orange
```
**Output**:
- Apple
- Banana
- Orange

**Alternative Symbols**:
```markdown
* Apple
* Banana
* Orange
```
or
```markdown
+ Apple
+ Banana
+ Orange
```
All render the same way:
- Apple
- Banana
- Orange

## Nesting Unordered Lists

To create a nested (sub) list, indent the sub-items by **four spaces** or **one tab** under the parent item.

**Example**:
```markdown
- Fruits
    - Apple
    - Banana
- Vegetables
    - Carrot
    - Broccoli
```
**Output**:
- Fruits
    - Apple
    - Banana
- Vegetables
    - Carrot
    - Broccoli

## Starting List Items with Numbers

If an item starts with a number followed by a period (e.g., `2023.`), Markdown might mistake it for an ordered list. To prevent this, use a backslash (`\`) before the period.

**Example**:
```markdown
- 2023\. A great year!
- 2024\. Even better!
```
**Output**:
- 2023. A great year!
- 2024. Even better!

**Without Backslash (Incorrect)**:
```markdown
- 2023. A great year!
```
This might render as an ordered list, which is not the intended behavior.

## Adding Elements to Lists

You can add other Markdown elements (e.g., paragraphs, blockquotes, code blocks) within a list by indenting them **four spaces** or **one tab** under the list item.

### Paragraphs
```markdown
- Item 1
- Item 2
    This is an extra paragraph for Item 2.
- Item 3
```
**Output**:
- Item 1
- Item 2
    This is an extra paragraph for Item 2.
- Item 3

### Blockquotes
```markdown
- Item 1
- Item 2
    > This is a blockquote for Item 2.
- Item 3
```
**Output**:
- Item 1
- Item 2
    > This is a blockquote for Item 2.
- Item 3

### Code Blocks
Code blocks in lists need **eight spaces** or **two tabs** for proper indentation.
```markdown
- Step 1
- Step 2
        <html>
            <title>My Site</title>
        </html>
- Step 3
```
**Output**:
- Step 1
- Step 2
        <html>
            <title>My Site</title>
        </html>
- Step 3

## Best Practices

1. **Use Consistent Symbols**: Stick to one symbol (`-`, `*`, or `+`) for the entire list to avoid rendering issues.
   - **Do**:
     ```markdown
     - Item 1
     - Item 2
     - Item 3
     ```
   - **Don’t**:
     ```markdown
     - Item 1
     * Item 2
     + Item 3
     ```

2. **Add Blank Lines**: Place blank lines before and after the list for better compatibility with Markdown processors.
   - **Do**:
     ```markdown
     Text before...

     - Item 1
     - Item 2

     Text after...
     ```
   - **Don’t**:
     ```markdown
     Text before...
     - Item 1
     - Item 2
     Text after...
     ```

3. **Use Backslashes for Numbers**: Always escape periods after numbers (e.g., `2023\.`) to ensure they render as unordered list items.

4. **Check Indentation**: Ensure nested items and additional elements are indented correctly (four spaces or one tab for most elements, eight spaces for code blocks).

## Why Use Unordered Lists?

Unordered lists are ideal for items that don’t require a specific order, such as:
- Shopping lists
- Feature lists
- Checklists
- Categories or groups

By following these guidelines, your unordered lists will be clear, consistent, and compatible across different Markdown applications.