# Sprout Design System

A comprehensive design specification for the Sprout AI assistant interface. This document serves as the single source of truth for all visual design decisions and can be referenced across projects.

---

## 1. Color Palette

### Neutral / Slate (Warm Brown-Grey)

| Token | Hex | Usage |
|---|---|---|
| `--slate-950` | `#1C2A1F` | Sidebar background, app shell |
| `--slate-900` | `#3E2723` | Primary text, strong foreground |
| `--slate-800` | `#4E342E` | Heavy UI elements |
| `--slate-700` | `#5D4037` | Secondary text, hover states |
| `--slate-600` | `#6D4C41` | Muted foreground, avatars |
| `--slate-500` | `#737373` | Tertiary text, icons, labels |
| `--slate-400` | `#A1887F` | Placeholder text, disabled icons |
| `--slate-300` | `#BCAAA4` | Subtle borders, sidebar hover text |
| `--slate-200` | `#E0D6C9` | Borders, dividers |
| `--slate-100` | `#EFEBE9` | Light borders, separator lines |
| `--slate-50` | `#F5F0EB` | Hover backgrounds, subtle fills |

### Sage / Green (Brand Accent)

| Token | Hex | Usage |
|---|---|---|
| `--sage-600` | `#2E7D33` | Active badges, deep accent |
| `--sage-500` | `#34D25C` | Primary accent, logo gradient, active toggles |
| `--sage-400` | `#4CAF52` | Secondary accent, focus rings |
| `--sage-100` | `#C8E6CA` | Light accent backgrounds |
| `--sage-50` | `#E8F5E9` | Chip backgrounds, subtle accent fills |

### Gold

| Token | Hex | Usage |
|---|---|---|
| `--gold-500` | `#B8941F` | Star ratings, highlights |
| `--gold-400` | `#D4AD2E` | Gold accent elements |
| `--gold-100` | `#FDF8E8` | Gold tinted backgrounds |

### Red

| Token | Hex | Usage |
|---|---|---|
| `--red-500` | `#AA0008` | Error states, destructive actions, recording indicator |
| `--red-100` | `#FFEBEE` | Error backgrounds |

### Surface Colors

| Token | Hex | Usage |
|---|---|---|
| `--white` | `#FFFFFF` | Card backgrounds, input backgrounds |
| `--warm-white` | `#FAF6F2` | Main content area background |

---

## 2. Typography

### Font Families

| Token | Stack | Usage |
|---|---|---|
| `--font-body` | `'Inter', -apple-system, sans-serif` | All body text, UI labels, inputs |
| `--font-display` | `'Newsreader', Georgia, serif` | Headings, greeting text, brand name |

**Google Fonts import:**
```
Inter: 300, 400, 500, 600 (with italic 300, 400)
Newsreader: 300, 400, 500 (with italic 300, 400)
```

### Type Scale

| Category | Size | Usage |
|---|---|---|
| **Display** | `2.4rem` | Hero headings |
| **H1** | `1.8rem` | Page titles |
| **H2** | `1.5rem` - `1.6rem` | Section titles |
| **H3** | `1.2rem` - `1.4rem` | Card titles, modal headings |
| **H4** | `1.05rem` - `1.15rem` | Subsection titles |
| **Body Large** | `0.95rem` - `1rem` | Primary body text, inputs |
| **Body** | `0.88rem` - `0.92rem` | Standard body text |
| **Body Small** | `0.82rem` - `0.85rem` | Secondary text, nav items |
| **Caption** | `0.75rem` - `0.8rem` | Timestamps, metadata, menu items |
| **Micro** | `0.68rem` - `0.72rem` | Badges, toggle labels, tiny labels |
| **Nano** | `0.6rem` - `0.65rem` | Uppercase labels, category tags |

### Font Weights

| Weight | Name | Usage |
|---|---|---|
| `300` | Light | Placeholder text, input text, secondary body |
| `400` | Regular | Standard body text, nav items, menu items |
| `500` | Medium | Headings, active states, emphasis, brand name |
| `600` | Semi-bold | Strong emphasis, button text |

