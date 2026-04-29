# 🚦 Traffic Simulator

A console-based traffic simulation built in Python. Vehicles, intersections, and traffic flow are all modelled and tracked — with full output logged to the console.

## Overview

This project simulates traffic movement through a network of roads and intersections. Rather than relying on a graphical display, all simulation events and statistics are printed to the console and saved to the `outputs/` directory, making it easy to analyse results programmatically.

## Features

- Simulates vehicles moving through a road network modelled as a graph
- Tracks traffic flow, vehicle states, and intersection behaviour
- Outputs simulation results and statistics to the console
- Saves results to the `outputs/` directory for further analysis

## Requirements

- Python 3.8+
- [Jupyter Notebook](https://jupyter.org/) (to run the `.ipynb` file)

### Python Dependencies

```
networkx>=2.6
numpy>=1.21
matplotlib>=3.5
```

## Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/Froskersss/Traffic-simulator.git
   cd Traffic-simulator
   ```

2. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

## Usage

Open and run the Jupyter Notebook:

```bash
jupyter notebook traffic_simulation_improved.ipynb
```

Run all cells from top to bottom. Simulation output will appear in the console/notebook output, and results will be saved to the `outputs/` folder.

## Project Structure

```
Traffic-simulator/
├── traffic_simulation_improved.ipynb   # Main simulation notebook
├── requirements.txt                    # Python dependencies
├── outputs/                            # Simulation results and logs
└── README.md
```

## How It Works

The simulation uses **NetworkX** to model the road network as a directed graph, where nodes represent intersections and edges represent roads. Vehicles are spawned and routed through the network, with their positions and states tracked at each simulation step. **NumPy** is used for numerical computations, and **Matplotlib** is available for any chart generation.

## Notes

- There is no real-time visual output — all tracking is console/text based.
- Outputs are stored in the `outputs/` directory after each run.
