# DACTA — Differentially-Asymmetric Calorimetric Thermal Anemometer

**Custom PCB Design | Simulation | Hardware Development | Experimental Validation**

## 1. Project Overview

The system employs a central heating element and two temperature sensors (T1 and T2) positioned asymmetrically around the heater. Airflow modifies the thermal distribution across the sensing region, producing a differential temperature response that can be used to characterize airflow. The project encompasses the complete engineering development process, from theoretical investigation and circuit simulation to PCB design, hardware implementation and experimental validation.

This repository contains the technical documentation, design files, simulation results, experimental datasets and development records generated throughout the project.

## 2. Operating Principle

The anemometer operates on the calorimetric principle of thermal transport. A heating element generates a localized thermal field within the airflow channel. In the absence of airflow, the temperature distribution around the heater is approximately symmetric. When airflow is introduced, convective heat transfer modifies this distribution, creating a temperature difference between the two sensing elements. The differential temperature response is therefore related to the magnitude and direction of airflow.

The system incorporates:

- A central heating element for generating the thermal field.
- An NTC Thermistor Ta to measure ambient temperature, and another NTC Ts for monitoring thermal distribution from the heater.
- Electronic circuitry for heater control (operating in constant temperature mode) and temperature measurement.
- A data acquisition system for processing and recording sensor outputs.

## 3. System Architecture

Read it as: |        Subsystem       |                      Function                      |

- |     Heating element    |            Generates the thermal field             |
- |   Temperature sensors  | Measure upstream and downstream thermal variations |
- | Heater control circuit |            Regulates heater operation              |
- |   Signal conditioning  |    Interfaces with temperature sensing elements    |
- |     Data acquisition   |      Acquires and processes sensor measurements    |

## 4. Hardware Development

A custom PCB was designed to integrate the sensing, heating, control and measurement electronics.

Hardware development includes:

- The Sensor Head: Heater drive and temperature regulation circuitry.
- Dual temperature sensing channels.
- Analogue Front-End: Signal conditioning using acquisition to an ADC.
- PCB schematic capture, layout and fabrication.

Particular attention was given to the physical placement of the heater and sensing elements to minimise unwanted thermal coupling with the main electronics.

## 5. Simulation and Design Validation

Circuit-level simulations were conducted during the design process to investigate circuit behavior and validate key electrical characteristics before hardware implementation. This was done on COMSOL© to ensure a good state of accuracy.

Simulation records include:

- Heater control circuit behaviour.
- Temperature sensing and signal conditioning.
- Analogue circuit response.
- Power supply and voltage regulation.
- Design verification and iterative improvements (multiple, in fact).

## 6. Experimental Validation

The fabricated PCB is evaluated through experimental testing to investigate the relationship between airflow and the differential thermal response. This was cross calibrated using an Industrial anemometer, the Wika A2G-20.

Experimental investigations include:

- Heater temperature regulation & iterative reworking.
- Temperature sensor response.
- Airflow-dependent sensor behaviour.
- System stability and repeatability.
- Comparison between simulated and experimental performance.

Experimental datasets, measurement records, photographs and analysis are maintained within this repository.

## 7. Repository Contents

This repository serves as a comprehensive engineering record of the project, covering the development process from initial design to hardware validation.

It includes:

- Theoretical background and design calculations.
- Electronic schematics and PCB design files.
- Component specifications and datasheets.
- Circuit simulation files and results.
- Firmware and data acquisition code.
- Experimental procedures and raw datasets.
- Data processing, analysis and visualisation.
- Hardware photographs and validation records.

## 8. Tools and Technologies

Read it as: |      Tool / Technology     |                   Application                  |

- |       Altium Designer      |         Schematic capture and PCB design       |
- |          LTspice           |                Circuit simulation              |
- |        Arduino Mega        |     Embedded control and data acquisition      |
- |           Python           | Experimental data processing and visualisation |
- |          SPI         |              Peripheral communication          |

## 9. Project Status

[Hardware development and experimental validation.]

The repository is maintained as a continuously updated record of the design iterations, simulation studies, hardware implementation and experimental findings.

## 10. Author

Arsh Malik | M.Sc. in EEE, Sensor Systems Engineering  
Imperial College London
