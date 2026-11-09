# Tic-Tac-Toe (Blazor WebAssembly)

Classic Tic-Tac-Toe in the browser. Play a friend on the same screen, or play against the computer.

I built it to practise Blazor WebAssembly components and simple game logic: board state, turn handling, and detecting wins and draws.

## Features

- **Two modes:** toggle between two-player and playing the computer
- **Computer opponent:** takes a winning move if it has one, otherwise blocks yours, otherwise plays a random free square
- Detects wins, losses and draws, and highlights the winning line
- Reset button to start a new game

## Run it locally

Requires the [.NET 7 SDK](https://dotnet.microsoft.com/download/dotnet/7.0).

```bash
git clone https://github.com/MohamedAliSalam/TicTacToe-Blazor.git
cd TicTacToe-Blazor
dotnet run
```

Then open the URL printed in the terminal (by default `https://localhost:7174`).

## How it's built

| File | What it does |
|---|---|
| `Components/GameBoardComponent.razor` | Board state, turns, the computer's move choice (`GetWinningMove`, `RandomTurn`), win and draw checks |
| `Pages/Index.razor` | Hosts the game board |
| `wwwroot/css/app.css` | Board styling and the winning-line highlight |

## License

[MIT](LICENSE)
