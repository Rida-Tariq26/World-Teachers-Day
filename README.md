# World Teachers' Day Tribute Card

A single-file, mobile-first, interactive digital tribute created by the students of Y-5 (GIRLS), Punjab College - Al-Rehman Garden Campus, honoring their teachers for World Teachers' Day (October 5).

## Overview

This project is a lightweight, responsive HTML/CSS/JS application designed without external frameworks, backend requirements, or heavy asset dependencies. It is completely offline-friendly and can be deployed directly to Netlify or GitHub Pages as a single index.html file.

## Class Identity

- Class: Y-5 (GIRLS)
- Institution: Punjab College - Al-Rehman Garden Campus
- Event: World Teachers' Day (October 5)

## Experience Flow

1. Gate Screen
   - Features an opening gate screen displaying the class and campus identity.
   - Allows entering a teacher's name to personalize the greeting.
   - Automatically pre-fills the name if passed in the URL query string (for example, `?to=Name`).
   - Uses textContent for rendering user input to prevent XSS vulnerabilities.

2. Opening Transition & Confetti
   - Upon clicking "Open Card", a lightweight, pure JavaScript canvas confetti particle burst is triggered.
   - Respects the prefers-reduced-motion media query for accessibility.

3. Personalized Greeting
   - Displays a custom salutation ("Dear Prof. [Name]," or fallback "Dear Teacher,").
   - Features an original opening message focusing on intellectual growth and mentorship beyond textbook lectures.

4. Five Interactive 3D Flip Cards
   - Uses CSS 3D transforms (`preserve-3d`, `rotateY(180deg)`) for smooth card flips.
   - Accessible via keyboard (Tab navigation, Space/Enter to flip) with visible focus rings and ARIA attributes.
   - Card 1: Intellectual Rigor (Beyond Memorization)
   - Card 2: Voice & Confidence (The Room to Ask)
   - Card 3: Correction with Dignity (Firmness with Grace)
   - Card 4: Professional Demeanor (The Unseen Habit)
   - Card 5: Enduring Legacy (What Stays Behind)

5. Closing & Signature
   - Displays a collective closing thought from Y-5 (GIRLS).
   - Features the student signature and campus footer.

## Copy Structure

All editable copy is organized in a single `copy` JavaScript object within index.html:

```javascript
const copy = {
  gate: { ... },
  greeting: { ... },
  cards: [ ... ],
  closing: { ... }
};
```

Alternative copy options are included as inline JavaScript comments for easy modification.

## Design System & Brand Palette

- Primary Navy: #1B2A6B
- Deep Navy: #0F1A44
- Accent Red: #E31E24
- Soft Sky Blue: #60A5FA
- White: #FFFFFF
- Headlines: Montserrat (Google Fonts)
- Body: Poppins (Google Fonts)
- Script Accent: Great Vibes (Google Fonts)

## Deployment

Simply host index.html on Netlify, GitHub Pages, or any static file host.
