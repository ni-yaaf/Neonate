# NEONATE — 11:12

### Between Stars

A small interactive birthday experience made for **Neonate**.

**Created by:** Niyaaf
**Birthday:** December 11, 2026
**Type:** Personal interactive web experience

---

## About

**NEONATE — 11:12** is a quiet digital library floating through a nebula.

Instead of presenting a traditional birthday page, the experience lets one person wander through a collection of rooms containing stories, poems, photographs, a handwritten-style letter, hidden discoveries, and a constellation assembled piece by piece.

The experience is intentionally personal.

Nothing is generated to fill missing memories. Personal sections use explicit placeholders until the creator replaces them with real material.

> The library is warm because you are.
> The books are full because you've been paying attention.
> The stars are there because you put them there.

---

## Experience

The journey follows this path:

```text
Door
  ↓
Hall
  ├── Fiction Room
  ├── Poetry Room
  ├── Art Room
  └── Letter
          ↓
     Open When
          ↓
     Observatory
          ↓
      Final Scene
```

### The Door

The entrance to the library.

A wooden door waits in the darkness beneath the title:

**THE LIBRARY OF US**

### The Hall

The central room connecting the experience.

It contains:

* fireplace
* armchair
* lamp
* lectern
* bookshelves
* windows
* ceiling stars
* hidden interactions

### The Fiction Room

A room of books containing memories and stories.

Books can be pulled from the shelves and opened as full-page readers.

### The Poetry Room

A quieter room containing poems and things that were meant to be said.

Poems reveal themselves gradually, line by line.

### The Art Room

A visual archive containing photographs, screenshots, drawings, and small things worth keeping.

### The Letter

A ten-chapter letter addressed directly to Neonate.

The letter includes:

* chapter navigation
* handwritten margin notes
* constellation progress
* hidden discoveries
* eight **Open When** envelopes

### The Observatory

A hidden room that isn't immediately advertised.

Discovering it reveals:

* telescope interactions
* a twelve-entry journal
* additional stars
* a hidden final message

### The Final Scene

Once the experience has been explored, the armchair becomes available.

The ending moves away from menus and interfaces and becomes a quiet room containing only:

* fireplace
* window
* constellation
* paper star

The intention is simple:

**stay.**

---

## Star System

The library contains **40 star positions**.

Stars are earned by exploring the experience.

Possible sources include:

| Source                | Reward |
| --------------------- | -----: |
| Book                  |     +1 |
| Poem                  |     +1 |
| Artwork               |     +1 |
| Letter chapter        |     +1 |
| Open When envelope    |     +1 |
| Easter egg            |     +1 |
| Observatory discovery |     +5 |
| Journal entry         |     +1 |

The constellation develops as stars are discovered.

```text
5 stars   → The Beginning
12 stars  → The Middle
20 stars  → Your Thing
30 stars  → My Thing
40 stars  → Us
```

The final constellation becomes a paper-star shape.

---

## Easter Eggs

The experience contains 15 small discoveries.

They reward curiosity rather than announcing themselves.

Examples include:

* clicking the moon
* interacting with the fireplace
* turning on the lamp
* double-clicking a book spine
* returning a pulled book
* discovering the hidden poem
* clicking the telescope
* finding the letter's hidden star
* looking beneath the room
* waiting in the Hall
* discovering the shooting star

Some discoveries only make sense once the library has been explored.

---

## Design

The visual language is intentionally restrained.

### Atmosphere

* warm wood
* old paper
* candlelight
* fireplace glow
* deep nebula colours
* quiet gold highlights
* handwritten annotations
* soft shadows
* subtle film grain

### Typography

**Cormorant Garamond**
Used for titles, books, letters, and literary content.

**Inter**
Used for interface text and supporting information.

**Segoe Print / Bradley Hand / cursive**
Used for handwritten notes and discoveries.

### Core palette

```text
Wall        #1A1410
Shelf       #2B1F17
Ember       #D48A3A
Candle      #E8C87A
Paper       #E9E1D0
Ink         #2A2420
Nebula      #1A0F2E
            #0F1A2E
            #2A1A3E
Star        #F1EFE9
Star Gold   #D8C891
```

