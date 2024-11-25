# Sudoku Solver  

This project is a Python-based Sudoku solver that employs **Constraint Propagation** and **Optimised Backtracking** using advanced heuristics such as **Minimum Remaining Value (MRV)** and **Least Constraining Value (LCV)** to solve puzzles efficiently.  

![Sudoku Example](images/sudoku.png)


## Features  

- Utilises **Constraint Propagation** to reduce the problem space by eliminating impossible values.  
- Implements **Optimised Backtracking** with MRV and LCV heuristics for efficient exploration.  
- Mimics human-like logical reasoning by prioritising deductions before exploring possibilities.  

## How It Works  

1. **Constraint Propagation**:  
   - Simplifies the puzzle using techniques like Naked Singles and Hidden Singles to narrow down candidate numbers for each cell.  

2. **Optimised Backtracking**:  
   - MRV selects the most constrained cell (with the fewest options) to minimise the branching factor.  
   - LCV orders values in a way that maximises flexibility for subsequent decisions, reducing the likelihood of conflicts.  

## Results  

- Significant performance improvement: Hard Sudoku puzzles were solved in under 1 second compared to 27+ seconds with basic backtracking.  
- Successfully tested on challenging puzzles, demonstrating a marked reduction in search space and computational time.  

## Getting Started  

### Prerequisites  

- Python 3.x  
- Jupyter Notebook (to run the `.ipynb` file)  

### Installation  

1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/sudoku-solver.git
   cd sudoku-solver

2. Install required dependencies:  
   ```bash
   pip install -r requirements.txt

3. Run the Jupyter Notebook:
    ```bash
    jupyter notebook sudoku.ipynb
## Future Work  

- Explore the use of machine learning techniques to predict the most promising search paths.  
- Develop parallel processing methods to explore multiple branches concurrently and improve performance further.  

## References  

- Russell, S.J. and Norvig, P., *Artificial Intelligence: A Modern Approach*.  
- Online Sudoku resources:  
  - [Sudopedia](http://sudopedia.enjoysudoku.com/)  
  - [Sudoku.com](https://sudoku.com/)  

