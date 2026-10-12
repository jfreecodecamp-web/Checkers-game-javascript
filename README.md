# Checkers — Canvas Edition

**JavaScript · HTML5 Canvas · CSS · Browser game prototype**

A browser-based Checkers prototype built with vanilla JavaScript and HTML5 Canvas. Play a local two-player match or practice against a computer opponent with selectable piece colours and highlighted legal moves.

[Play live demo](https://jfreecodecamp-web.github.io/Checkers-game-javascript/) · [Browse source](https://github.com/jfreecodecamp-web/Checkers-game-javascript/blob/main/index.html) · [Developer profile](https://github.com/jfreecodecamp-web)

## Preview

![Checkers — Canvas Edition — game interface](https://github.com/user-attachments/assets/a90fe2a0-ba11-4cc3-a99d-b9428de8438c)

![Checkers — Canvas Edition — setup and gameplay](https://github.com/user-attachments/assets/35d993ce-49f4-42f6-b978-cbfa478a6bc0)

![Checkers — Canvas Edition — board view](https://github.com/user-attachments/assets/a70175ff-8096-42d3-bb7a-5f466c2b3929)

## Features

- Local Player vs Player and Player vs AI modes.
- Piece colour selection and an animated coin toss to choose the starting player.
- Highlighted legal moves, mandatory captures, and consecutive-jump handling.
- King promotion and extended diagonal movement for kings.
- Piece counters and an active-turn display.

## Run locally

No package installation or build step is required.

```bash
git clone https://github.com/jfreecodecamp-web/Checkers-game-javascript.git
cd Checkers-game-javascript
```

Open `index.html` in a current desktop browser. For a local HTTP server, run `python -m http.server 8000` from the project directory and visit **http://localhost:8000**. Python is only needed for the optional local server.

## How to play

1. Choose **Player vs Player** or **Player vs AI**, then select your piece colour.
2. After the coin toss, click one of your pieces to display its legal destinations.
3. Click a highlighted destination to move or capture; continue a capture sequence when another jump is available.
4. Kings are marked with **K**. The current win detection triggers when an opponent has no pieces left.

## Implementation highlights

| Area | Implementation |
| --- | --- |
| Board model | An 8 × 8 array stores pieces and promoted king values. |
| Rules | Move generation, mandatory-capture checks, promotion, and board updates. |
| Rendering | Canvas board, shaded pieces, selected-piece outline, and destination markers. |
| Turn flow | Local turns, delayed computer moves, piece counts, and coin-toss setup. |

## Repository guide

| File | Purpose |
| --- | --- |
| `index.html` | Complete application with inline styles, rules, Canvas rendering, and computer moves. |

## Project status

This prototype uses mouse controls and a custom rules variant with flying kings and backward captures. The AI currently chooses randomly from legal moves; the difficulty menu does not yet change its strategy. Win detection covers piece elimination; stalemate and draw handling remain planned.

## Planned improvements

- Implement distinct computer strategies for the difficulty settings.
- Add stalemate detection, draw handling, and complete capture-sequence tests.
- Add keyboard and touch controls and separate rules from the interface.

## Author

**Javel Swaby** · [GitHub](https://github.com/jfreecodecamp-web)

Part of a portfolio exploring interactive interfaces, state management, and rule-based JavaScript applications.