### Letter Spacing

| Value | Usage |
|---|---|
| `-0.03em` | Display headings |
| `-0.02em` | Large headings |
| `-0.01em` | Brand name, medium headings |
| `0.02em` | Slight emphasis |
| `0.04em` | Uppercase small labels |
| `0.06em` - `0.08em` | Section labels, uppercase text |

### Line Heights

| Value | Usage |
|---|---|
| `1` - `1.2` | Single-line elements, compact labels |
| `1.3` - `1.4` | Headings, card titles |
| `1.5` - `1.6` | Body text, inputs, messages |
| `1.65` - `1.75` | Long-form reading content |

---

## 3. Spacing

A 4px base unit scale:

| Token | Value | Usage |
|---|---|---|
| `--space-1` | `4px` | Micro gaps, tight padding |
| `--space-2` | `8px` | Small gaps, inline spacing |
| `--space-3` | `12px` | Standard gaps, icon padding |
| `--space-4` | `16px` | Component padding, section gaps |
| `--space-5` | `20px` | Generous padding |
| `--space-6` | `24px` | Card padding, section spacing |
| `--space-8` | `32px` | Large section spacing |
| `--space-10` | `40px` | Page-level spacing |
| `--space-12` | `48px` | Hero spacing |
| `--space-16` | `64px` | Major layout spacing |

---

## 4. Shadows

All shadows use warm brown tones (`rgba(62, 39, 35, ...)`) to match the earthy palette:

| Token | Value | Usage |
|---|---|---|
| `--shadow-sm` | `0 1px 2px rgba(62,39,35,0.04)` | Subtle depth, buttons |
| `--shadow-md` | `0 2px 8px rgba(62,39,35,0.06), 0 1px 2px rgba(62,39,35,0.04)` | Cards, inputs |
| `--shadow-lg` | `0 8px 24px rgba(62,39,35,0.08), 0 2px 8px rgba(62,39,35,0.04)` | Elevated cards, focused inputs |
| `--shadow-xl` | `0 16px 48px rgba(62,39,35,0.1), 0 4px 12px rgba(62,39,35,0.05)` | Modals, overlays |

**Special shadows:**
- Dropdown menus: `0 8px 32px rgba(0,0,0,0.12), 0 2px 8px rgba(0,0,0,0.08)`
- Focus ring: `0 0 0 3px rgba(46,125,51,0.12)` (sage-tinted)

---

## 5. Border Radius

| Value | Usage |
|---|---|
| `4px` | Tiny elements, code blocks |
| `6px` | Chips, small badges, sidebar collapse button |
| `8px` | **Primary radius** — buttons, inputs, nav items, toggles, tags |
| `10px` | Medium buttons, sidebar thread |
| `12px` | Cards, vault cards, agent cards, modals |
| `14px` - `16px` | Large cards, input boxes, dialog boxes |
| `18px` - `20px` | Feature cards, large modals |
| `50%` | Avatars, circular badges |

**Asymmetrical patterns:**
- Main content panel: `12px 0 0 12px` (rounds left side only)
- Input textarea: `16px 16px 0 0` (rounds top only)
- Chat bubbles: `16px 16px 4px 16px` / `16px 4px 16px 16px` (tail corner)

---

## 6. Motion & Transitions

### Easing Curves

| Token | Value | Usage |
|---|---|---|
| `--ease-out` | `cubic-bezier(0.16, 1, 0.3, 1)` | Primary easing — entrances, interactions |
| `--ease-in-out` | `cubic-bezier(0.65, 0, 0.35, 1)` | Symmetric transitions |

### Durations

| Token | Value | Usage |
|---|---|---|
| `--duration-fast` | `150ms` | Hover states, toggles, micro-interactions |
| `--duration-normal` | `250ms` | Standard transitions, panel slides |
| `--duration-slow` | `400ms` | Large reveals, complex animations |

### Animation Library

