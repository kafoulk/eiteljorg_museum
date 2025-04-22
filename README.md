# eiteljorg_museum | Field Trip Project

##  Project Summary

This project is a highly interactive, web-based experience based on the Eiteljorg Museum based in Indianapolis, Indiana, amnd is inspired by real exhibits and artifacts at said museum. The website presents a fictionalized digital museum where the user takes on the role of a time-traveling detective, solving clues connected to real historical objects. Through puzzles and exploration, users “unlock” additional content and insights about each artifact.

I chose this concept because it blends history, critical thinking, and immersive storytelling, encouraging meaningful engagement with museum-style content in a creative and gamified format. The project is inspired by online tours from institutions like the Louvre and the Smithsonian, but adds a narrative-driven twist to enhance interactivity and user immersion.

This experience aims to bridge art, history, and technology, creating a playful, story-based environment where each interaction deepens the user's understanding of the past and the significance of cultural artifacts.

## Core Webpages

**Home / Lobby Page**
  - Sets the scene with a mysterious message from the curator and an invitation to begin the investigation.
  - Interactive elements: subtle ambient sounds, animated intro text, and a “Begin Mystery” button.

**Virtual Museum Map**
  - A stylized, clickable floor plan of the Eiteljorg Museum.
  - Rooms to explore:
  - Native American Gallery
  - Western Art Gallery
  - Contemporary Native Art
  - Outdoor Sculpture Garden
  - Hovering reveals artifact previews; clicking enters themed exhibit areas.

**Exhibit Room Pages**
  - Exhibit Room Pages
    Each room features one highlighted artifact with interactive content. Example rooms:
    - Native American Gallery
    - Artifact: Traditional Lakota beadwork
    - Interaction: Solve a bead pattern puzzle to learn its meaning.
  - Western Art Gallery
    - Artifact: Cowboy gear from the 1800s
    - Interaction: Match objects to their historical purpose.
  - Contemporary Native Art
    - Artifact: Modern sculpture or painting
    - Interaction: Drag and rotate the piece to explore symbolic details.
  - Outdoor Sculpture Garden
    - Artifact: Bronze sculpture
    - Interaction: Hover or click to hear the story behind its creation.

**Clue Tracker / Journal**
  - A virtual journal logs clues the user discovers in each room.
  - Acts as both a progress tracker and learning summary, updated dynamically with each interaction.

## Design Choices & Examples

**Websites Referenced:**
- [Louvre Virtual Tour](https://www.louvre.fr/en/online-tours)
- [Smithsonian Natural History Tour](https://naturalhistory.si.edu/visit/virtual-tour)
- [Bruno Simon](https://bruno-simon.com) for UI playfulness and smooth transitions

**Color Palette:**
- Warm parchment (#f5f0e1) – backgrounds for readability
- Deep navy (#0a1a2f) – header/nav & immersive room backdrops
- Gold (#c9a449) – used to highlight clickable clues or solved riddles
- Brick red (#8b3a3a) – warnings, errors, or puzzle failures
- Soft green (#9ec39b) – progress indicators or correct answers

**Layout:**
- Fullscreen fixed-layout pages with dynamic movement elements (CSS transitions + JS triggers)
- Sticky inventory bar and interactive floor plan on scroll

**Data Structure:**
Artifacts and clues will be stored as JavaScript objects:
```js
const exhibits = [
  {
    id: "egypt-room",
    name: "Ancient Sarcophagus",
    clue: "I hold secrets of the afterlife.",
    image: "sarcophagus.jpg",
    unlocked: false,
    fact: "This artifact is from 1000 BC and reflects beliefs about death and rebirth."
  },
  // more artifacts...
];
