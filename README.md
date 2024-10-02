# Self-Driving Car Simulation using Genetic Algorithm

## Overview

This project implements a self-driving car simulation using Genetic Algorithms (GA) to evolve optimal driving behaviors. The simulation is built entirely in JavaScript, allowing it to run in web browsers for easy access and visualization.

## Features

- Browser-based 2D car physics simulation
- Genetic Algorithm implementation for evolving car behaviors
- Customizable environments and obstacles
- Real-time visualization of car performance and evolution

## Requirements

- Modern web browser (Chrome, Firefox, Safari, or Edge)
- Local development server (e.g., Node.js with http-server, or Python's SimpleHTTPServer)

## Installation

1. Clone the repository:
   ```
   git clone https://github.com/yourusername/self-driving-car-ga-js.git
   cd self-driving-car-ga-js
   ```

2. No additional installation is required as the project uses vanilla JavaScript.

## Usage

1. Start a local development server in the project directory. For example, if you have Node.js installed:
   ```
   npx http-server
   ```

2. Open your web browser and navigate to `http://localhost:8080` (or the appropriate port).

3. The simulation should start automatically in your browser.

## How It Works

1. **Car Model**: Each car is represented by a simple neural network implemented in JavaScript. It takes sensor inputs and outputs driving actions.

2. **Genetic Algorithm**:
   - A population of cars is initialized with random neural network weights.
   - Cars are evaluated based on their performance in the simulation (distance traveled, collisions avoided, etc.).
   - The best-performing cars are selected for reproduction.
   - Crossover and mutation operations are applied to create a new generation of cars.
   - The process repeats for a set number of generations or until a satisfactory performance is achieved.

3. **Simulation Environment**: The environment includes various obstacles and goals that the cars must navigate, all rendered in the browser using HTML5 Canvas or WebGL.

## Configuration

Adjust the following parameters in `config.js`:

- `POPULATION_SIZE`: Number of cars in each generation
- `NUM_GENERATIONS`: Number of generations to run
- `MUTATION_RATE`: Probability of mutation in genetic algorithm
- `CROSSOVER_RATE`: Probability of crossover in genetic algorithm

## Project Structure

- `index.html`: Main entry point for the application
- `styles.css`: CSS styles for the user interface
- `main.js`: Core simulation logic and genetic algorithm implementation
- `car.js`: Car model and physics
- `neuralNetwork.js`: Neural network implementation for car decision making
- `environment.js`: Simulation environment setup and obstacle generation

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Inspired by the work of [relevant researchers or projects in the field]
- Thanks to [any individuals or organizations that provided support or resources]