| Name | Effect | Duration | Usage |
|---|---|---|---|
| `fadeIn` | Opacity 0 to 1 | 0.6s | App shell entrance |
| `homeIn` | Fade + translate Y 16px | 0.6s | Home view entrance |
| `messageIn` | Fade + translate Y 12px | 0.3s | Chat message entrance |
| `chipIn` | Fade + scale 0.9 to 1 | 0.2s | Input chip addition |
| `panelSlideIn` | Translate X 100% to 0 | 0.35s | Side panel reveal |
| `slideUp` | Fade + translate Y 20px | 0.3s | Bottom-up content reveal |
| `modalFadeIn` | Opacity 0 to 1 | 0.25s | Modal overlay |
| `modalSlideUp` | Fade + scale 0.97 + translate Y 20px | 0.3s | Modal dialog |
| `userMenuSlideUp` | Fade + translate Y 8px | 0.2s | Menu popover |
| `projCardIn` | Fade + translate Y 10px | 0.3s | Project card stagger |
| `spin` | Rotate 360deg | 0.8s linear | Loading spinners |
| `voicePulse` | Scale 1 to 1.15 | 1.2s | Voice recording indicator |
| `conicSweep` | Conic gradient rotation | 2s linear | Voice input border sweep |

---

## 7. Z-Index Scale

| Value | Layer | Usage |
|---|---|---|
| `-1` | Background | Decorative pseudo-elements |
| `0` | Base | Default layer |
| `1` - `3` | Stacked | Overlapping file icons |
| `10` | Elevated | Content overlays |
| `100` | Floating | Sidebar expand button, persistent UI |
| `200` - `210` | Dropdown | Tooltips, popovers |
| `1000` | Modal | Modals, overlays, dropdown menus |
| `1100` | Top | High-priority modals |

---

## 8. Layout Patterns

### App Shell

```
.app (flex row, 100vh)
  .sidebar (260px fixed width)
  .main (flex: 1, warm-white background, 12px left radius)
```

### Sidebar

- Width: `260px`
- Background: `--slate-950`
- Border: `1px solid rgba(255,255,255,0.06)`
- Collapsible with smooth transition
- Structure: header > nav > footer

### Content Areas

- Max-width for centered content: `640px` (home), `900px` (projects), `1200px` (explore)
- Standard padding: `var(--space-6)` to `var(--space-8)`

### Responsive Grid

- Projects grid: `repeat(auto-fill, minmax(300px, 1fr))`
- Knowledge base grid: `repeat(auto-fill, minmax(260px, 1fr))`
- Explore agents grid: `repeat(auto-fill, minmax(260px, 1fr))`

---

## 9. Component Specifications

### Cards

```css
background: var(--white);
border: 1px solid var(--slate-100);
border-radius: 12px;
padding: var(--space-5) to var(--space-6);
transition: all var(--duration-fast) var(--ease-out);
```

Hover: `border-color: var(--sage-400); box-shadow: var(--shadow-md);` or `transform: translateY(-2px)`

### Buttons

**Primary (dark):**
```css
background: var(--slate-900);
color: var(--white);
border-radius: 8px;
padding: var(--space-2) var(--space-5);
font-size: 0.85rem;
font-weight: 500;
```

**Ghost/icon button:**
```css
background: none;
border: none;
width: 30px; height: 30px;
border-radius: 8px;
color: var(--slate-400);
```
Hover: `background: var(--slate-50); color: var(--slate-700);`

### Input Box

```css
background: var(--white);
border: 1px solid var(--slate-200);
border-radius: 16px;
box-shadow: var(--shadow-md);
```
Focus: `border-color: var(--sage-400); box-shadow: var(--shadow-lg), 0 0 0 3px rgba(46,125,51,0.12);`

### Modals

```css
/* Overlay */
background: rgba(0,0,0,0.4);
z-index: 1000;

/* Dialog */
background: var(--white);
border-radius: 16px;
box-shadow: var(--shadow-xl);
max-width: 480px to 640px;
padding: var(--space-8);
animation: modalSlideUp 0.3s var(--ease-out);
```

### Dropdowns

