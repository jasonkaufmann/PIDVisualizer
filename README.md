# PID Visualizer in Unity

The PID Visualizer is a Unity-based tool that graphically represents the response of a system controlled by a Proportional-Integral-Derivative (PID) controller. The Graph Controller script dynamically plots the system's response over time, providing clear visual feedback on the effect of PID tuning.

## Features

- **Real-time Visualization:** Observes the system's response in real-time as the PID values are adjusted.
- **PID Input Fields:** Easily modify proportional (P), integral (I), and derivative (D) values through the Unity Editor or runtime UI.
- **Scalable Data Points:** Adjust the number of points for finer or coarser graph detail.
- **Flexible Visualization:** Can be used to visualize any system that can be controlled by PID, such as motors, heaters, or other automated responses.

## Getting Started

### Prerequisites

- Unity (Version 2020.3 or later recommended).
- TextMeshPro package for displaying PID values.

### Installation

1. Import the Graph Controller script into your Unity project's `Scripts` directory.
2. Attach the Graph Controller script to a new GameObject in your scene.
3. Add a `LineRenderer` component to the same GameObject to draw the graph line.
4. Create UI elements using TextMeshPro and link them to the script to represent the P, I, and D values.

### Configuration

- Set up your target system GameObject and assign it to the `targetPosition` field of the Graph Controller.
- Configure the `numPoints` to determine how many data points you want to plot on the graph.
- The `incrementX` variable controls the spacing between each point along the X-axis.

## Usage

Once everything is set up, enter Play mode in Unity. Adjust the PID values through the linked TextMeshPro UI elements and observe the system's response on the graph. The visualizer will plot the performance of the system, providing instant feedback on the PID tuning.

## Customization

- Adjust the `LineRenderer` settings such as color, width, and material to match the desired aesthetic for the graph.
- Modify the script to accept input from different sources or to represent different types of data.

## Contributing

Your contributions are welcome! If you'd like to contribute to the PID Visualizer, please fork the repository, make your changes, and submit a pull request for review.

## License

This project is open-source and available under the MIT License. See the [LICENSE](LICENSE.md) file for more information.
