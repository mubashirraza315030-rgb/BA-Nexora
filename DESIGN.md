---
name: Nexora AI Narrative
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#393939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#bac9cc'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#849396'
  outline-variant: '#3b494c'
  surface-tint: '#00daf3'
  primary: '#c3f5ff'
  on-primary: '#00363d'
  primary-container: '#00e5ff'
  on-primary-container: '#00626e'
  inverse-primary: '#006875'
  secondary: '#f8acff'
  on-secondary: '#570067'
  secondary-container: '#e248ff'
  on-secondary-container: '#4c005a'
  tertiary: '#ffeac0'
  on-tertiary: '#3e2e00'
  tertiary-container: '#fec931'
  on-tertiary-container: '#6f5500'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#9cf0ff'
  primary-fixed-dim: '#00daf3'
  on-primary-fixed: '#001f24'
  on-primary-fixed-variant: '#004f58'
  secondary-fixed: '#ffd6ff'
  secondary-fixed-dim: '#f8acff'
  on-secondary-fixed: '#350040'
  on-secondary-fixed-variant: '#7b0090'
  tertiary-fixed: '#ffdf96'
  tertiary-fixed-dim: '#f3bf26'
  on-tertiary-fixed: '#251a00'
  on-tertiary-fixed-variant: '#594400'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 64px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-sm:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1.0'
    letterSpacing: 0.1em
  headline-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  container-max: 1440px
  gutter: 24px
  margin-desktop: 64px
  margin-mobile: 20px
  stack-sm: 12px
  stack-md: 24px
  stack-lg: 48px
---

## Brand & Style

The design system is engineered for a high-performance, AI-driven future. It targets tech-savvy professionals and developers who value speed, precision, and a "bleeding-edge" aesthetic. The brand personality is hyper-modern, sophisticated, and slightly mysterious—evoking the feeling of a command center for the next generation of artificial intelligence.

The visual direction is **Cyber-Glassmorphism**. It combines the raw, high-contrast energy of cyberpunk with the refined polish of modern Silicon Valley SaaS. The UI relies on deep obsidian surfaces, translucent glass layers, and vibrant neon accents that act as "light sources" within a dark digital void. Every element should feel like a holographic projection: ethereal yet structurally sound.

## Colors

The palette is built on a "True Black" foundation to maximize OLED contrast and power efficiency. 

- **Primary (Electric Blue):** Used for primary actions, progress indicators, and active states. It represents the "pulse" of the AI.
- **Secondary (Vivid Magenta):** Used for accents, data visualization, and secondary highlights to provide a dual-tone neon aesthetic.
- **Neutral (Slate Grays):** Reserved for low-priority text and subtle borders to prevent the UI from becoming overwhelming.
- **Glass Surfaces:** Semi-transparent overlays use a blurred slate gray to create depth without sacrificing the obsidian backdrop.

## Typography

The typography system creates a "technical editorial" feel. 

**Space Grotesk** is used for all headlines. Its geometric quirks and futuristic terminal cuts reinforce the AI theme. Use tight tracking for large display headers to increase impact.

**Inter** provides high legibility for complex data and body copy, ensuring that despite the aggressive styling, the tool remains functional and easy to read.

**JetBrains Mono** (Label Font) is introduced for metadata, code snippets, and small labels to lean into the developer-centric, "under-the-hood" nature of the system.

## Layout & Spacing

The layout philosophy follows a **strict 4px grid** within a **fluid 12-column system**. 

While the grid is rigid, the negative space is generous. Content should feel like it has room to "breathe" on the glass planes. Large margins (64px+) are used on desktop to center the focus. 

Breakpoints:
- **Mobile (<768px):** 4 columns, 20px margins. Headlines scale down significantly.
- **Tablet (768px - 1280px):** 8 columns, 40px margins.
- **Desktop (>1280px):** 12 columns, 64px margins, 1440px max-width.

## Elevation & Depth

Depth is not achieved through traditional shadows, but through **Backdrop Blurs** and **Luminous Borders**.

- **Level 0 (Floor):** Pure #000000.
- **Level 1 (Navigation/Background Elements):** Subtle 20px blur with a 5% white overlay.
- **Level 2 (Cards/Modals):** 40px backdrop blur, 10% white overlay, and a 1px "inner-glow" border (Primary color at 20% opacity).
- **Active States:** Elements being hovered or interacted with should emit a soft outer glow (`box-shadow: 0 0 20px`) using the Primary or Secondary neon colors. 

The "3D Hover" effect is achieved by a slight scale increase (1.02x) and a shift in the gradient border intensity, making the component appear to tilt toward the user.

## Shapes

The design system utilizes a **Soft-Tech** shape language. Elements are not perfectly sharp (which feels too aggressive) nor fully rounded (which feels too consumer-friendly). 

- **Primary UI Elements:** 4px (0.25rem) corner radius.
- **Containers & Cards:** 8px (0.5rem) corner radius.
- **Interactive Triggers:** Buttons use a 4px radius to maintain a precise, engineered look.

The use of thin (1px) lines for all borders is mandatory to maintain the "holographic" aesthetic.

## Components

### Buttons
- **Primary:** Solid Electric Blue text on a transparent background with a 1px Primary border. On hover, the button gains a subtle blue outer glow and a 10% Primary fill.
- **Ghost:** White text with no border. On hover, it gains a Magenta underline or "scanline" effect.

### Cards
- Surfaces must use `backdrop-filter: blur(20px)`.
- Borders are 1px solid `rgba(255,255,255,0.1)`.
- On hover, the border color transitions to the Primary Electric Blue.

### Input Fields
- Underline-only or subtle 4-sided borders. 
- When focused, the label (in JetBrains Mono) should glow slightly, and the cursor should be a solid Primary color block.

### Chips / Status Indicators
- Small, uppercase labels. 
- Use "Pulse" animations (a soft breathing opacity) for live AI processing states.

### Background Gradients
- Use "Orbs" of blurred color (#00E5FF and #D500F9) placed randomly behind the glass UI layers to create a sense of moving energy and depth.