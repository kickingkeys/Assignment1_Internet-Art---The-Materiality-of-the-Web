# Digital Decay

An interactive web art piece exploring the concept of digital impermanence through visual deterioration.

## Concept

Digital Decay is a minimalist webpage that transforms from a clean, aesthetic design into glitched corruption before fading entirely to black over a 20-second timeline. The piece comments on the ephemeral nature of digital content and the inevitable decay of all digital artifacts.

## Current Implementation Status

### Step 1: Base Structure ✅
- Created the HTML layout with semantic structure
- Styled the initial pristine state with clean aesthetics
- Implemented a responsive design that works across devices
- Added a subtle grid background and positioned elements precisely
- Set up CSS variables for animation timeline and color palette

### Step 2: ASCII Art Creation ✅
- Designed enhanced ASCII art for the central focal point using block characters
- Created a more complex navigation ASCII element
- Developed multiple layers of corrupted ASCII versions for the decay animation
- Ensured ASCII characters are well-formed and display properly across browsers
- Added subtle text-shadow effects to enhance the visual appearance

### Step 3: Animation Framework ✅
- Set up CSS keyframe animations for all elements
- Created percentage-based animation timing variables
- Implemented a complete 20-second master timeline
- Added specific animations for each component (ASCII art, navigation, title, background)
- Designed layered corruption effects with varying opacity, positioning, and color shifts

## Technical Approach

The project uses pure HTML and CSS to create a visually evolving experience without any JavaScript:

- **HTML**: Semantic structure with header, navigation, and main content areas
- **CSS**: 
  - Clean, minimal aesthetic with variables for timing and colors
  - CSS animations and keyframes for creating the decay effect
  - CSS custom properties for controlling the animation timeline
  - Transform, opacity, and filter effects to create glitching visuals
  - Mix-blend-mode for creating glitch effects

## Animation Implementation

The decay animations are implemented through a series of coordinated keyframe animations:

1. **masterFade**: Controls the overall page darkness and color shifting
2. **asciiMainFade**: Fades out the original ASCII art
3. **asciiCorrupt1/2**: Gradually reveals corrupted versions with increasing intensity
4. **titleGlitch**: Applies color shifting, text-shadow, and position changes to the title
5. **navGlitch**: Distorts the navigation ASCII element
6. **containerGlitch**: Applies skew, translation, and rotation to the entire ASCII container
7. **gridFade**: Modifies the background grid visibility and dimensions
8. **overlayGlitch**: Controls the glitch overlay that applies color and noise effects

## Animation Timeline

The 20-second decay process is divided into specific phases:

```css
/* Timeline percentages */
--pristine-end-pct: 15%;        /* 3s / 20s = 15% */
--ascii-corrupt-start-pct: 15%; /* 3s / 20s = 15% */
--ascii-corrupt-end-pct: 35%;   /* 7s / 20s = 35% */
--nav-corrupt-start-pct: 35%;   /* 7s / 20s = 35% */
--nav-corrupt-end-pct: 50%;     /* 10s / 20s = 50% */
--major-glitch-start-pct: 50%;  /* 10s / 20s = 50% */
--major-glitch-end-pct: 75%;    /* 15s / 20s = 75% */
--fade-start-pct: 75%;          /* 15s / 20s = 75% */
--fade-end-pct: 90%;            /* 18s / 20s = 90% */
--blackout-start-pct: 90%;      /* 18s / 20s = 90% */
--blackout-end-pct: 100%;       /* 20s / 20s = 100% */
```

## Setup Instructions

1. Clone this repository
2. Open `index.html` in a modern web browser
3. Watch the digital decay process unfold over 20 seconds

## Timeline of Decay Effects

- **0-3 seconds**: Pristine state, subtle hints of upcoming decay
- **3-7 seconds**: Initial corruption of central ASCII art (first corruption layer appears)
- **7-10 seconds**: Navigation elements and title begin to corrupt
- **10-15 seconds**: Major glitching phase, colors shift dramatically, second corruption layer visible
- **15-18 seconds**: Elements begin to fade, increased darkness
- **18-20 seconds**: Final dissolution to complete blackness

## CSS Animation Techniques Used

- **Keyframe animations** for character corruption
- **RGB shifts** with mix-blend-mode properties
- **Transform and position distortion** (translate, skew, rotate)
- **Overlay techniques** with increasing opacity
- **CSS filters** (hue-rotate, brightness, blur) for visual distortion
- **Background manipulation** for additional effects
- **Timing functions** to control animation pacing
- **animation-fill-mode: forwards** to maintain final states

## References and Inspiration

- ASCII Art aesthetics
- Digital glitch art
- Web-based deterioration effects
- Data moshing techniques

---

*This is a work in progress for "Assignment 1: Internet Art - The Materiality of the Web"* 