# MJC Child Development Club - Project Guide

## Project Overview
Marketing materials for the MJC Child Development Club. HTML documents designed for browser Print-to-PDF (8.5x11" letter) plus a live website.

## Style Guide

### Colors
- **Primary accent**: Baby blue `#85C1E9` — used for borders, headings, highlights
- **Primary accent (darker, for text)**: `#5DADE2` — used for CTA text and bold callouts
- **Primary accent (light bg)**: `#F0F7FC` — used for highlighted chip/card backgrounds
- **Secondary accents** (use sparingly for variety):
  - Soft green: `#7EC8A0` / bg `#F0FFF5`
  - Soft blue: `#5DADE2` / bg `#F0F9FF`
  - Lavender: `#B07CC6` / bg `#FAF5FF`
  - Soft pink: `#E88DB6` / bg `#FFF0F6`
  - Coral: `#E85D75`
- **Text**: `#333` primary, `#666` secondary, `#777` muted, `#999` very muted
- **Borders**: `#eee` default, accent color for emphasis
- **Backgrounds**: `#fff` primary, `#FAFAFA` subtle sections

### Colors to AVOID
- **No yellow or gold** — looks jarring on screen
- **No dark navy backgrounds** — too heavy, wastes ink when printed
- **No dark header/footer bars** — keep everything light and airy

### Typography
- Font: `'Segoe UI', Tahoma, Geneva, Verdana, sans-serif`
- Headings: weight 700-800, color `#333`
- Accent headings (section titles): use `#85C1E9`
- Body text: 12.5-14px, color `#666`

### Mascot Usage
- **Male pirate** (`MalePirateMJC.png`): always LEFT side
- **Female pirate** (`FemalePirateMJC.png`): always RIGHT side
- When only one mascot is needed, use the **female pirate** on the right
- Mascots should be prominent — they are the brand identity
- Flyer sizes: 80-180px depending on placement (headers ~120px, body ~170px, footers ~80-120px)
- Images are transparent PNGs, located in `assets/images/`

### Layout Principles
- White backgrounds — these get printed, save ink
- Light borders (`2px solid #eee`) for card containers
- Accent-colored borders (`2px solid #85C1E9`) for emphasis boxes
- Dashed borders (`2px dashed #85C1E9`) for CTA sections
- Border-radius: 12-14px for cards, 20px for chips/pills
- Generous padding, clean whitespace

### Print Flyer Template
- Size: `8.5in x 11in` (letter)
- `@page { size: letter; margin: 0; }`
- `overflow: hidden` on body
- Footer: `position: absolute; bottom: 0;` with top border separator
- Always include `@media print` with `-webkit-print-color-adjust: exact`

## File Structure
```
assets/images/
  FemalePirateMJC.png    — Female pirate mascot (RIGHT side)
  MalePirateMJC.png      — Male pirate mascot (LEFT side)
  combined footer.png     — Both mascots side-by-side
  MalePirateMJCFinal.png — Older version, do not use
flyers/
  ece-cd-flowchart.html  — 4-step ECE/CD major pathway
  club-info.html         — Club recruitment flyer (STYLE REFERENCE)
  multicultural-day.html — March 13 event flyer
website/
  index.html             — Club website (responsive)
```

## Club Info
- **Name**: MJC Child Development Club
- **School**: Modesto Junior College
- **Meetings**: 1st & 3rd Fridays at 12:00 PM
- **Location**: John Muir Hall 160, West Campus
- **Spring 2026 dates**: Feb 6, Feb 20, Mar 6, Mar 20, Apr 3, Apr 17
- **Affiliations**: Office of Student Services, Associated Students

## Workflow
1. Edit HTML files directly
2. Open in browser to preview
3. For flyers: File > Print > Save as PDF for clean output
4. Website is self-contained HTML meant to be hosted
