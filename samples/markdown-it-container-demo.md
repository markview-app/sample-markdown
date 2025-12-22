# Custom Containers (markdown-it-container)

> **MarkView** supports custom containers using the `markdown-it-container` plugin. You can create various types of containers such as info, warning, danger, details, and spoiler boxes.

## Info Container

::: info
This is an info container.
You can put any markdown content here.
:::

## Warning Container

::: warning
**Warning:** This is a warning message.
Be careful with this operation!
:::

## Danger Container

::: danger
**Danger Zone!**
This action cannot be undone.
:::

## Details Container

::: details
**Click to expand:**
This content is hidden by default.
You can toggle visibility.
:::

## Spoiler Container

::: spoiler
This contains spoilers for the movie!
The main character was the villain all along.
:::

## Container with Title

::: info Custom Title
This info box has a custom title.
The title appears at the top.
:::

::: danger Security Notice
Never share your API keys publicly!
Store them securely in environment variables.
:::

## Container with Markdown Content

::: warning Important Notice
This container supports **full markdown**:

- Bullet lists
- **Bold** and *italic* text
- `Code blocks`
- [Links](https://example.com)

```javascript
console.log("Even code blocks!");
```

:::
