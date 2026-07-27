# AGENTS.md

This repository contains a static web page NMDC team members use to display messages during outages
and other special events. The web page fetches a Markdown file, uses Showdown to convert its content
into HTML, and renders it within the web page.

## Dependencies

- Bootstrap 5 (loaded via CDN)
- Google Fonts (for the `Arimo` font)
- [Showdown](https://github.com/showdownjs/showdown) (to convert Markdown into HTML)

## Commands

- Preview website locally: `$ uvx reloadserver` and visit [localhost:8000](http://localhost:8000)

## Commonly-edited files

- `index.css` - styles applied to `index.html`
- `index.html` - web page (loads CSS, loads third-party JavaScript, and contains custom JavaScript)
- `message.md` - Markdown content that gets converted into HTML and injected into the web page
