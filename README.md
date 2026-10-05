# Animation🎨 CSS Animation Examples

A beginner-friendly HTML and CSS animation project that demonstrates different types of CSS animations using "@keyframes", "transform", "opacity", "animation-delay", and other CSS animation properties.

The project contains several animated squares, a square-path animation, and a Google-style bouncing ball animation.

📸 Project Overview

The project demonstrates the following animations:

Basic Animations

- 🎨 Color – Changes the background color
- 🔄 Rotate – Rotates the element
- ↕️ Move – Moves the element vertically
- 🌫️ Fade – Changes the opacity
- 🌀 Spin – Creates a spinning loader effect
- 💓 Pulse – Enlarges and shrinks the element

Advanced Animations

- 🔷 Square Path Animation – Moves a square around a rectangular path
- 🔴🟠🟡🟢 Google Animation – Creates a bouncing-ball effect using multiple colored balls and animation delays

🛠️ Technologies Used

- HTML5
- CSS3
- CSS "@keyframes"
- CSS "transform"
- CSS animations

No external libraries or frameworks are required.

📂 Project Structure

css-animation-examples/
│
├── index.html
└── README.md

🎬 Animation Examples

1. Color Animation

The first square continuously changes between crimson and light green.

@keyframes color {
    0% {
        background-color: crimson;
    }

    50% {
        background-color: rgb(167, 240, 165);
    }

    100% {
        background-color: crimson;
    }
}

This demonstrates changing an element's background color over time.

---

2. Rotate Animation

The second square rotates through a complete 360-degree rotation.

@keyframes rotate {
    0% {
        transform: rotate(0);
    }

    50% {
        transform: rotate(180deg);
    }

    100% {
        transform: rotate(360deg);
    }
}

This demonstrates the CSS "rotate()" transform.

---

3. Move Animation

The third square moves vertically between two positions.

@keyframes Move {
    from {
        transform: translate(0, 100px);
    }

    to {
        transform: translate(0, -100px);
    }
}

This demonstrates the "translate()" transform.

---

4. Fade Animation

The fourth square repeatedly fades in and out.

@keyframes Fade {
    0% {
        opacity: 0;
    }

    50% {
        opacity: 1;
    }

    100% {
        opacity: 0;
    }
}

The "opacity" property controls the visibility of the element.

---

5. Spin Animation

The fifth square is styled as a circular loading spinner.

.s5 {
    border: 10px solid white;
    border-top: 10px solid blue;
    border-radius: 50%;
    animation-name: rotate;
}

It uses the previously defined "rotate" animation to create a spinning effect.

---

6. Pulse Animation

The sixth square continuously grows and returns to its original size.

@keyframes Pulse {
    0% {
        transform: scale(1);
    }

    50% {
        transform: scale(1.5);
    }

    100% {
        transform: scale(1);
    }
}

This demonstrates the CSS "scale()" transform.

🔷 Square Path Animation

The project also contains a blue square that moves around a rectangular path.

@keyframes box {
    0% {
        transform: translate(0, 0);
    }

    25% {
        transform: translate(435px, 0);
    }

    50% {
        transform: translate(435px, 300px);
    }

    75% {
        transform: translate(0, 300px);
    }

    100% {
        transform: translate(0, 0);
    }
}

Movement Pattern

┌───────────────────────────────┐
│  🔷 ───────────────────────→  │
│                               │
│                               ↓
│  ←──────────────────────── 🔷 │
│  ↑                            │
└───────────────────────────────┘

The square moves:

1. From the top-left to the top-right
2. From the top-right to the bottom-right
3. From the bottom-right to the bottom-left
4. From the bottom-left back to the top-left

🔴 Google-Style Animation

The project creates six colored balls that move vertically with different animation delays.

<div class="ball b1"></div>
<div class="ball b2"></div>
<div class="ball b3"></div>
<div class="ball b4"></div>
<div class="ball b5"></div>
<div class="ball b6"></div>

The balls use:

.ball {
    animation-timing-function: ease-in-out;
    animation-name: google;
    animation-duration: 3s;
    animation-iteration-count: infinite;
}

The animation is defined as:

@keyframes google {
    0%, 100% {
        transform: translate(0);
    }

    50% {
        transform: translate(0, 50px);
    }
}

⏱️ Animation Delays

Each ball starts its animation at a different time.

Ball| Color| Delay
B1| Red| 0s
B2| Orange| 0.3s
B3| Yellow| 0.6s
B4| Green| 0.9s
B5| Brown| 1.2s
B6| Cornflower Blue| 1.5s

The different delays create a sequential bouncing effect.

For example:

.b2 {
    background-color: orange;
    animation-delay: .3s;
}

.b3 {
    background-color: yellow;
    animation-delay: .6s;
}

⚙️ Important CSS Animation Properties

The project demonstrates several important CSS animation properties:

Property| Purpose
"animation-name"| Specifies the animation
"animation-duration"| Controls animation speed
"animation-iteration-count"| Controls how many times it repeats
"animation-delay"| Delays the start of an animation
"animation-timing-function"| Controls animation speed behavior
"@keyframes"| Defines animation stages
"transform"| Moves, rotates, or scales elements
"opacity"| Controls visibility

▶️ How to Run

1. Create a folder named "css-animation-examples".
2. Create an "index.html" file.
3. Copy the provided HTML and CSS code into the file.
4. Save the file.
5. Open "index.html" in a modern web browser.
6. Observe the different animations running continuously.

🎯 Learning Objectives

This project helps beginners understand:

- CSS animations
- "@keyframes"
- "animation-name"
- "animation-duration"
- "animation-delay"
- "animation-iteration-count"
- Animation timing functions
- CSS transforms
- "translate()"
- "rotate()"
- "scale()"
- "opacity"
- Creating loading animations
- Creating sequential animations

💡 Possible Improvements

The project could be improved by:

- Adding smooth hover-triggered animations
- Making the animation layout responsive
- Adding animation controls such as Play/Pause
- Adding more animation examples
- Using CSS variables for colors
- Adding animation direction examples
- Demonstrating "animation-fill-mode"
- Demonstrating "animation-direction"
- Adding transitions between different states
- Replacing fixed pixel movement values with responsive units

⚠️ Note

The Square Path Animation uses fixed values such as:

transform: translate(435px, 300px);

Because these values are fixed, the animation may not scale correctly on smaller screens.

For a responsive version, relative units or a more flexible layout can be used.

👨‍💻 Author

Created as a beginner-friendly HTML & CSS Animation project for practicing CSS "@keyframes", transforms, timing, delays, and animation effects.
