# Visual QA Prompt

```text
Start the local development server and inspect the UI in browser automation.

Required viewports:
- 1440x900
- 1024x768
- 390x844

Check:
- blank or broken rendering
- element overlap
- text clipping
- horizontal page scroll on mobile
- poor contrast
- inconsistent spacing
- awkward component sizing
- broken images or icons
- missing loading, empty, error, disabled, hover, active, and selected states

Fix all issues found, then rerun the same checks.

Return:
- inspected URLs
- screenshots or screenshot paths when available
- issues found
- fixes made
- remaining risks
```

