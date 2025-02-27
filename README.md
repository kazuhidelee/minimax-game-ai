# 🎮 Minimax AI for Tic-Tac-Toe & Connect 4

This repository contains an AI implementation for Tic-Tac-Toe (TTT) and Connect 4 (C4) using the Minimax algorithm with Alpha-Beta pruning.

## 📂 Project Structure

- `Agent.py` – Implements the Minimax algorithm with αβ pruning.
- `Game.py` – Handles game execution and AI vs. human interactions.
- `TTT.py` – Implements Tic-Tac-Toe game logic.
- `Connect4.py` – Implements Connect 4 game logic with a graphical display.

## 🚀 Getting Started

### 1️⃣ Setup Environment  
Create a virtual environment and install dependencies:

```bash
python -m venv venv  
source venv/bin/activate  # On Windows use `venv\Scripts\activate`  
python -m pip install -r requirements.txt  
```

### 2️⃣ Running the Agent  
To play Tic-Tac-Toe:

```bash
python Game.py TTT.py  
```
To play Connect 4:

```bash
python Game.py Connect4.py  
```

## 🔍 Search Algorithms
The AI evaluates moves using Minimax with Alpha-Beta pruning to optimize performance. Key considerations:
- Winning in the fewest moves is prioritized.
- Losing in the most moves is chosen if unavoidable.
- Heuristic function assigns scores based on board evaluation.
  
| Function | Description |
|-----------|------------|
| minimax(board, depth, maximizingPlayer, alpha, beta) | Implements Minimax with Alpha-Beta pruning. |
| get_valid_moves(board) | Returns valid moves. |
| play_move(board, move, player) | Simulates a move. |
| heuristic_value(board, player) | Evaluates the board. |
| is_winner(board, player) | Checks if a player has won. |
| is_full(board) | Checks if the board is full. |

## 📝 Notes

- Tic-Tac-Toe runs in the terminal.
- Connect 4 has a graphical interface for better visualization.
- The AI can be tested with predefined moves by modifying turn in Game.py.


