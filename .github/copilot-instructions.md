# Copilot Instructions: Koyribu Website

## Purpose
This repository contains a simple static website for the family cabin Koyribu. The assistant should improve the site while keeping it simple, maintainable, and visually professional.

## Project Context

- Content lives in `en/` and `nn/`
- Shared layout and styling live in `_layouts/default.html`
- Images live in `img/`
- The site should remain a simple static HTML/CSS solution

## Priorities

1. Make the site feel welcoming, trustworthy, and easy to use
2. Keep guest information easy to find and easy to scan
3. Preserve a simple technical structure
4. Maintain a strong mobile experience
5. Keep accessibility and HTML quality solid

## Language

- English is the primary language
- Nynorsk must also be supported
- Keep both languages aligned when practical
- If a task touches only one language, avoid unnecessary parallel edits unless requested

## Design Direction

The site should feel warm, calm, light, summer-oriented, and distinctly Norwegian without becoming generic or over-designed.

Use [Designsystemet](https://designsystemet.no/no/fundamentals/) for design principles only. Follow its approach to hierarchy, spacing, clarity, contrast, and accessibility.

## Technical Rules

- Prefer HTML and CSS over JavaScript
- Avoid unnecessary frameworks or build complexity
- Keep styling shared and centralized where practical
- Prefer small reusable utilities over repeated inline styling
- Make sure the structure can grow, including adding more images later

## Content Guidance

- Main page types should usually be Home, Cabin, Guest Info, Activities or Summer Guide, and Hikes
- Guest info pages should read like clear reference pages, not marketing pages
- Home and cabin pages can feel more editorial and inviting
- Keep content skimmable and reduce clutter and repetition
- Suggest clearer wording when the current text feels awkward or overly literal

## Accessibility

- Use semantic HTML
- Keep heading hierarchy clear
- Ensure sufficient contrast
- Provide visible focus states
- Use descriptive alt text
- Do not rely on color alone
- Keep content easy to read on mobile and desktop

## Working Style

- Prioritize structure before polish when both are in flux
- Prefer small, understandable improvements over large rewrites
- Keep the technical solution easy to maintain

## Testing And Delivery

- Test visual changes in a browser before considering the task complete
- Check readability, spacing, hierarchy, navigation state, and overall page coherence
- If browser screenshots fail, verify as much as possible another way and explain the limitation clearly
- When finishing a task, usually update the relevant Markdown, HTML, or CSS, keep styles centralized, explain key decisions briefly, and verify links and rendered appearance

## Avoid

- Introducing unnecessary JavaScript
- Overengineering the architecture
- Duplicating presentation rules across many Markdown files
- Making the site feel like a public-sector template instead of a warm cabin site