The guiding principle is:

> When in doubt, choose quieter, warmer, simpler.

---

## Technology

The project is intentionally lightweight.

### Stack

* React 18
* Vite 5
* Plain CSS
* React hooks
* localStorage
* CSS keyframe animations
* optional HTML5 audio
* Google Fonts

### No

* backend
* database
* authentication
* AI APIs
* analytics
* tracking
* heavy animation libraries
* large UI frameworks
* Tailwind
* unnecessary external APIs

The experience is designed to work as a static website.

---

## Project Structure

```text
neonate-birthday/
├── index.html
├── package.json
├── vite.config.js
├── public/
│   ├── favicon.svg
│   └── images/
│       ├── artifacts/
│       ├── textures/
│       └── nebula/
└── src/
    ├── main.jsx
    ├── App.jsx
    ├── content/
    ├── components/
    ├── screens/
    ├── systems/
    └── styles/
```

---

## Personal Content

Personal content belongs in the content files rather than inside the interface logic.

Examples:

```text
src/content/books.js
src/content/poems.js
src/content/art.js
src/content/letter.js
src/content/openWhen.js
src/content/observatory.js
src/content/easterEggs.js
src/content/stars.js
src/content/copy.js
```

Images belong in:

```text
public/images/artifacts/
public/images/textures/
public/images/nebula/
```

### Important

Do not replace placeholders with invented memories.

Every personal detail should come from the creator.

Placeholder content should remain visibly marked until replaced.

---

## Local Development

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Build for production:

```bash
npm run build
```

Preview the production build:

```bash
npm run preview
```

---

## Deployment

This project is designed to deploy directly to **Vercel**.

### Vercel + GitHub

1. Push the project to GitHub.
2. Open Vercel.
3. Choose **Add New → Project**.
4. Import the GitHub repository.
5. Let Vercel detect the Vite configuration.
6. Deploy.

No server or database configuration is required.

---

## Persistence

Exploration progress is stored locally in the visitor's browser.

The experience uses localStorage for:

```text
neonate:visited
neonate:readBooks
neonate:readPoems
neonate:viewedArt
neonate:readChapters
neonate:openedEnvelopes
neonate:stars
neonate:eggs
neonate:observatory
neonate:journalRead
neonate:finalUnlocked
```

This allows the recipient to leave and return without losing progress.

Refreshing the page after completing the final scene returns to the Door as intended.

---

## Accessibility

The experience is designed with accessibility in mind.

Supported features include:

* keyboard navigation
* visible focus states
* Escape-to-close interactions
* semantic buttons
* ARIA labels
* reduced-motion support
* readable paper-text contrast
* descriptive image alt text
* no autoplaying audio
* no flashing effects
* no interaction dependent only on colour

Interactive touch targets should remain suitable for iPad use.

---

## Responsive Targets

Primary design targets:

```text
Desktop
1440 × 900
1680 × 1050
1920 × 1080
2560 × 1440

iPad landscape
1366 × 1024

iPad portrait
1024 × 1366
```

The experience prioritizes desktop and iPad while remaining usable on smaller screens.

---

## Performance

The project aims to remain lightweight:

* small initial JavaScript bundle
* lazy-loaded artwork
* compressed images
* minimal JavaScript animation
* CSS-based transitions
* static star generation
* limited DOM depth
* no unnecessary libraries

Large artwork should be optimized before being added to the project.

---

## Build Philosophy

This is not meant to feel like a generic birthday website.

It should feel like something one person made slowly for another person.

That means:

**intimacy over features**
**meaning over spectacle**
**warmth over polish-for-polish's-sake**
**real memories over generated content**

The interface should never compete with the person it's made for.

---

## Creator

**Niyaaf**

Made for **Neonate**.

December 11, 2026.

> “Still here.”

---

## License

This project is a personal gift and is not intended as a commercial template or public product.

Please do not reuse private photographs, letters, memories, or other personal material contained in the project without permission.
