# Digital Decay

An interactive web art piece exploring the concept of digital impermanence through visual deterioration.

## Concept

Digital Decay is a minimalist webpage that transforms from a clean, aesthetic design into glitched corruption before fading entirely to black over a 20-second timeline. The piece comments on the ephemeral nature of digital content and the inevitable decay of all digital artifacts. Starting with a simple seed character, the work metaphorically represents how digital entropy spreads through systems, gradually consuming and transforming the pristine into chaos, culminating in a mesmerizing display of random characters that consume the viewport before fading to darkness.

## Current Implementation Process

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

## How to Set Up and Run This Application

1. **Clone the Repository**
   ```
   git clone https://github.com/kickingkeys/Assignment1_Internet-Art---The-Materiality-of-the-Web.git
   cd digital-decay
   ```

2. **Local Development**
   - Open `index.html` in any modern browser
   - For the best experience, view in Chrome, Firefox, or Safari
   - The animation will automatically begin and run for 20 seconds

3. **Restarting the Animation**
   - Refresh the page to restart the animation sequence
   - Each viewing provides a slightly different experience due to the random nature of some animations

## Technical Approach

The project uses pure HTML and CSS to create a visually evolving experience: (mostly)

### HTML Structure
- Simple semantic structure with main container
- Multiple layers of ASCII art positioned for the corruption sequence
- Random character grid overlay system
- SVG filter definitions for advanced glitch effects
- Overlay elements for glitch and fade effects

### CSS Techniques
- CSS Grid for random character positioning (80x50 grid)
- CSS Variables for timing control and animation coordination
- Complex keyframe animations for visual decay
- CSS Filters and blend modes for visual distortion
- Individual character animations with calculated delays
- Responsive design with media queries

### Animation Implementation

The decay animations are implemented through several coordinated systems:

1. **Central ASCII Evolution**
   - seedPulse: Initial pulsing of the seed character
   - spread1/2/3: Controls the appearance and fading of corruption layers

2. **Random Character Grid**
   - 4000 individual characters
   - Row-by-row appearance animation
   - Calculated delays for smooth filling effect
   - Scale and rotation effects during disappearance

3. **Master Effects**
   - masterFade: Controls overall page darkness
   - gridFade: Background grid dissolution
   - finalBlackout: Clean fade to pure black

## Animation Timeline

The 20-second decay process is divided into specific phases:

1. **0-5 seconds**: Initial state
   - Single 's' character pulses in center
   - Random characters begin appearing row by row from top of screen
   - Grid background visible with subtle animation

2. **5-9 seconds**: First Pattern Emergence
   - First spread pattern forms around central 's'
   - More random characters continue filling the viewport
   - Initial corruption patterns begin to form

3. **8-13 seconds**: Pattern Evolution
   - Second spread pattern emerges
   - Random characters continue filling more of the screen
   - Increased complexity in corruption patterns

4. **12-17 seconds**: Maximum Corruption
   - Largest spread pattern forms
   - Random characters now fill entire viewport
   - Peak of visual complexity

5. **15-20 seconds**: Dissolution
   - Random characters begin disappearing
   - Final fade to pure black (#000000)
   - Complete darkness achieved at 20 seconds

## Timeline of Decay Effects

- **0-3 seconds**: Pristine state, subtle pulsing of seed character
- **3-7 seconds**: Initial corruption spreads from the seed (first corruption layer appears)
- **7-10 seconds**: Second corruption layer begins to appear
- **10-15 seconds**: Major glitching phase, colors shift dramatically, more complex patterns emerge
- **15-18 seconds**: Elements begin to fade, increased darkness and visual distortion
- **18-20 seconds**: Final dissolution to complete blackness

## Technical Challenges and Solutions

### Challenges:

1. **Creating Complex Visual Effects Without JavaScript**
   - Successfully implemented a grid of 4000 random characters using CSS Grid
   - Coordinated multiple animation timelines for smooth character appearance/disappearance
   - Used CSS custom properties for precise timing calculations

2. **Browser Compatibility**
   - Some CSS filters and blend modes behave differently across browsers
   - Tested in multiple browsers and adjusted code to ensure consistent experience

3. **Performance Optimization**
   - Optimized grid animations using transform and opacity
   - Implemented row-based animation delays to reduce CPU load
   - Carefully tuned animation timing to prevent stuttering

4. **ASCII Art Positioning**
   - Maintaining proper alignment of multiple ASCII layers was challenging
   - Solved using absolute positioning and careful transform adjustments

## Deployment to Netlify

1. Connected my GitHub repository to Netlify
2. Configured the build settings (not required for this static site)
3. Set up automatic deployments from the main branch
4. Tested the deployed version to ensure animations work properly
5. Project is live at: [ https://relaxed-zuccutto-35622b.netlify.app/ ]

## CSS Animation Techniques Used

- **Keyframe animations** for character corruption
- **RGB shifts** with mix-blend-mode properties
- **Transform and position distortion** (translate, skew, rotate)
- **Overlay techniques** with increasing opacity
- **CSS filters** (hue-rotate, brightness, blur) for visual distortion
- **SVG filters** for more complex displacement effects
- **Background manipulation** for additional effects
- **Timing functions** to control animation pacing
- **animation-fill-mode: forwards** to maintain final states

## Future Enhancements

If I had more time or in a future version, I would:

1. Add user interaction to influence the decay process
2. Implement audio effects to accompany the visual decay
3. Create more elaborate ASCII patterns that respond to mouse movement
4. Add text that becomes increasingly corrupted as the animation progresses
5. Create alternative decay sequences with different visual styles

## Inspiration and References

- **Glitch Art Aesthetics**: Inspired by artists like Rosa Menkman and the glitch art movement
- **Early Net Art**: Influences from Jodi.org and early internet art experiments
- **Digital Entropy**: Concepts from information theory about data degradation
- **ASCII Art Culture**: Drawing on the rich history of ASCII art in digital spaces

### Technical Resources Used:
- [MDN Web Docs: CSS Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations)
- [CSS-Tricks: A Guide to CSS Animation](https://css-tricks.com/almanac/properties/a/animation/)
- [Smashing Magazine: Advanced CSS Animations](https://www.smashingmagazine.com/2018/04/background-css-animations/)
- [CSS SVG Filters](https://developer.mozilla.org/en-US/docs/Web/CSS/filter)

## Personal Reflection

Creating Digital Decay has been a fascinating exploration of how digital content ages and deteriorates. While physical objects show wear through physical processes, digital decay happens through corruption, format obsolescence, and the fragility of our storage systems.

Working within the constraints of HTML and CSS pushed me to find creative solutions for visual effects typically accomplished with JavaScript. This constraint actually enhanced the conceptual framework of the piece - just as digital systems have inherent constraints that shape how they break down.

The most challenging aspect was creating a meaningful progression of decay that felt organic rather than mechanical. I wanted the viewer to experience a sense of inevitable loss as the pristine digital space gradually succumbs to entropy.

This project has deepened my appreciation for the materiality of the web - despite its seemingly immaterial nature, digital content has its own forms of physicality and decay that this piece attempts to make visible.

---

*This project was created for "Assignment 1: Internet Art - The Materiality of the Web"* 