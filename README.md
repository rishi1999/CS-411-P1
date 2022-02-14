# CS 411: Artificial Intelligence I
## Project 1: Sudoku

### initialize_domains()
Initialize domains for all cells to be used in consistency checking. Return domains and domain sizes.

### read_data(filename)
Read input data from file `filename` and perform consistency check on it. Return input board, updated domains, and updated domain sizes.

### board_str(board)
Return string representation of board `board`.

### write_data(filename, board)
Write string representation of board `board` to file `filename`.

### consistency_check(domains, dom_sizes, i, j, k)
Perform consistency check for board with domains `domains` and domain sizes `dom_sizes` after having value `k` entered in cell (`i`,`j`). Return updated domains, updated domain_sizes, and consistency flag.

### backtrack(cell_id, board, domains, dom_sizes)
Use backtrack search to find a value for cell `cell_id` (numbered left to right then top to bottom) in board `board` with domains `domains` and domain sizes `dom_sizes`. Return consistency flag, updated board, updated domains, and updated domain sizes.

### solve(board, domains, dom_sizes)
Execute backtrack search to solve board `board` with domains `domains` and domain sizes `dom_sizes` and print solved board. Return flag indicating if puzzle was solved and solved board if puzzle was solvable.