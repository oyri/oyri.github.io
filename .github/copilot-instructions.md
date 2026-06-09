# Copilot Instructions: Koyribu Website

## Purpose
This repository contains a simple static website for the family cabin Koyribu. The assistant should improve the site while keeping it simple, maintainable, and visually professional.

## Project Overview

**Important context:** See [OPPDRAG-HYTTENETTSIDE.md](../../OPPDRAG-HYTTENETTSIDE.md) for strategic goals and target audience, and [ARBEIDSLOGG-HYTTENETTSIDE.md](../../ARBEIDSLOGG-HYTTENETTSIDE.md) for completed work and next steps.

**Tech stack:** Jekyll static site generator with plain HTML/CSS (no JavaScript frameworks).

## Project Context

- Content lives in `en/` and `nn/` directories (five main pages per language: index, cabin, guest-info, activities, hikes)
- Shared layout and styling live in `_layouts/default.html` (all CSS is inline to keep the site portable)
- Images live in `img/`
- The site should remain a simple static HTML/CSS solution
- This site is deployed as a GitHub Pages site

## Priorities

1. Make the site feel welcoming, trustworthy, and easy to use
2. Keep guest information easy to find and easy to scan
3. Preserve a simple technical structure
4. Maintain a strong mobile experience
5. Keep accessibility and HTML quality solid

## Site Structure

The website has five main pages per language:

- **Home (index.md)** – Landing page with cabin overview, key features, booking link, and summer activities preview
- **Cabin (cabin.md)** – Detailed presentation of the cabin: sleeping arrangements, facilities, location, and suitability for different visit types
- **Guest Info (guest-info.md)** – Practical reference for guests: check-in, check-out, house rules, utilities, equipment, emergency contact
- **Activities (activities.md)** – Summer activities and local recommendations: hikes, swimming, fishing, family activities
- **Hikes (hikes.md)** – Detailed hiking guides and mountain tips specific to the area

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
- Keep styling shared and centralized where practical (all CSS lives in `_layouts/default.html`)
- Prefer small reusable utilities over repeated inline styling
- Make sure the structure can grow, including adding more images later
- CSS variables (`--bg`, `--link`, `--text`, etc.) are defined in `:root` and reused throughout for consistent theming
- Use Liquid templating variables (e.g., `{{ page.lang }}`, `{{ page.title }}`) for dynamic content like page language and title
- All markdown files must include frontmatter with `lang` and `title` so the layout can render them correctly

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
- **How to preview locally:** This is a Jekyll site hosted on GitHub Pages. The easiest preview method is to commit changes to a test branch and view them at `https://oyri.github.io/oyri.github.io/` (or open the built HTML in a browser if you have Jekyll installed locally)
- Check readability, spacing, hierarchy, navigation state, and overall page coherence
- If browser screenshots fail, verify as much as possible another way and explain the limitation clearly
- When finishing a task, usually update the relevant Markdown, HTML, or CSS, keep styles centralized, explain key decisions briefly, and verify links and rendered appearance
- For language-paired changes: always update both `en/` and `nn/` files to keep structure aligned (unless explicitly told to update one language only)

## Avoid

- Introducing unnecessary JavaScript
- Overengineering the architecture
- Duplicating presentation rules across many Markdown files
- Making the site feel like a public-sector template instead of a warm cabin site
