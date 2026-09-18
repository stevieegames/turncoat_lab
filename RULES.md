# Turncoat — Laboratory Ruleset

Rules for prototype **0.9**.

## 1. Players and components

Turncoat is played by two players: **Ivory** and **Chestnut**.

Each player begins with:

- 3 Cubes
- 2 Wedges
- 1 Main Piece
- 4 No Go areas by default; this quantity is configurable before restarting

The normal board is 6 rows by 5 columns. A red boundary surrounds it and counts as permanently occupied for surrounding purposes. If Gullies are enabled, ten marked boundary locations become ordinary playable tiles.

## 2. Starting position

Chestnut begins at the top of the board and Ivory begins at the bottom. The layouts mirror one another.

From each player's nearest edge, their two ranks are:

| Rank | Column 2 | Column 3 | Column 4 |
|---|---|---|---|
| Nearest edge | Wedge | Cube | Wedge |
| Next rank | Cube | Main Piece | Cube |

Ivory takes the first turn with 2 Tempo. Chestnut begins with 1 Tempo.

## 3. Tempo and passing

There are 3 Tempo in total. Spending Tempo transfers it to the opponent.

| Action | Cost |
|---|---:|
| Move a piece | 1 Tempo |
| Turncoat a piece | 1 Tempo |
| Place a No Go area | 2 Tempo |

A player cannot pass before acting:

- If the turn began with 1 or 2 Tempo, spend at least 1 Tempo.
- If the turn began with 3 Tempo, spend at least 2 Tempo.
- Placing one No Go area spends 2 Tempo, so it satisfies the second requirement by itself.

Select **PASS** to end the turn once the requirement is met.

## 4. Movement

A piece must finish on an unoccupied playable tile.

- **Cube:** moves 1 tile horizontally, vertically, or diagonally.
- **Main Piece:** moves 1 tile horizontally, vertically, or diagonally.
- **Wedge:** moves along a path of up to 3 connected tiles in any horizontal, vertical, or diagonal directions. It may change direction between steps and may jump over occupied tiles, but its landing tile must be unoccupied.

Red boundary locations that are not open Gullies cannot be entered.

## 5. No Go areas

Spend 2 Tempo to place one of your remaining No Go areas on any unoccupied playable tile.

A No Go area:

- Never moves for the rest of the game
- Cannot be entered by a piece
- Counts as occupied when checking surrounds
- Has no owner for turncoating or victory requirements

## 6. Turncoating

Spend 1 Tempo to convert an eligible enemy Cube or Wedge to your colour. The Main Piece cannot be turncoated.

A surrounding location can contain any piece, a No Go area, or a closed red boundary tile. At least one required location must contain one of the attacking player's actual pieces.

### Cube formations

A Cube can be turncoated when either of these complete four-location squares surrounds it:

- North, South, East, and West
- Northeast, Northwest, Southeast, and Southwest

### Wedge formations

A Wedge can be turncoated when any one of these complete three-location triangles surrounds it:

- Northeast, Southeast, and West
- North, Southwest, and Southeast
- Northwest, Southwest, and East
- South, Northwest, and Northeast

### Blue shield

A turncoated piece receives a blue shield. The opponent cannot turncoat that piece during their immediately following turn. At the start of the piece owner's next turn, the shield cracks and fades away.

## 7. Winning and forfeiting

The eight locations around a Main Piece form its surrounding area. A location counts as filled if it contains:

- An Ivory piece
- A Chestnut piece
- A No Go area
- A closed red boundary tile

To win by surrounding the opponent's Main Piece:

1. All eight surrounding locations must be filled.
2. At least one of those locations must contain one of your own pieces.
3. You must have at least 1 Tempo remaining, which is spent to complete the win.

If your action surrounds your own Main Piece entirely with your own pieces, you immediately forfeit.

## 8. Gullies

Gullies are an optional setting. When enabled, ten specific locations in the red boundary become open tiles: three across the top, three across the bottom, and two on each side.

An open Gully behaves like any other playable tile. It can be entered, can hold a piece or No Go area, and participates normally in surrounding formations. No additional outer boundary is added around Gullies in this prototype.

