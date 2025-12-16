# GitHub-Style Alerts Test

This document tests all alert/callout types supported by MarkView.

---

## Alert Type: NOTE

> [!NOTE]
> Highlights information that users should take into account, even when skimming.

Example use case: Useful tips that improve understanding.

---

## Alert Type: TIP

> [!TIP]
> Optional information to help a user be more successful.

Example use case: Pro tips and best practices.

---

## Alert Type: IMPORTANT

> [!IMPORTANT]
> Crucial information necessary for users to succeed.

Example use case: Critical requirements or key concepts.

---

## Alert Type: WARNING

> [!WARNING]
> Critical content demanding immediate user attention due to potential risks.

Example use case: Deprecation notices or breaking changes.

---

## Alert Type: CAUTION

> [!CAUTION]
> Negative potential consequences of an action.

Example use case: Data loss warnings or dangerous operations.

---

## Multiple Alerts in Sequence

> [!NOTE]
> If you are looking for a list of MCP servers, you can browse published servers on [the MCP Registry](https://registry.modelcontextprotocol.io/). The repository served by this README is dedicated to housing just the small number of reference servers maintained by the MCP steering group.

> [!TIP]
> Use keyboard shortcuts to navigate faster:
>
> - `Ctrl+B` - Toggle sidebar
> - `Ctrl+Shift+T` - Toggle theme
> - `Ctrl+Shift+C` - Toggle centered layout

> [!IMPORTANT]
> **Breaking Changes in v2.0:**
>
> - Minimum Node.js version is now 16+
> - Old API endpoints have been removed
> - Configuration format has changed

> [!WARNING]
> ⚠️ This feature is experimental and may change in future releases.

> [!CAUTION]
> **Do not run this command in production!**
>
> Running `rm -rf /` will permanently delete all files on your system.

---

## Alerts with Rich Content

> [!NOTE]
>
> ### Nested Headings Work
>
> You can include various markdown elements:
>
> - Bullet lists
> - **Bold** and *italic* text
> - `Inline code`
> - [Links](https://example.com)
>
> ```javascript
> // Even code blocks!
> console.log('Hello from alert');
> ```

> [!IMPORTANT]
>
> 1. First step
> 2. Second step
> 3. Third step
>
> | Column 1 | Column 2 |
> |----------|----------|
> | Data 1   | Data 2   |

---

## Real-World Examples

### MCP Server Registry Notice

> [!IMPORTANT]
> If you are looking for a list of MCP servers, you can browse published servers on [the MCP Registry](https://registry.modelcontextprotocol.io/). The repository served by this README is dedicated to housing just the small number of reference servers maintained by the MCP steering group.

### Installation Warning

> [!WARNING]
> Before installing, ensure you have the following dependencies:
>
> - Node.js 16 or higher
> - pnpm 8 or higher
>
> Using npm or yarn is not supported and may cause issues.

### Security Notice

> [!CAUTION]
> **Never commit sensitive information to your repository!**
>
> This includes:
>
> - API keys
> - Passwords
> - Private keys
> - Personal access tokens
>
> Use environment variables or secret management tools instead.

### Feature Tip

> [!TIP]
> **Performance Optimization:**
>
> Enable caching for faster load times:
>
> ```bash
> npm run build --cache
> ```
>
> This can reduce build time by up to 70%!

---

## Edge Cases

### Empty Alert

> [!NOTE]

### Single Line Alert

> [!TIP]
> Quick tip!

### Very Long Alert

> [!IMPORTANT]
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
>
> Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt.
