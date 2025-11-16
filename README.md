# han1lsatothemax
📍 Pixel Reveal Visualization
Interactive Image Decomposition Using Recursive Circle Subdivision

(Inspired by KoalasToTheMax — custom version revealing han1lsa)

🎨 Overview

Pixel Reveal Visualization is an interactive web application that gradually reveals an image through recursive subdivision of colored circles.
As the user moves the cursor across the canvas, each circle splits into four smaller circles, each colored based on the average pixel color of its respective region.

In my version, the visualization is configured to reveal an image of my university campus, turning a simple graphic algorithm into an engaging and playful exploration experience.

The entire project is implemented using pure JavaScript and HTML5 Canvas, with no server-side code or backend processing.

🚀 Features

🔵 Recursive circle subdivision (quadtree-like algorithm)

🎨 Real-time pixel color sampling using Canvas API

🖱️ Interactive interface — circles split on hover

🏫 Custom image of university campus as the reveal target

⚡ Fully client-side, zero dependencies

📱 Works in any modern browser

🧠 How It Works
1. Image Loading

The image (campus.jpg) is loaded directly in the browser — no server needed.

2. Canvas Rendering

The app draws a single large circle covering the whole image.

3. User Interaction

When the cursor touches a circle:

The circle is removed.

Four new circles are created.

Each circle corresponds to one quadrant of the original circle’s region.

For each quadrant, the average RGB value of the underlying pixels is computed.

The circle is filled with this color.

4. Recursion

Each new circle can further subdivide until reaching the minimum size, gradually revealing the full image.

This method resembles quadtree spatial subdivision, but rendered as circles instead of rectangles, creating a smooth, aesthetically pleasing effect.

🛠 Technologies Used

JavaScript (ES6+)

HTML5 Canvas API

CSS3
