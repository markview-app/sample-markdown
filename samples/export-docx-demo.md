# DOCX Export Test Document

This document tests all features: **images**, **syntax highlighting**, and **enhanced tables**.

Please click the "Export to DOCX" button in **MarkView** to generate a Word document and verify that all content is rendered correctly.

---

## 1. Image Support Testing

### 1.1 Remote Images (HTTP/HTTPS)

Here's the Markdown logo from the web:

![Markdown Logo](https://upload.wikimedia.org/wikipedia/commons/4/48/Markdown-mark.svg)

### 1.2 Small Image

![GitHub Icon](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)

### 1.3 Data URL Image (Base64)

![Red Square](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAoAAAAKCAYAAACNMs+9AAAAFUlEQVR42mP8z8BQz0AEYBxVSF+FABJADveWkH6oAAAAAElFTkSuQmCC)

---

## 2. Syntax Highlighting Testing

### 2.1 JavaScript Code

```javascript
// JavaScript example with various syntax elements
function greet(name) {
  const greeting = `Hello, ${name}!`;
  console.log(greeting);
  return greeting;
}

class Person {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  introduce() {
    return `I'm ${this.name} and I'm ${this.age} years old.`;
  }
}

const person = new Person('Alice', 30);
console.log(person.introduce());
```

### 2.2 TypeScript Code

```typescript
// TypeScript example with type annotations
interface User {
  id: number;
  name: string;
  email: string;
  role: 'admin' | 'user' | 'guest';
}

function getUserInfo(user: User): string {
  return `${user.name} (${user.email}) - Role: ${user.role}`;
}

const admin: User = {
  id: 1,
  name: 'Bob',
  email: 'bob@example.com',
  role: 'admin',
};

console.log(getUserInfo(admin));
```

### 2.3 Python Code

```python
# Python example with various features
def fibonacci(n):
    """Generate Fibonacci sequence up to n terms."""
    if n <= 0:
        return []
    elif n == 1:
        return [0]

    sequence = [0, 1]
    for i in range(2, n):
        sequence.append(sequence[i-1] + sequence[i-2])

    return sequence

class Animal:
    def __init__(self, name, species):
        self.name = name
        self.species = species

    def make_sound(self):
        return f"{self.name} the {self.species} makes a sound"

dog = Animal("Rex", "Dog")
print(dog.make_sound())
print(fibonacci(10))
```

### 2.4 HTML/CSS Code

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Test Page</title>
    <style>
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        .button {
            background-color: #007bff;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Hello World</h1>
        <button class="button">Click Me</button>
    </div>
</body>
</html>
```

### 2.5 JSON Data

```json
{
  "name": "MarkView",
  "version": "1.0.3",
  "description": "Modern Markdown Viewer",
  "features": [
    "Syntax highlighting",
    "Image support",
    "Enhanced tables",
    "DOCX export"
  ],
  "settings": {
    "theme": "auto",
    "fontSize": 14,
    "enableExport": true
  }
}
```

### 2.6 SQL Queries

```sql
-- SQL example with various operations
CREATE TABLE users (
    id INT PRIMARY KEY AUTO_INCREMENT,
    username VARCHAR(50) NOT NULL UNIQUE,
    email VARCHAR(100) NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

INSERT INTO users (username, email)
VALUES ('alice', 'alice@example.com'),
       ('bob', 'bob@example.com');

SELECT u.username, u.email, COUNT(o.id) as order_count
FROM users u
LEFT JOIN orders o ON u.id = o.user_id
WHERE u.created_at > '2024-01-01'
GROUP BY u.id
HAVING order_count > 5
ORDER BY order_count DESC;
```

---

## 3. Enhanced Table Testing

### 3.1 Simple Data Table

| Name | Age | City | Occupation |
|------|-----|------|------------|
| Alice | 30 | New York | Engineer |
| Bob | 25 | Los Angeles | Designer |
| Charlie | 35 | Chicago | Manager |
| Diana | 28 | Boston | Developer |

### 3.2 Feature Comparison Table

| Feature | Phase 1 | Phase 2 | Phase 3 (Planned) |
|---------|---------|---------|-------------------|
| Headings | ✅ | ✅ | ✅ |
| Lists | ✅ | ✅ | ✅ |
| Code Blocks | ✅ Plain | ✅ **Highlighted** | ✅ Highlighted |
| Images | ❌ | ✅ **New!** | ✅ |
| Tables | ✅ Basic | ✅ **Enhanced** | ✅ Enhanced |
| Math | ❌ | ⏳ Partial | ✅ Full OMML |

### 3.3 Numeric Data Table

| Product | Q1 Sales | Q2 Sales | Q3 Sales | Q4 Sales | Total |
|---------|----------|----------|----------|----------|-------|
| Widget A | $12,500 | $15,300 | $18,700 | $22,100 | $68,600 |
| Widget B | $8,200 | $9,500 | $11,300 | $13,800 | $42,800 |
| Widget C | $15,600 | $17,200 | $19,800 | $24,500 | $77,100 |

---

## 4. Combined Features Test

### 4.1 Code Block in List

Here's a shopping list with code examples:

1. **First item**: Install dependencies

   ```bash
   npm install docx unified remark-parse
   ```

2. **Second item**: Create configuration

   ```javascript
   const config = {
     theme: 'light',
     export: {
       format: 'docx',
       images: true
     }
   };
   ```

3. **Third item**: Run the application

   ```bash
   npm start
   ```

### 4.2 Table with Code References

| Language | Example Function | Description |
|----------|------------------|-------------|
| JavaScript | `console.log()` | Print to console |
| Python | `print()` | Output to stdout |
| Java | `System.out.println()` | Print with newline |

### 4.3 Nested Lists with Images

1. **Frontend Technologies**
   - React
   - Vue
   - Angular

2. **Backend Technologies**
   - Node.js
   - Python
   - Go

3. **Tools**
   - VSCode
   - Git
   - Docker

### 4.4 Task Lists (Checkboxes)

**Project Setup Checklist:**

- [x] Initialize Git repository
- [x] Install dependencies via npm
- [x] Configure ESLint and Prettier
- [ ] Write unit tests
- [ ] Set up CI/CD pipeline
- [ ] Deploy to production

**Feature Implementation:**

1. **Phase 1 Tasks**
   - [x] Basic markdown parsing
   - [x] Simple text rendering
   - [x] List support

2. **Phase 2 Tasks**
   - [x] Image support
   - [x] Syntax highlighting
   - [x] Enhanced tables
   - [ ] Math equations (OMML)

3. **Phase 3 Tasks**
   - [ ] Mermaid diagrams
   - [ ] Custom themes
   - [ ] Export templates

---

## 5. Text Formatting Tests

### 5.1 Inline Formatting

This paragraph contains **bold text**, *italic text*, ***bold and italic***, ~~strikethrough text~~, and `inline code`.

### 5.2 Blockquotes

> This is a blockquote with a **bold** word.
>
> It can span multiple paragraphs and include *italic* text too.

---

## 6. Links and References

Check out these resources:

- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Flavored Markdown](https://github.github.com/gfm/)
- [CommonMark Spec](https://commonmark.org/)

---

## 7. Advanced Code Examples

### 7.1 React Component

```jsx
import React, { useState, useEffect } from 'react';

function Counter() {
  const [count, setCount] = useState(0);

  useEffect(() => {
    document.title = `Count: ${count}`;
  }, [count]);

  return (
    <div className="counter">
      <h1>Count: {count}</h1>
      <button onClick={() => setCount(count + 1)}>
        Increment
      </button>
      <button onClick={() => setCount(count - 1)}>
        Decrement
      </button>
    </div>
  );
}

export default Counter;
```

### 7.2 Async/Await Example

```javascript
async function fetchUserData(userId) {
  try {
    const response = await fetch(`/api/users/${userId}`);

    if (!response.ok) {
      throw new Error(`HTTP error! status: ${response.status}`);
    }

    const data = await response.json();
    return data;
  } catch (error) {
    console.error('Error fetching user:', error);
    throw error;
  }
}

// Usage
fetchUserData(123)
  .then(user => console.log(user))
  .catch(error => console.error(error));
```

### 7.3 Long Line Code Test (Word Wrap)

```javascript
// This code block tests word wrapping with very long lines that exceed typical page width
const veryLongVariableName = "This is a very long string that demonstrates how the DOCX exporter handles lines that are longer than the typical page width and need to wrap to the next line automatically without breaking the layout or causing horizontal scrolling issues in the exported Word document";

const apiEndpoint = "https://api.example.com/v1/users/profile/detailed-information/with-preferences/and-settings/including-all-metadata?includeHistory=true&format=json&pretty=true&apiKey=super_long_api_key_that_should_wrap_to_next_line";

function processLongComplicatedDataStructureWithManyParameters(param1, param2, param3, param4, param5, param6, param7, param8, param9, param10, param11, param12) {
  return { param1, param2, param3, param4, param5, param6, param7, param8, param9, param10, param11, param12 };
}

// CSS example with very long selector
const cssRule = ".container .header .navigation .menu .item .link:hover:not(.disabled):not(.active) { background-color: rgba(255, 255, 255, 0.1); transition: all 0.3s ease-in-out; }";
```

### 7.4 Python Long Line Example

```python
# Python code with long lines
very_long_list_comprehension = [item.strip().lower().replace(" ", "_") for item in some_very_long_variable_name_that_contains_a_list_of_strings if len(item) > 10 and item.startswith("prefix_") and not item.endswith("_suffix")]

# Long string concatenation
error_message = f"An error occurred while processing the request: {error_type} - Details: {error_details} - Timestamp: {timestamp} - User: {user_id} - Session: {session_id} - Request ID: {request_id}"

# Long function call with many arguments
result = some_complex_function_with_many_parameters(argument1="value1", argument2="value2", argument3="value3", argument4="value4", argument5="value5", argument6="value6", argument7="value7", argument8="value8")
```

---

## 8. Math Equations (Phase 3 Preview)

Inline math: $E = mc^2$

Display math:

$$
\int_{a}^{b} f(x) dx = F(b) - F(a)
$$

*Note: Math equations currently render as plain text. Full OMML support coming in Phase 3.*

---

## 9. Performance Test

### Large Table

| ID | Name | Email | Department | Salary | Hire Date |
|----|------|-------|------------|--------|-----------|
| 001 | John Smith | <john@company.com> | Engineering | $95,000 | 2020-01-15 |
| 002 | Jane Doe | <jane@company.com> | Design | $85,000 | 2020-03-22 |
| 003 | Mike Johnson | <mike@company.com> | Marketing | $78,000 | 2021-06-10 |
| 004 | Sarah Williams | <sarah@company.com> | Sales | $92,000 | 2019-11-05 |
| 005 | Tom Brown | <tom@company.com> | Engineering | $98,000 | 2020-07-18 |

---

## 10. Edge Cases

### 10.1 Empty Code Block

```

```

### 10.2 Code Without Language

```
This is plain code without syntax highlighting.
It should still render properly with monospace font.
```

### 10.3 Single Cell Table

| Single Cell |
|-------------|
| Content     |

---

## Summary

This document tests:

✅ **Image Support**

- HTTP/HTTPS URLs
- Data URLs (base64)
- Image resizing

✅ **Syntax Highlighting**

- JavaScript/TypeScript
- Python
- HTML/CSS
- JSON
- SQL
- JSX/React

✅ **Enhanced Tables**

- Header row styling
- Cell padding
- Auto-fit layout
- Multiple column widths

✅ **Combined Features**

- Code in lists
- Tables with inline code
- Nested structures

---

**Test Date:** 2025-11-28  
**Version:** Phase 2 Implementation  
**Status:** Ready for Export  
