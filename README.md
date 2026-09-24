🚗 Self-Driving Car Simulation in Vanilla JavaScript

A 2D self-driving car simulation built from scratch in pure JavaScript and HTML5 Canvas, featuring ray-casting sensors, custom neural networks, and evolutionary algorithms without any external libraries.

🌟 Overview

This project demonstrates the core concepts behind autonomous vehicles and artificial intelligence by implementing a self-driving car in a simulated environment. The car senses its surroundings using ray-casting virtual sensors, processes inputs using a custom-built Neural Network, and learns to navigate traffic safely using a Genetic Algorithm / Evolutionary Approach.

✨ Features

🏎️ Physics & Car Dynamics: Custom physics engine for acceleration, friction, steering, and turn radius.

📡 Ray-Casting Sensors: Multi-directional sensors detecting distance to road borders and other vehicles/obstacles.

💥 Collision Detection: Polygon intersection algorithms to accurately detect precise visual boundaries and collisions.

🧠 Custom Neural Network: Multi-layer perceptron (MLP) built from scratch to calculate steering and speed controls.

🧬 Evolutionary Algorithm: Simulated genetic mutation and natural selection to optimize car control weights over successive generations.

📊 Real-time Neural Network Visualization: Canvas visualizer showing input values, network weights, biases, and decision nodes live.

💾 Local Storage Persistence: Save the best-performing neural network model directly in the browser's local storage.

🛠️ Tech Stack

Language: JavaScript (ES6+ / Vanilla)

Rendering: HTML5 Canvas API

Styling: CSS3

Tools: Browser LocalStorage API

🚀 Getting Started

No installations or build processes (npm, webpack, etc.) are required! You can run the project directly in any modern browser.

Prerequisites

All you need is a web browser (Google Chrome, Mozilla Firefox, Brave, Edge, etc.).

Installation

Clone the repository:
git clone https://github.com/Narcis734/Self-driving-car-js.git

Navigate into the project folder:
cd Self-driving-car-js

Open index.html in your favorite web browser (or use VS Code Live Server extension).

🎮 How It Works

Traffic & Environment: Randomly generated or static traffic lanes are created on a multi-lane highway.

Sensors: Each car emits rays that intersect with road boundaries and traffic obstacles.

Feed-Forward Neural Network: Sensor readings serve as inputs to hidden layers. Outputs determine four control states: Forward, Backward, Left, Right.

Training Process:

A population of cars is instantiated each generation.

The car that travels the furthest along the road is selected as the candidate.

Click the Save button to store the best network weights to localStorage.

On refresh, new cars clone the saved weights with slight random mutations to progressively improve driving accuracy.

📁 Project Structure

├── index.html         # Main application entry point & layout
├── style.css          # Visual styling and canvas positioning
├── car.js             # Car physics, controls, and boundary polygons
├── sensor.js          # Ray-casting implementation and intersection logic
├── network.js         # Neural Network (Layers, Level, Feed-Forward)
├── visualizer.js      # Live neural network architecture viewer
├── road.js            # Highway lanes, boundaries, and math projections
├── utils.js           # Mathematical functions (lerp, line intersections)
└── main.js            # Main animation loop, traffic generation, and mutation logic

💳 Acknowledgments & Credits

This project was built following the insightful course "Self-Driving Car with JavaScript Course – Neural Networks and Machine Learning" created by Radu Mariescu-Istodor and hosted on freeCodeCamp.

📺 Watch the Course on YouTube: https://www.youtube.com/watch?v=Rs_rAxEsAvI

👨‍🏫 Course Creator: Radu Mariescu-Istodor

📜 License

This project is open-source and available under the MIT License.
