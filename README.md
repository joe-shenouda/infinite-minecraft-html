# Infinite Minecraft-like World

This project demonstrates an infinite, procedurally generated, Minecraft-like world using **Three.js** and **Simplex Noise**. The world features blocks of grass, dirt, and stone, with adjustable terrain height and rendering distance.

## Table of Contents

- [Demo](#demo)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Code Overview](#code-overview)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

## Demo

Check out the live demo [here](https://joe-shenouda.github.io/infinite-minecraft-html/).

## Features

- Infinite, procedurally generated terrain
- Smooth camera controls with WASD and pointer lock
- Simple block placement and removal with mouse click
- Adjustable render distance for performance optimization
- Real-time chunk generation and disposal based on player position

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/infinite-minecraft-like-world.git
   ```
2. Navigate to the project directory:
   ```bash
   cd infinite-minecraft-like-world
   ```
3. Open `index.html` in your web browser to start the application.

## Usage

- **Move**: Use `W`, `A`, `S`, `D` to move forward, left, backward, and right respectively.
- **Look Around**: Click to lock the pointer and look around.
- **Place Block**: Left-click to place a grass block.
- **Remove Block**: Right-click to remove a block.
- **Fly Up**: Press `Space` to move up.
- **Fly Down**: Press `Shift` to move down.

## Code Overview

### Initialization

The scene, camera, renderer, and controls are initialized in the `init()` function. The initial chunks are generated and event listeners are set up for window resize, mouse click, and keyboard input.

### Chunk Generation

Chunks are generated using Simplex Noise to create varying terrain heights. The `generateChunk()` function is responsible for creating the geometry and mesh for each chunk.

### Controls

The `PointerLockControls` are used to manage the camera's movement and locking mechanism. Movement is handled by adjusting the camera's position based on key inputs.

### Block Manipulation

Blocks can be placed and removed using the mouse buttons. The `placeBlock()` and `removeBlock()` functions handle these actions and update the chunks accordingly.

### Real-time Updates

The `animate()` function continuously updates the scene, checks player movement, and generates or removes chunks as needed.

## Customization

- **Render Distance**: Adjust the `renderDistance` variable to change how many chunks are rendered around the player.
- **Terrain Height**: Modify the `chunkHeight` variable to change the maximum height of the terrain.
- **Movement Speed**: Change the `moveSpeed` variable to adjust how fast the player moves.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes. Ensure that your code follows the existing style and include tests where applicable.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Built by Joe Shenouda (Cyber-Consult.org) with ❤️ using [Three.js](https://threejs.org/) and [Simplex Noise](https://github.com/jwagner/simplex-noise.js).
