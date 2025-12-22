# Table of Contents (TOC) Sidebar Demo

> MarkView's Table of Contents (TOC) sidebar feature automatically extracts headings from your markdown files and provides a clickable navigation structure for easy access to different sections of your document.

## Introduction

The TOC sidebar should automatically extract all headings and create a clickable navigation structure.

### Purpose

Test various heading levels and nesting patterns.

### Expected Behavior

- Auto-generate TOC from h1-h6
- Clickable navigation
- Active section highlighting
- Smooth scrolling

## Feature Set

This section describes the features being tested.

### Auto-Extraction

The TOC should find all headings without manual configuration.

#### Implementation Details

Uses querySelector to find all h1-h6 elements.

##### Technical Notes

Headings without IDs get auto-generated IDs based on their text.

###### Deep Nesting Test

This is the deepest level (h6). TOC should handle this gracefully.

### Nested Structure

Headings should nest properly based on their level.

## Scroll Spy

As you scroll through this document, the TOC should highlight the current section.

### IntersectionObserver

Modern API for efficient scroll tracking.

## Navigation Controls

Test the control buttons.

### Expand/Collapse

- Click ⊞ to expand all
- Click ⊟ to collapse all

### Close Button

Click ✕ to hide the TOC sidebar.

## Edge Cases

Testing unusual scenarios.

### Non-Sequential Levels

What happens when we jump from h2 to h5?

##### Skipped h3 and h4

This should still work correctly.

### Special Characters in Headings

Headings with **bold**, *italic*, and `code` should work.

### Very Long Heading That Might Need To Be Truncated Because It Contains Too Much Text

The UI should handle long headings with ellipsis.

## Performance

Large documents with many headings.

### Section A

### Section B

### Section C

### Section D

### Section E

### Section F

### Section G

### Section H

### Section I

### Section J

All sections should render quickly.

## Dual Sidebar Test

When both folder browser (left) and TOC (right) are visible:

- Content should be centered
- Margins should adjust properly
- Both sidebars should work independently

## Theme Support

TOC should support both light and dark themes.

### Light Theme

Default appearance with light colors.

### Dark Theme

Switch theme in settings to test dark mode.

## Conclusion

If you can see this heading in the TOC and click it to navigate here, the feature works! ✅

### Final Notes

- All headings extracted
- Navigation works
- Scroll spy active
- Styling correct
- Performance good

Thank you for testing! 🎉
