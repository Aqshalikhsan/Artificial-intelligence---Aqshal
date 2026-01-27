# Artificial Intelligence - Aqshal

This repository contains AI and Machine Learning implementations, algorithms, and experiments.

## Author
- **Aqshal Ikhsan**
- Email: aksalikhsan@gmail.com

## Contents

### Main Module (`AI`)
Core AI module providing:
- **Search Algorithms**: BFS, DFS, A*
- **Machine Learning Utilities**: Train/test split, normalization, standardization
- **Data Processing**: CSV loading, missing value handling, categorical encoding

### Notebooks
- `Sistem_Cerdas.ipynb`: Intelligent systems concepts and implementations
- `Sistem_Cerdas_2.ipynb`: Advanced AI topics including informed search

## Installation

```bash
# Install dependencies
pip install -r requirements.txt
```

## Usage

### Running the Main Module

```bash
# Make executable
chmod +x AI

# Run demonstrations
python3 AI
```

### Importing in Python

```python
from AI import SearchAlgorithms, MachineLearning, DataProcessor

# Use BFS
graph = {'A': ['B', 'C'], 'B': ['D'], 'C': ['D'], 'D': []}
path = SearchAlgorithms.bfs(graph, 'A', 'D')
print(path)  # ['A', 'B', 'D']

# Split data
X_train, X_test, y_train, y_test = MachineLearning.train_test_split(X, y)

# Process data
df = DataProcessor.load_csv('data.csv')
df_clean = DataProcessor.handle_missing_values(df)
```

## Features

### Search Algorithms
- **Breadth-First Search (BFS)**: Uninformed search, guaranteed shortest path
- **Depth-First Search (DFS)**: Uninformed search, memory efficient
- **A* Search**: Informed search using heuristics, optimal with admissible heuristic

### Machine Learning
- Train/test split with random state support
- Feature normalization (min-max scaling)
- Feature standardization (z-score)

### Data Processing
- CSV file loading
- Missing value handling (mean, median, drop)
- Categorical variable encoding (one-hot)

## Examples

See the notebooks for detailed examples and tutorials:
- Search strategies and problem-solving
- Machine learning algorithms
- Data preprocessing techniques

## License

MIT License

## Contributing

Feel free to open issues or submit pull requests for improvements.