```css
background: var(--white);
border: 1px solid var(--slate-100);
border-radius: 12px;
box-shadow: 0 8px 32px rgba(0,0,0,0.12);
padding: var(--space-2) 0;
z-index: 1000;
```

### Tags / Chips

```css
padding: 4px 10px;
border-radius: 6px to 8px;
font-size: 0.68rem to 0.75rem;
font-weight: 400 to 500;
background: var(--sage-50) or var(--slate-50);
color: var(--sage-600) or var(--slate-600);
```

### Toggle Switch

```css
/* Track */
width: 32px; height: 18px;
border-radius: 9px;
background: var(--slate-200);         /* off */
background: var(--sage-500);          /* on */

/* Thumb */
width: 14px; height: 14px;
border-radius: 50%;
background: var(--white);
box-shadow: 0 1px 3px rgba(62,39,35,0.15);
transform: translateX(14px);          /* on */
```

### Avatar

```css
width: 32px; height: 32px;
border-radius: 50%;
background: linear-gradient(135deg, var(--slate-600), var(--slate-700));
font-size: 0.75rem;
font-weight: 500;
color: var(--slate-200);
```

### Navigation Item

```css
padding: var(--space-2) var(--space-3);
border-radius: 8px;
color: var(--slate-400);
font-size: 0.9rem;
font-weight: 400;
```
Hover: `color: var(--slate-200); background: rgba(255,255,255,0.04);`
Active: `color: var(--white); background: rgba(255,255,255,0.07);`

---

## 10. Iconography

- **Library:** Inline SVGs (Feather-style, consistent stroke)
- **Stroke width:** `1.5` to `2` for standard icons, `1.8` for medium icons
- **Caps:** `stroke-linecap="round" stroke-linejoin="round"`
- **Sizes:**
  - Inline/small: `12px` - `13px`
  - Standard: `16px`
  - Navigation: `18px`
  - Feature: `20px` - `24px`
  - Hero: `28px` - `40px`

---

## 11. Scrollbar Styling

```css
::-webkit-scrollbar { width: 6px; }
::-webkit-scrollbar-track { background: transparent; }
::-webkit-scrollbar-thumb {
  background: var(--slate-200);
  border-radius: 3px;
}
::-webkit-scrollbar-thumb:hover { background: var(--slate-300); }
```

---

## 12. Design Principles

1. **Warm, earthy palette** — Brown-grey neutrals with sage green accent. Never cold blue-grey.
2. **Quiet confidence** — Generous whitespace, restrained color usage, no competing focal points.
3. **Consistent depth** — Shadows use warm `rgba(62,39,35,...)` tones, not pure black.
4. **Soft interactions** — All transitions use the custom ease-out curve. Hover states are subtle.
5. **Serif for personality** — Display headings use Newsreader (serif) to add warmth. All UI text uses Inter.
6. **Progressive disclosure** — Panels slide in, messages animate up, chips scale in. Content enters naturally.
7. **One accent color** — Sage green is the only accent. It marks active states, focus rings, and primary actions.

---

## 13. Applying to New Projects

### Quick Setup

1. Copy the `:root` CSS variables block (colors, spacing, shadows, transitions)
2. Import the Google Fonts (Inter + Newsreader)
3. Set `html { font-size: 15px; }` and `body { font-family: var(--font-body); color: var(--slate-900); }`
4. Apply `--warm-white` as the main background, `--white` for cards
5. Use `--slate-100` / `--slate-200` for borders, `--slate-400` for placeholder text
6. Use `--sage-500` / `--sage-400` sparingly for active states and focus rings

### Token Override Guide

To adapt for a different brand:

| What to change | Tokens |
|---|---|
| Brand color | `--sage-*` (swap green for your accent) |
| Text warmth | `--slate-900` through `--slate-400` |
| Background warmth | `--warm-white`, `--slate-50` |
| Shadow warmth | Update `rgba(62,39,35,...)` in shadow tokens |
| Display font | `--font-display` |
| Base font size | `html { font-size }` (default: 15px) |
