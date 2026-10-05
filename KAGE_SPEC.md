# Alayendo Specification

## Project Overview

**Alayendo** is a cinematic, single-page WebGL experience inspired by Japanese temple architecture and night gardens. It presents a five-chapter night walk through a fictional Kyoto mountain temple, where the user scrolls through a live 3D scene rendered with Three.js. The experience feels like an editorial art book moving through a live 3D world, not a conventional product landing page.

### Vision

Create a deliberately small static site that combines procedural WebGL scenery with editorial layout, generated cinematic stills, and alpha-preserving foreground cutouts. The site should have no build step, no package manager, and no runtime network dependencies — everything runs from a single HTML file with vendored assets.

## Experience

- **Fixed full-viewport Three.js canvas** as the environmental layer
- **Five continuous chapters** driven by page scroll, each feeling like a new composed shot rather than a hard scene replacement
- **Procedural temple architecture**: temple, torii, stairs, lanterns, moon, terrain, trees, fog, rain, drifting leaves, embers, atmosphere
- **Restrained visual effects**: bloom, film grain, vignette, depth haze, warm shoji light, cold moonlight, large vermilion moon
- **Color palette**: near-black, blue-charcoal, warm amber, bone white, vermilion
- **No frameworks, build tooling, analytics, trackers, remote fonts, generic glassmorphism, or decorative motion without narrative purpose**

## Layout

The page structure consists of:

1. **Hero chapter** — initial establishing view with large heading and navigation
2. **Chapter I: The Gate** — garden gate with wall, pine, and grass foreground elements, the latest 5 videos.
3. **Chapter II: Pathways** — garden cards with lantern court, moonwater, and approach scenes, the videos based on the month of year 2026, 
4. **Chapter III: Sacred Craft** — curriculum/lessons section with basalt stones and wall fragments, album videos (long duration more than 20 minutes)
5. **Chapter IV: Eternity** — afterlight closing with hill, shrine ruins, and horizon, the videos based on the month of year 2025
6. **Chapter V: Year 2025** — Fall scene of US New York State,  closing with hill, shrine ruins, and horizon, the videos based on the month of year 2025
7. **Footer/Manifesto** — closing statement and navigation

### Typographic Scale

- **Display**: Uppercase, tight tracking, text shadow for depth
- **Headings**: Hierarchical sizes with clamp() responsiveness
- **Body**: 16px base, 1.6 line-height, subtle text shadow
- **CJK Japanese**: Noto JP font, used for display and labels
- **Numerals**: Tabular numerals for aligned numbers

### Section Scrims

Each chapter section has a radial gradient scrim that:
- Holds the chapter's "copy off the sanctuary"
- Inset edges never land as seams
- Masks top of chapter on entry, full strength by first line arrival

## Motion

- **Word-by-word heading reveal** with staggered transitions
- **Slow, precise section transitions** with eased camera interpolation
- **Subtle parallax** on foreground and background layers
- **Navigation, chapter rail, cards, and foreground layers** respond to active section
- **Reduced-motion behavior** preserves complete reading experience
- Custom cursor only for fine pointer devices

## Interaction

- **Anchor navigation** working across desktop and mobile
- **Responsive layouts** from 390×844 mobile to desktop
- **Semantic landmarks** and accessible labels
- **Mobile navigation** as slide-in sheet
- **Chapter rail** for section jumping
- **Focus-visible** states for keyboard navigation

## Assets

### Generated WebP Scene Plates

Each chapter has corresponding generated WebP plates stored in `secret-pathways-assets/generated/`:

| File | Chapter |
|------|---------|
| kage-approach.webp | Chapter II (approach) |
| kage-lantern-court.webp | Chapter II (lantern court) |
| kage-moonwater.webp | Chapter II (moonwater) |
| kage-sanmon-preview.webp | Hero (Sanmon gate preview) |

### Foreground PNG Cutouts

Alpha-preserving PNG cutouts stored in `secret-pathways-assets/foreground/png/`, placed per chapter via `data-fg` attributes:

| Chapter | Elements |
|---------|----------|
| I (gate) | wall, pine, grass |
| II (pathways) | sakura, leaves, lantern, bush |
| III (lessons) | wall, stones, grass |
| IV (eternity) | hill, ruins, grass, sakura |
| Foot (colophon) | bush, grass, stones |

### Image References (from SRC_BRIEF.md)

The following image files are referenced in the project:

- image.png, image-1.png through image-20.png (various project plates and plates)
- image-16.png, image-17.png

All 20 image files exist in the project directory.

## Build & Run

**No build step or environment variables required.** To run locally:

```bash
python3 -m http.server 4173 --bind 127.0.0.1
```

Then visit http://127.0.0.1:4173/.

Any equivalent static server will work. The site uses relative paths and works under a GitHub Pages repository subpath.

## Design and Attribution

- Cinematic scene plates and foreground artwork generated using GPT Image 2, then art-directed and composed with the live Three.js scene
- Vendored Three.js r149 build retains its MIT license notice and copyright attribution
- Kage is an original, independent design study inspired by Japanese temple architecture and night gardens
- Not affiliated with a specific temple, cultural institution, or tourism organization

## More Projects

- Complete Shelf — Three.js library of seven interactive clothbound hardcovers
- Sketchbook — page-flipping sketchbook of Singapore
- Agent Skills — reusable skill library including falling leaves and pointer trail techniques
