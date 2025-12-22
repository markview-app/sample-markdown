# Syntax Highlighting Demo

> This document tests MarkView's syntax highlighting capabilities across various programming languages and plain text scenarios.

## Language Labels

Language labels should appear in the top-left corner of code blocks.

### JavaScript

```javascript
function calculateTotal(items) {
  return items.reduce((sum, item) => sum + item.price, 0);
}
```

### Python

```python
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n-1) + fibonacci(n-2)
```

### TypeScript

```typescript
interface Product {
  id: number;
  name: string;
  price: number;
}

const products: Product[] = [
  { id: 1, name: 'Laptop', price: 999 },
  { id: 2, name: 'Mouse', price: 29 }
];
```

### CSS

```css
.button {
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  border: none;
  border-radius: 8px;
  padding: 12px 24px;
  color: white;
  font-weight: 600;
}
```

### SQL

```sql
SELECT u.name, COUNT(o.id) as order_count
FROM users u
LEFT JOIN orders o ON u.id = o.user_id
WHERE u.active = true
GROUP BY u.id, u.name;
```

### Bash

```bash
#!/bin/bash
for file in *.md; do
  echo "Processing $file"
  pandoc "$file" -o "${file%.md}.html"
done
```

## Plain Text (No Highlighting)

Plain text blocks should NOT have syntax highlighting colors applied.

### No Language Specified

```
This is plain text.
It should not have any syntax highlighting colors.
Just plain monospace text with no colors.

123456
ABCDEF
special@characters#here
```

### Explicit "text" Language

```text
This is also plain text.
Using the explicit "text" language.
No colors should be applied here either.

Variable = Value
Function()
Random words and numbers: 42
```

### Very Long Plain Text Line

```text
This is a very long line of plain text that is intended to test how the syntax highlighting handles long lines without any specific language. It should remain uncolored and simply wrap or scroll as needed based on the viewer's settings, ensuring that no syntax highlighting is applied whatsoever.
```

### Comparison: With vs Without Highlighting

**Plain text (should be monochrome):**

```
function test() {
  console.log("no colors");
  return true;
}
```

**JavaScript (should have syntax highlighting):**

```javascript
function test() {
  console.log("has colors");
  return true;
}
```

## Other Languages

### HTML

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Test Page</title>
</head>
<body>
  <h1>Hello World</h1>
</body>
</html>
```

### JSON

```json
{
  "name": "markview",
  "version": "1.0.0",
  "features": [
    "syntax-highlighting",
    "language-labels",
    "code-copy"
  ]
}
```

### Markdown

```markdown
# Markdown in Markdown

- Item 1
- Item 2

**Bold** and *italic* text.
```

### YAML

```yaml
name: markview
version: 1.0.0
features:
  - syntax-highlighting
  - language-labels
  - code-copy
```

### XML

```xml
<note>
  <to>User</to>
  <from>MarkView</from>
  <heading>Reminder</heading>
  <body>Don't forget to test syntax highlighting!</body>
</note>
```
