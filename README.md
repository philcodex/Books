# Ebooks & Audiobooks

A simple, self-hosted web page for sharing ebooks and audiobooks — built for easy reading and downloading on both desktop and mobile.

## Overview

This project provides a clean, accessible page listing books available for download in ebook (`.epub`, `.m4b`) and audiobook (`.zip`, `.m4b`) formats. It was put together to share a personal reading list focused on parenting, child development, and free speech.

## Features

- **Responsive design** — desktop shows a clean table layout; mobile (under 640px) switches to full-width card-based layout with large, thumb-friendly download buttons
- **Separate author column** — title and author clearly separated for easy scanning
- **Bordered download buttons** — ebook and audiobook links styled as distinct buttons
- **Android audiobook guide** — companion page with step-by-step instructions for downloading and playing audiobooks on Android using Smart Audiobook Player
- **Analytics** — Google Analytics and Statcounter tracking included

## Files

| File | Description |
|---|---|
| `index.html` | Main book listing page |
| `audiobook-androidguide.html` | Step-by-step Android audiobook setup guide |

## Books Included

| Title | Author |
|---|---|
| The Montessori Baby | Simone Davies & Junnifa Uzodike |
| The Coddling of the American Mind | Greg Lukianoff & Jonathan Haidt |
| Bad Therapy: Why the Kids Aren't Growing Up | Abigail Shrier |
| Time to Think | Hannah Barnes |
| The New Puritans | Andrew Doyle |
| Hags | Victoria Smith |
| Free Speech and Why It Matters | Andrew Doyle |
| Woke Racism | John McWhorter |

## File Structure

```
/
├── index.html
├── audiobook-androidguide.html
├── MontessoriBaby.epub
├── TheMontessoriBaby.m4b
├── TheCoddlingoftheAmericanMind.epub
├── TheCoddlingoftheAmericanMind.zip
├── Abigail-Shrier-BadTherapy.epub
├── Abigail-Shrier-BadTherapy-Audiobook.m4b
├── HannahBarnes-TimeToThink.epub
├── HannahBarnes-TimetoThink.zip
├── AndrewDoyle-TheNewPuritans.epub
├── AndrewDoyle-TheNewPuritans.zip
├── VictoriaSmith-Hags.epub
├── VictoriaSmith-Hags.zip
├── AndrewDoyle-FreeSpeech.epub
├── AndrewDoyle-FreeSpeech.zip
├── JohnMcWhorter-WokeRacism.epub
└── JohnMcWhorter-WokeRacism.zip
```

## Deployment

This is a static HTML project — no build step or dependencies required. Drop the files onto any web server or static hosting provider (e.g. Apache, Nginx, GitHub Pages, Netlify).

Ensure all book files are placed in the same directory as `index.html` so the download links resolve correctly.

## Adding a New Book

1. Add the ebook and/or audiobook file to the server directory
2. Add a new `<tr>` row to the `<tbody>` in `index.html`:

```html
<tr>
  <td>Book Title</td>
  <td>Author Name</td>
  <td><a href="filename.epub" target="_blank">Download Ebook</a></td>
  <td><a href="filename.zip" target="_blank">Download Audiobook</a></td>
</tr>
```

## Analytics

The page includes:
- **Google Analytics** (`REMOVED`)
- **Statcounter** (project `REMOVED`)

To use your own analytics, replace the tracking IDs in `index.html`.