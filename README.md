# SDR Hardware Abstraction Layer (HAL) Investigation

This repository focuses on investigating whether a Hardware Abstraction Layer (HAL) is needed to integrate an existing Python-based Drone-ID signal processing chain with a different Software Defined Radio (SDR) or SDR control library than the one the original code was built around.

The goal is to assess if introducing a HAL would make integration cleaner, simpler, and more maintainable, or if direct adaptation of the existing code is sufficient.

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

4.
