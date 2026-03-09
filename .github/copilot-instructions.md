# AI Coding Agent Instructions: Random Color Generator

## Project Overview

This is a simple single-file HTML/JavaScript application that generates random hexadecimal color codes and displays them in the page background. The project is currently **incomplete** with syntax errors and ID mismatches.

## Known Issues to Fix

1. **HTML/JavaScript ID Mismatch**: 
   - HTML button has `id="btn-change-colour"`
   - JavaScript queries `document.getElementById('change-colour')` (missing "btn-" prefix)
   
2. **Incomplete JavaScript**: 
   - The for-loop in the color generation function is incomplete
   - Missing closing braces for the event listener callback

## Project Structure

```
index.html          # Single-file app with HTML markup and inline JavaScript
```

## Implementation Pattern

The color generator follows this pattern:
1. **Color Array Approach**: Uses an array of hex digits (0-F) to randomly build a 6-character hex color code
2. **Event-Driven**: Button click triggers the color generation
3. **DOM Updates**: Display the generated color code in a `<span>` element

Example completed function should:
- Generate 6 random hex digits
- Prepend '#' to create valid hex color code
- Update `<span id="box-colour">` with the color value
- Apply the color to the page background or element styling

## Conventions

- Use camelCase for JavaScript variables (`btnchangeColour`, `boxColour`)
- Prefix button references with clear intent (`btn-`, `box-`)
- Keep console-free: No logging or console output needed
- Vanilla JavaScript only: No frameworks or dependencies

## Common Tasks

**Fix and Complete the Code**:
- Fix the `getElementById()` selector to match HTML attributes
- Complete the for-loop: iterate 6 times, randomly select from `arrColours`
- Properly close all braces
- Test by clicking the button to verify color changes are visible

**Styling Enhancements** (if needed):
- Update `document.body.style.backgroundColor` to apply generated color
- Consider adding CSS for button styling or color display
