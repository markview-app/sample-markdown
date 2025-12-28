# Line Breaks Behavior Test

This document tests MarkView's line break behavior. MarkView uses CommonMark standard (`breaks: false`), which means single newlines are treated as spaces.

---

## How Line Breaks Work in MarkView

MarkView follows CommonMark standard where single newlines are treated as spaces. To create line breaks, you need:

- **Two trailing spaces + newline, OR**
- **Explicit `<br>` tag, OR**
- **Double newline (blank line) to create a new paragraph**

---

## Test Case 1: Single Newlines (No trailing spaces)

This is the first line.
This is the second line.
This is the third line.

**Expected**: All three lines should appear as one continuous line (spaces between them).

---

## Test Case 2: Double Newlines (Paragraph Break)

This is paragraph one.

This is paragraph two.

This is paragraph three.

**Expected**: Creates separate paragraphs with proper spacing.

---

## Test Case 3: Two Trailing Spaces + Newline

This is the first line with two spaces.  
This is the second line with two spaces.  
This is the third line.

**Expected**: Creates hard line breaks between each line.

---

## Test Case 4: Explicit `<br>` Tags

This is the first line.<br>
This is the second line.<br>
This is the third line.

**Expected**: Creates hard line breaks between each line.

---

## Test Case 5: Mixed Scenarios

Here's a complex example:
Line 1 - single newline
Line 2 - single newline  
Line 3 - two trailing spaces

Line 4 - after blank line<br>
Line 5 - after br tag

**Expected**:

- Lines 1 and 2 merge together (single newlines become spaces)
- Line 3 has a break before it (due to trailing spaces on line 2)
- Line 4 starts a new paragraph (blank line creates paragraph break)
- Line 5 has a break before it (due to br tag)

---

## Test Case 6: Poetry/Lyrics (Common Use Case)

### Without Hard Breaks

Roses are red,
Violets are blue,
Sugar is sweet,
And so are you.

### With Trailing Spaces (Hard Breaks)

Roses are red,  
Violets are blue,  
Sugar is sweet,  
And so are you.

### With Explicit BR Tags

Roses are red,<br>
Violets are blue,<br>
Sugar is sweet,<br>
And so are you.

**Note**: In MarkView, the first version appears as a single line. Use trailing spaces or `<br>` tags for poetry formatting.

---

## Test Case 7: Code Blocks (Should Not Be Affected)

```
Line 1
Line 2
Line 3
```

**Expected**: Line breaks in code blocks are always preserved.

---

## Test Case 8: Lists

Unordered list:

- Item 1
- Item 2
- Item 3

Ordered list:

1. First item
2. Second item
3. Third item

**Expected**: Lists always work correctly with proper line breaks.

---

## Summary

| Scenario | MarkView Behavior |
|----------|------------------|
| Single newline | Converted to space |
| Double newline (blank line) | New paragraph (`<p>`) |
| Two trailing spaces + newline | Creates `<br>` |
| Explicit `<br>` tag | Creates `<br>` |
| Code blocks | Line breaks preserved |
| Lists | Line breaks preserved |

---

## Testing Instructions

1. Open this file in MarkView
2. Check that single newlines in Test Case 1 appear as one continuous line
3. Check that poetry in Test Case 6 (first version) appears on one line
4. Verify that trailing spaces and `<br>` tags create proper line breaks
5. Confirm that double newlines create paragraph breaks
6. Notice that the second and third poetry versions display correctly with line breaks

---

## Why CommonMark?

MarkView uses CommonMark standard (`breaks: false`) because:

- ✅ Single newlines → spaces (standard markdown behavior)
- ✅ Requires explicit intent for line breaks (2 trailing spaces or `<br>`)
- ✅ More predictable and portable across markdown renderers
- ✅ Prevents accidental line breaks from text editor line wrapping
