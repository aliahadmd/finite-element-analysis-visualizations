# FEA Mesh Visualizations

Interactive visualizations accompanying the review paper "Mesh Discretization and Accuracy in Finite Element Analysis".

## Getting Started

Open `index.html` in any modern browser - no server required. All files are standalone with embedded CSS/JavaScript.

## Visualizations

### index.html - Main Landing Page
Navigation hub with cards linking to all 7 visualizations. Includes sidebar navigation and responsive layout.

### 01-domain-discretization.html
Demonstrates how continuous 2D domains are divided into finite elements.
- Domain shapes: Rectangle, L-shape
- Element types: Quadrilaterals, Triangles
- Adjustable mesh density slider
- Real-time element/node/DOF count display

### 02-shape-functions.html
3D visualization of polynomial shape functions on triangular elements using Three.js.
- Linear (3-node) and Quadratic (6-node) shape functions
- Interactive node selection to highlight individual functions
- Partition of unity demonstration (sum = 1)
- Orbit controls for 3D rotation/zoom

### 03-mesh-types-comparison.html
Side-by-side comparison of structured vs unstructured meshes.
- Split-screen canvas layout
- Geometry options: Square with hole, L-bracket
- Quality metrics display for each mesh type
- Synchronized density controls

### 04-h-refinement.html
Demonstrates element subdivision refinement strategies.
- Plate with circular hole geometry
- Uniform and adaptive refinement modes
- Error-based element coloring
- Step-by-step refinement controls
- Element count and error metrics

### 05-p-refinement.html
Shows how polynomial degree affects approximation quality.
- Single element with adjustable p (1-4)
- Target function: sin(2πx)
- Interpolated approximation overlay
- Node positions for each polynomial degree
- DOF count display

### 06-convergence-plot.html
Interactive mesh convergence study using Chart.js.
- Log-log scale error vs mesh size plot
- Add custom data points
- Pre-loaded linear/quadratic examples
- Convergence rate computation via regression
- Richardson extrapolation estimate
- Theoretical slope reference lines

### 07-element-quality.html
Real-time element quality metrics with draggable nodes.
- Quadrilateral and Triangle element types
- Drag corner nodes to distort element
- Live computation of:
  - Aspect ratio
  - Skewness
  - Jacobian ratio
- Color-coded quality indicators
- Reset to ideal shape button

## Technologies

- **Three.js r128** - 3D graphics (shape functions)
- **Chart.js 4.4.0** - 2D charts (convergence plot)
- **MathJax 3** - Mathematical notation
- **Vanilla JavaScript** - Interactive controls

## Browser Support

Tested in Chrome, Firefox, and Edge.

## Author

**Ali Ahad**
- Website: [aliahad.com](https://aliahad.com)
- Resume: [resume.aliahad.com](https://resume.aliahad.com)

© 2026 Ali Ahad. All rights reserved.
