# Agent Guidelines for Truck Snake

## Project Structure
- Single-page browser game: `truck-snake.html` with embedded CSS and JavaScript
- Assets stored in `assets/` directory (SVG/PNG images for game sprites)
- No build process, testing framework, or package dependencies

## Running the Game
- Open `truck-snake.html` in a web browser (no build required)
- No test commands available (manual testing only)

## Code Style

### HTML/CSS
- Use 4-space indentation consistently
- Embedded styles in `<style>` tag within `<head>`
- BEM-like naming for CSS classes (e.g., `.game-container`, `.canvas-container`)

### JavaScript
- Vanilla JavaScript (no frameworks or dependencies)
- `let` and `const` for variable declarations (no `var`)
- camelCase for variable and function names (e.g., `updateTruck`, `gameOver`, `intervalTime`)
- Object destructuring avoided; use `Object.assign({}, obj)` for copying
- String concatenation with template literals: `` `Score: ${score}` ``
- Arrow functions for event listeners and callbacks
- No semicolons required but used consistently

### Game Logic Conventions
- Grid-based movement using `stepSize = 32` (matches sprite dimensions)
- Canvas size: 640x640 pixels
- LocalStorage key: `truck-snake-highScores` for persistence
