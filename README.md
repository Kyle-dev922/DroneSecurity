# SDR Integration & Real-Time Drone-ID Visualization

This repository investigates two core aspects of enhancing the Drone-ID signal processing system:

1. Whether implementing a Hardware Abstraction Layer (HAL) is necessary to integrate the existing Python-based Drone-ID signal processing chain with different Software Defined Radio (SDR) hardware or control libraries.

2. The development of a Graphical User Interface (GUI) or application to wrap the reference code and Cyrus’ work, allowing the system to be showcased as a real-time demonstration of signal capture, decoding, and GPS visualization.

The aim is to make SDR integration cleaner and more maintainable while providing an interactive front-end for real-time data presentation.


## Reference Material

The open-source project can be found at [Drone-ID Receiver for DJI OcuSync 2.0](https://github.com/RUB-SysSec/DroneSecurity). This project not only provides a thorough explanation of the underlying theory and methodology but also includes the complete python signal processing code.

## Objectives

Primary Goal

Determine whether implementing a Hardware Abstraction Layer (HAL) is necessary and beneficial for integrating the existing Python-based processing chain with multiple SDR control libraries or hardware platforms.

1. Understand the Existing Processing Chain

   * Review how the current Python code interfaces with its SDR source.
   * Identify which parts of the code are tightly coupled to the original SDR implementation.

2. Study the Target SDR / Control Library

   * Examine how the new SDR handles initialization, data streaming, and sample formats.
   * Identify key differences in API calls, data structures, or performance characteristics compared to the original SDR.
  
3. Assess Compatibility and Integration Options

   * Determine whether the new SDR can be integrated by simply adapting the current code.
   * If major restructuring would be required, evaluate whether a HAL could simplify or future-proof the integration.

# Secondary Goal — Real-Time Demonstration GUI

Develop a Graphical User Interface (GUI) or standalone application to wrap the reference Drone-ID processing code and Cyrus’ enhancements, enabling the project to function as a live demonstration tool.

The GUI will include three key visualization components:

1. Raw Capture (Frequency Domain): Display real-time spectrum data directly from the SDR input.

2. Unpackaged Data: Visualize decoded Drone-ID data using the existing Python processing chain.

3. GPS Data Visualization: Present extracted GPS coordinates on an interactive globe or map interface.
