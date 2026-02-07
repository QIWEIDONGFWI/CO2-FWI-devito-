## 📖 Project Overview
This repository contains a Python implementation of **2D Acoustic Wave Forward Modelling** based on the finite-difference method (FDM). 

As a senior undergraduate student in **Exploration Technology and Engineering (Applied Geophysics)** at the **Ocean University of China (OUC)**, I developed this project to explore high-performance seismic simulation tools widely used in both academia and the industry (e.g., DUG).

The simulation leverages **Devito**, a Domain-Specific Language (DSL) that automatically generates optimized C code for solving partial differential equations (PDEs).

## 🚀 Key Features
- **Physical Model**: A custom 2D velocity model simulating a water layer ($V_p=1.5 km/s$) over a high-velocity sediment layer ($V_p=2.5 km/s$).
- **Source**: Ricker wavelet source injection (f0 = 10Hz).
- **Solver**: Second-order temporal and spatial finite-difference operators solving the acoustic wave equation:
  $$\frac{1}{c^2} \frac{\partial^2 u}{\partial t^2} - \nabla^2 u = 0$$
- **Stability**: Automatic time-step computation satisfying the **CFL (Courant-Friedrichs-Lewy) condition**.

## 🛠️ Usage
### Prerequisites
- Python 3.7+
- Devito
- Matplotlib / Numpy

### Installation
```bash
pip install devito numpy matplotlib
