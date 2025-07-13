# Battleship Game

## Overview

This is a browser-based implementation of the classic Battleship game where a player competes against the computer. The game features a drag-and-drop interface for ship placement, a dynamic gameboard, and turn-based attack mechanics. The UI visually updates to reflect hits and misses, providing immediate feedback to the player.

---

## Features and Strengths

- **Interactive Drag-and-Drop Ship Placement:** Players can intuitively position their ships on the grid before the game starts.
- **Clear Visual Feedback:** Hits and misses are color-coded on both player and computer boards.
- **Modular Architecture:** Core game logic (board state, ships, attacks) is separated from UI rendering and event handling, improving maintainability.
- **Randomized Computer Ship Placement:** The computer places ships with logic to avoid overlap and out-of-bounds placement.
- **Simple, Responsive UI:** The game is easy to understand and interact with on standard desktop browsers.

---

## Areas for Improvement

- **Separation of Concerns Could Be Stronger:** UI and game logic are mostly separated, but event handling and game flow control are mixed within `index.js`. Refactoring event listeners into dedicated UI or controller modules would improve clarity and scalability.
- **Lack of Game State Persistence:** Currently, there’s no saving or restoring of game progress — implementing local storage or backend support would enhance user experience.
- **Limited Accessibility:** The drag-and-drop interface lacks keyboard navigation support and screen reader friendliness.
- **Basic AI Logic:** The computer's attack strategy is purely random without targeting logic, which can be improved to create a more challenging opponent.
- **No Mobile Support Yet:** The UI and interactions have not been optimized for touch devices.
- **Minimal Styling and Animations:** Adding CSS animations or transitions could make the gameplay more engaging visually.

---

## How to Run

1. Clone or download the repository.
2. Open `template.html` in a modern web browser.
3. Drag and drop ships on the player board.
4. Click enemy cells to attack and play against the computer.
