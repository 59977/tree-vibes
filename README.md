# 3D Tree Generator

## Overview

The 3D Tree Generator is a web-based application that procedurally generates 3D trees with realistic textures and structures using Three.js. It uses dynamically generated textures for bark, bump maps, leaves, and stems. The user interface allows you to customize various parameters such as the maximum depth of branches, initial branch length and thickness, branch spread, branch factor, branch probability, decay factors, and leaf size.

## Features

- Procedural generation of intricate 3D trees
- Customizable parameters:
  - Max Depth of tree
  - Initial branch length and thickness
  - Branch spread and branch factor
  - Branch probability and decay factors (for both length and thickness)
  - Leaf size and leaf placement
- Realistic textures for bark, leaves, and stems generated dynamically using HTML5 Canvas
- Interactive UI to adjust tree parameters and regenerate the tree
- Smooth camera control using OrbitControls

## How to Run

This project utilizes JavaScript ES modules, so it must be run from a local web server. Follow these steps:

1. Clone the repository:
   ```
   git clone <repository-url>
   cd vibe-3d
   ```

2. Run a local web server. You can use one of the following methods:

   ### Using Python (if installed):
   ```
   python3 -m http.server 8000
   ```
   Then open your browser and navigate to: [http://localhost:8000/index.html](http://localhost:8000/index.html)

   ### Using Node.js with http-server:
   First, install http-server (if you don't have it):
   ```
   npm install -g http-server
   ```
   Then, start the server:
   ```
   http-server -p 8000
   ```
   Open [http://localhost:8000/index.html](http://localhost:8000/index.html) in your browser.

3. Modify parameters using the UI on the left side of the page and click the "Generate Tree" button to see the changes.

## Project Structure

- **index.html**: The main entry point that sets up the Three.js scene, camera, renderer, and user interface.
- **js/three.module.js**: The Three.js library (imported as an ES module).
- **js/OrbitControls.js**: The OrbitControls module for interactive camera control.

## Requirements

- A modern web browser with support for WebGL and ES modules.
- A local web server to serve the project files due to the module-based imports.

## Customization

Feel free to adjust the parameters in the UI or modify the code in `index.html` to experiment with different tree-generation styles and animations.

## License

This project is provided under the MIT License.

Enjoy generating unique 3D trees! 