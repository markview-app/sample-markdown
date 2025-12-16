# Syntax Highlighting Test

This file tests the improved syntax highlighting feature with language labels and proper plain text handling.

## Issue 1: Language Labels

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

## Issue 2: Plain Text (No Highlighting)

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

### Very long Plain Text

```text
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer ornare suscipit facilisis. Suspendisse ultricies mi nec risus vulputate pulvinar. Pellentesque mollis justo eget lacinia elementum. Mauris tempus metus nulla, fermentum gravida turpis luctus in. Sed eu interdum urna. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Praesent non hendrerit augue.

Nulla odio purus, volutpat sit amet augue sit amet, rutrum bibendum enim. Nam posuere tellus eget diam malesuada, in pulvinar lorem pharetra. Etiam efficitur ligula neque, blandit hendrerit nunc posuere in. Nunc pharetra lorem vel lectus pharetra, sed congue velit gravida. Nam metus nisi, sollicitudin ac tincidunt ut, hendrerit nec ante. Duis rhoncus ultricies gravida. Nunc libero diam, maximus sed neque eu, commodo scelerisque justo. Sed suscipit sem felis, et finibus mi aliquam et. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Sed luctus auctor enim ut consequat. Vivamus tempus hendrerit ex, nec condimentum tortor eleifend eu. Nullam lacus libero, eleifend vel semper non, vulputate eget risus. Praesent ac ornare nulla.

Donec congue augue elit, id egestas neque pharetra sit amet. Quisque libero nulla, consectetur at eros id, laoreet aliquam est. Quisque in nunc ornare, semper eros ac, mollis orci. Nulla pellentesque mattis diam id sagittis. Maecenas eget feugiat leo. Vestibulum rutrum id velit non ornare. Maecenas semper turpis sed faucibus tristique. Sed dictum malesuada elit. Aenean risus odio, pulvinar a luctus sed, viverra id nunc. Pellentesque bibendum pretium arcu non aliquam. Proin sit amet rutrum orci, et euismod augue.

Praesent nisi tellus, consequat ac dui sit amet, vestibulum cursus sapien. Quisque a vehicula sapien. In faucibus, ex sed vehicula consectetur, orci orci laoreet sapien, a finibus orci lacus vel quam. Duis nec leo justo. Curabitur placerat euismod ante non vehicula. Phasellus rutrum egestas consequat. Phasellus efficitur, lorem accumsan dapibus facilisis, felis diam molestie libero, in facilisis odio quam vel lorem. Nam purus metus, semper vel leo in, ultricies congue lectus. Cras lobortis orci velit, at dignissim ante convallis non. Phasellus scelerisque nulla magna, quis tempor quam pulvinar id. Sed ultricies, ante quis luctus venenatis, quam urna pretium purus, id auctor eros sapien vitae nibh. Integer eu suscipit justo, rutrum consequat dui. Quisque dapibus, nisi vel dapibus finibus, mi libero accumsan turpis, in vulputate odio sem et nisl.

Morbi facilisis tincidunt metus id molestie. Aenean quis sem nec orci tincidunt sagittis non nec purus. Cras metus dolor, vehicula non pulvinar sed, ullamcorper nec magna. Etiam sed purus quis libero porta placerat. Vivamus diam est, pulvinar tincidunt sem ac, vehicula fringilla erat. Donec lorem odio, volutpat sit amet metus id, porttitor gravida enim. Nulla facilisis hendrerit diam, a dictum dui scelerisque et. Pellentesque tempus eleifend nisl. Vestibulum metus nisl, eleifend vel neque eget, fringilla aliquam nibh.
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
