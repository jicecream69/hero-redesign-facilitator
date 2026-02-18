# Hero Redesign - facilitator.com

## What This Is
A prototype/mockup of a redesigned hero section for facilitator.com, meant to show a designer or developer what to build in Framer.

## Live URLs
- **Vercel**: https://hero-redesign-facilitator.vercel.app
- **GitHub**: https://github.com/jicecream69/hero-redesign-facilitator

## Current Design (latest iteration)
- **Dark mode** throughout (#0a0a0a background)
- **Nav sits outside the video** (not overlapping), dark theme with white text, "by AJ&Smart" yellow badge, generous padding (20px top, 56px sides, 28px bottom)
- **Video plays inside a rounded-corner container** (20px border-radius, 56px padding from page edges), Tony Robbins-style
- **Wistia video background** (ID: `ghi1nw7dk7`) from the EFM 2026 project, looping segment 00:24 to 00:39
- **Light gradient overlay** on the video (very subtle, about 35% max opacity at the bottom)
- **Hero text bottom-left**: headline + subtitle + two CTA buttons
- **Trust stats bottom-right**: three animated count-up numbers (35,000+ Facilitators Trained, 15 Years In Business, 25,582,830 YouTube Views) with dividers between them, weight 600, labels at 85% white
- **Staggered fade-in animations** on all content elements, count-up starts after fade-in completes

## Current Headline
"Facilitation? That's Us!" (with line break between "Facilitation?" and "That's Us!")

## Current Subtitle
"Workshop and facilitation training trusted by Google, LEGO, P&G, and 200+ companies worldwide."

## Current CTAs
- Primary (white pill): "Explore Programs"
- Secondary (glass outline): "Train My Team"

## Typography (aligned with EFM 2026 project)
- **Font**: Avenir Next LT Pro (falls back to Inter)
- **H1**: clamp(2.8rem, 6vw, 4.5rem), weight 900, line-height 1.1, letter-spacing -0.03em
- **Subtitle**: clamp(1.4rem, 2.8vw, 1.85rem), weight 500, line-height 1.4, pure white
- **Buttons**: 1rem (18px), weight 700
- **Labels**: 0.78rem, uppercase, 0.1em letter-spacing
- **Body weight**: 500 base
- **Font smoothing**: antialiased

## Previous Iterations Tried
1. Full-bleed video with white floating nav (rounded card), centered text
2. Full-bleed video with glass/transparent nav, bottom-left text
3. Various headlines: "The World's Best Facilitation Training", "Future-Proofed Facilitation Training", "Facilitation Training, but fun and future-proofed", "Modern Training for the Modern Facilitator", "Modern Facilitation Training"
4. YouTube embed (speaker-page video wT8Se9v-Ros) before switching to Wistia
5. Centered text layout vs bottom-left (landed on bottom-left)
6. Featured Program card for EFM on bottom-right (replaced with trust stats)
7. Yellow primary button (switched to white)
8. Yellow accents in featured card (removed, went tonal)
9. Heavy dark gradient overlay (reduced to ~35% max, user preferred lighter)
10. Caveat handwritten accent on keywords (removed, cleaner without)

## Key References
- **Speaker page** (`/Users/jonathancourtney/Desktop/Claude Code/speaker-page`): Original video hero inspiration, uses YouTube IFrame API with segment looping
- **EFM 2026** (`/Users/jonathancourtney/Desktop/Claude Code/EFM 2026`): Source of the Wistia video, typography system, and brand guidelines
- **SEO Facilitator.com** (`/Users/jonathancourtney/Desktop/Claude Code/SEO Facilitator.com`): Company positioning, messaging, and audience research used for subtitle copy
- **Tony Robbins** (tonyrobbins.com): Inspiration for dark mode + rounded video container + trust stats layout
- **Organic Basics**: Inspiration for floating white nav card (tried but moved away from)

## Tech
- Single HTML file, vanilla CSS/JS
- Wistia Player API for video embed + segment looping
- Count-up animation using requestAnimationFrame with cubic ease-out
- Google Fonts: Inter (UI) + Caveat (loaded but unused)
- Run with `python3 -m http.server 8090` from project directory
- Auto-deploys to Vercel on git push

## Nav Links (matching live facilitator.com)
Training Programs (dropdown), Corporate Training, Hire a Facilitator, Free Resources, About Us, Reviews, Get in Touch (outlined CTA)
