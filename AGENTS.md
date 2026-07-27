# AGENTS.md

This repository contains a static web page NMDC team members use to display messages during outages
and other special events. The web page fetches a Markdown file, uses Showdown to convert its content
into HTML, and renders it within the web page. The web page gets deployed to GitHub Pages.

## Dependencies

- [Bootstrap 5](https://getbootstrap.com/docs/5.2/) (frontend framework), fetched from a CDN
- [Google Fonts](https://fonts.google.com/specimen/Arimo) (for the `Arimo` font)
- [Showdown](https://github.com/showdownjs/showdown) (to convert Markdown into HTML)
- (Optional) [uv](https://docs.astral.sh/uv/) (for previewing the web page locally)

## Commands

- Preview web page locally: `$ uvx reloadserver` and visit [localhost:8000](http://localhost:8000)

## Commonly-edited files

- `index.css` - Styles applied to `index.html`
- `index.html` - Web page (loads CSS, loads third-party JavaScript, and contains custom JavaScript)
- `message.md` - Markdown content that gets converted into HTML and injected into the web page
