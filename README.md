# Louvain-Enhanced

This package has some functions taken from [python-louvain](https://github.com/taynaud/python-louvain) package

Louvain-Enhanced is a Python package for community detection in large networks using the Louvain method. This package provides enhanced functionalities and optimizations for efficient and accurate community detection.

## Features

- Efficient implementation of the Louvain method for community detection.
- Support for weighted and unweighted graphs.
- Easy integration with NetworkX.
- Randomized node evaluation for different partitions at each call.
- Modular and extensible design.

## Installation

You can install [Louvain-Enhanced](https://pypi.org/project/louvain-enhanced/) using pip:

```bash
pip install louvain-enhanced
```
## Usage

### Importing the Package
```python
import networkx as nx
```
```python
from louvain_enhanced import (
    get_partition_at_level,
    calculate_modularity,
    find_best_partition,
    create_dendrogram,
    create_induced_graph,
    load_binary_graph,
)
```

### Creating a Graph
```python
G = nx.karate_club_graph()
```

### Finding the Best Partition
```python
partition = find_best_partition(G)
print(partition)
```

### Calculating Modularity
```python
modularity = calculate_modularity(partition, G)
print(f"Modularity: {modularity}")
```

### Creating a Dendrogram
```python
dendrogram = create_dendrogram(G)
print(dendrogram)
```

### Getting Partition at a Specific Level
```python
level = 1
partition_at_level = get_partition_at_level(dendrogram, level)
print(partition_at_level)
```

### Creating an Induced Graph
```python
induced_graph = create_induced_graph(partition, G)
print(induced_graph)
```

### Loading a Binary Graph
```python
binary_graph = load_binary_graph("path_to_binary_file")
print(binary_graph)
```

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Author
[Himangshu Singh](https://github.com/himangshusingh)