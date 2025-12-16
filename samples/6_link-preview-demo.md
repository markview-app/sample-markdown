# External Link Preview Test

This document tests the new External Link Preview feature.

## Test Cases

### 1. Popular Websites

Hover over these links to see preview cards:

- [GitHub](https://github.com) - Code hosting platform
- [Stack Overflow](https://stackoverflow.com) - Q&A for developers
- [MDN Web Docs](https://developer.mozilla.org) - Web development documentation
- [Wikipedia](https://en.wikipedia.org) - Free encyclopedia

### 2. Tech Blogs

- [CSS-Tricks](https://css-tricks.com) - Web design and development blog
- [Smashing Magazine](https://www.smashingmagazine.com) - Design and development magazine
- [Dev.to](https://dev.to) - Developer community

### 3. News Sites

- [TechCrunch](https://techcrunch.com) - Technology news
- [The Verge](https://www.theverge.com) - Technology and culture news
- [Hacker News](https://news.ycombinator.com) - Tech news aggregator

### 4. Social Media

- [Twitter](https://twitter.com) - Social networking
- [Reddit](https://www.reddit.com) - Social news aggregation
- [LinkedIn](https://www.linkedin.com) - Professional networking

### 5. Edge Cases

#### Near Viewport Edges

Try hovering near the edges of the viewport to test positioning:

- Top edge: [OpenAI](https://openai.com)
- Right edge: [Google](https://www.google.com)
- Bottom edge: [Microsoft](https://www.microsoft.com)

#### Long URLs

- [This is a very long link with lots of text before it to test horizontal positioning](https://www.example.com)

#### Multiple Links in Paragraph

Test quick hover transitions: [Link 1](https://example1.com) and [Link 2](https://example2.com) and [Link 3](https://example3.com)

### 6. Internal Links (Should NOT Show Preview)

These are internal links and should not trigger preview:

- [Overview Test](./0_overview-test.md)
- [TOC Test](./1_toc-test.md)
- [Image Test](./2_internal-images-test.md)

### 7. Cache Test

Hover over these links, then hover again after 2 seconds. The second hover should be instant:

- [Cache Test 1](https://github.com)
- [Cache Test 2](https://stackoverflow.com)
