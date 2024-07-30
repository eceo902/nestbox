# Nestbox

Nestbox is a networked consensus coordinate system alignment tool. It provides a framework for aligning and optimizing multiple coordinate systems based on shared measurements and observations.

## Overview

Nestbox is designed to solve the problem of aligning multiple coordinate systems in a distributed environment. It's particularly useful in scenarios where different sensors or systems are observing the same features but from different perspectives or with different levels of uncertainty.

### Key Components

1. **Aligner**: The core optimization engine that aligns multiple coordinate systems based on shared observations.

2. **Coordinate Systems**: Representations of different frames of reference, each with its own origin and orientation.

3. **Measurements**: Data points observed by the observers, including position and uncertainty information.

4. **Features**: Identifiable points or objects in space that can be observed across multiple coordinate systems.

5. **Daemon**: A background process that manages the alignment process and handles communication between different parts of the system.

6. **API**: Interfaces for interacting with the Nestbox system, allowing for the creation of coordinate systems, addition of measurements, and retrieval of alignment results.

7. **Visualizer**: A 3D visualization tool for displaying the state of the coordinate systems and their alignment.

8. **Simulator**: A lightweight toolkit for creating mock uncertain measurement data for testing, including an *Environment* and different types of *Observers* like cameras or 3D trackers.


## Conceptual Workflow

1. Create multiple coordinate systems, each representing a different frame of reference.
2. Define features in the environment that can be observed by multiple coordinate systems.
3. Feed measurements of shared features into the system, including position and uncertainty information.
4. The aligner optimizes the relative positions and orientations of the coordinate systems to best fit all observations.
5. Visualize the results to see how the different coordinate systems align.

## Project Structure

- `python/`: Contains the core Python implementation of Nestbox.
- `csharp/`: C# implementation for cross-platform support.
- `protos/`: Protocol buffer definitions for data structures.
- `visualizer/`: 3D visualization tools for displaying alignment results.
- `docs/`: Documentation and notes.

## Current State

Nestbox is currently in development. The core concepts and structure are in place, but the system is not yet ready for production use. The optimization algorithms, API, and visualization capabilities are being refined and expanded.

## Contributing

As Nestbox is still in active development, we welcome contributions and feedback. Please feel free to open issues for bugs or feature requests. 
