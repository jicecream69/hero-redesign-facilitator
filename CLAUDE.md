# Hero Redesign - facilitator.com

## What This Is
A prototype/mockup of a redesigned hero section for facilitator.com, meant to show a designer or developer what to build in Framer.

## Current Design (latest iteration)
- **Dark mode** throughout (#0a0a0a background)
- **Nav sits outside the video** (not overlapping), dark theme with white text, "by AJ&Smart" yellow badge
- **Video plays inside a rounded-corner container** (20px border-radius, 20px padding from page edges), Tony Robbins-style
- **Wistia video background** (ID: `ghi1nw7dk7`) from the EFM 2026 project, looping segment 00:24 to 00:39
- **Dark gradient overlay** on the video (subtle top, heavy bottom) for text readability
- **Hero text bottom-left**: headline + subtitle + two CTA buttons
- **Featured Program card bottom-right**: glass-effect card for "Emergent Facilitation Mastery" with format/duration/pricing and a "Learn More" CTA with pulsing yellow dot
- **Staggered fade-in animations** on all content elements

## Current Headline
"Modern Training for the Modern Facilitator"

## Current CTAs
- Primary (yellow pill): "Explore Programs"
- Secondary (glass outline): "Train My Team"

## Current Subtitle
"Over the last 14 years, we've helped more than 35,000 people become world-class Facilitators."

## Previous Iterations Tried
1. Full-bleed video with white floating nav (rounded card), centered text
2. Full-bleed video with glass/transparent nav, bottom-left text
3. Various headlines: "The World's Best Facilitation Training", "Future-Proofed Facilitation Training", "Facilitation Training, but fun and future-proofed"
4. YouTube embed (speaker-page video wT8Se9v-Ros) before switching to Wistia
5. Centered text layout vs bottom-left (landed on bottom-left)
6. Stats section on bottom-right (removed in favor of Featured Program card)

## Key References
- **Speaker page** (`/Users/jonathancourtney/Desktop/Claude Code/speaker-page`): Original video hero inspiration, uses YouTube IFrame API with segment looping
- **EFM 2026** (`/Users/jonathancourtney/Desktop/Claude Code/EFM 2026`): Source of the Wistia video and Featured Program content (pricing, format, description)
- **Tony Robbins** (tonyrobbins.com): Inspiration for dark mode + rounded video container + "next event" card pattern
- **Organic Basics**: Inspiration for floating white nav card (tried but moved away from)

## Tech
- Single HTML file, vanilla CSS/JS
- Wistia Player API for video embed + segment looping
- Google Fonts: Inter (UI) + Caveat (accent, currently unused but loaded)
- Run with `python3 -m http.server 8090` from project directory

## Nav Links (matching live facilitator.com)
Training Programs (dropdown), Corporate Training, Hire a Facilitator, Free Resources, About Us, Reviews, Get in Touch (outlined CTA)
