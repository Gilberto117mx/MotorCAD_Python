# Motor-CAD Python Automation

A Python-based automation workflow for Motor-CAD analysis and thermal simulation.

## Contents

- **motorcad_automation_workflow.ipynb** - Jupyter notebook with Motor-CAD automation scripts
- **Gen8_3pp.mot** - Motor-CAD design file
- **Gen8_3pp.txt** - Motor-CAD configuration/data export

## Overview

This project automates Motor-CAD workflows using Python, including:
- Motor design analysis
- Thermal simulation and calculations
- Electromagnetic performance analysis
- Data processing and visualization

## Analyses Performed

- **Lab Model Build** - Constructs electromagnetic and loss models with configurable saturation methods
- **Heat Balance Analysis** - Thermal analysis with losses and dissipation calculations
- **Efficiency Map** - Complete efficiency mapping across speed and current ranges
- **Peak Operation** - Electromagnetic analysis at peak performance conditions
- **Continuous Operation** - Steady-state thermal and mechanical performance
- **Transient Operation** - Dynamic thermal analysis over specified time periods

## Generated Graphs

### Heat Balance Analysis
- `heat_balance.png` - Stacked bar chart of losses vs dissipation
- `axial_temperatures.png` - Axial temperature distribution
- `radial_temperatures.png` - Radial temperature distribution

### Peak Performance
- `peak_performance.png` - Torque and power curves
- `peak_performance_torque_power.png` - Combined torque/power graph

### Continuous Performance
- `continuous_performance.png` - Torque and power vs speed
- `continuous_max_temperatures.png` - Magnet and winding max temperatures
- `continuous_performance_torque_power.png` - Combined torque/power graph

### Efficiency Map
- `efficiency_map.png` - 2D efficiency contour map

### Transient Performance
- `transient{duration}s_performance.png` - Transient torque and power
- `transient{duration}s_max_temperatures.png` - Transient magnet and winding temperatures
- `transient_{duration}s_torque_power.png` - Combined transient torque/power

## Requirements

- Python 3.x
- Motor-CAD 2023.2+
- Jupyter Notebook
- NumPy, SciPy, Matplotlib, Seaborn

## Usage

Open `motorcad_automation_workflow.ipynb` in Jupyter Notebook and modify the analysis flags in the "VARIABLE DEFINITION" section to enable/disable specific analyses, then run the cells to execute the automation workflow.
