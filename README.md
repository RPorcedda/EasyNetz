# EasyNetz

EasyNetz is a Python tool for selecting graphs from the Netzschleuder database based on user-defined criteria such as whether they are directed, undirected, weighted, unweighted, and various properties like the number of nodes, edges, and graph density. Once the graphs are filtered according to the criteria, the selected graphs can be downloaded and exported into CSV files for further analysis.

## Parameters Overview
EasyNetz allows the user to filter graphs using a variety of parameters, which are defined in the `args` dictionary. Here's a breakdown of these parameters:

- **directed** (bool): Whether the graphs should be directed (`True`) or undirected (`False`).
- **also_undirected** (bool): If `True`, both directed and undirected graphs will be considered.
- **bipartite** (bool): Whether to include bipartite graphs.
- **also_unipartite** (bool): If `True`, both bipartite and unipartite graphs will be considered.
- **weighted** (bool): If `True`, only weighted graphs are selected.
- **also_unweighted** (bool): If `True`, unweighted graphs will also be included.
- **node_props** (bool): Whether the graph should have node properties.
- **also_no_node_props** (bool): If `True`, graphs without node properties will be considered as well.
- **min_num_nodes** (int): The minimum number of nodes a graph should have.
- **max_num_nodes** (int): The maximum number of nodes a graph can have.
- **min_num_edges** (int): The minimum number of edges a graph should have.
- **max_num_edges** (int): The maximum number of edges a graph can have.
- **min_density** (float): The minimum density of the graph (0 to 1).
- **max_density** (float): The maximum density of the graph (0 to 1).
- **take_max** (bool): If `True`, the graph with the maximum number of nodes will be selected.
- **take_min** (bool): If `True`, the graph with the minimum number of nodes will be selected.
- **ns_info_saved** (bool): Whether the Netzschleuder info file is pre-loaded (`True`) or needs to be downloaded (`False`).
- **access_token** (str): Optional access token for restricted datasets in Netzschleuder.

The tool provides flexibility by allowing users to adjust these parameters to suit specific graph filtering needs.

## Installation

Before running EasyNetz, you need to have the following dependencies installed. These can be installed using the `requirements.txt` file as shown below.

```bash
pip install -r requirements.txt
```

## Running

To run EasyNetz, open bash (or terminal) inside the EasyNetz folder and run the following command:

```bash
python -m main
```