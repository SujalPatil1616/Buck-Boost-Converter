# DC-DC Buck-Boost Converter Simulation using LTspice

## Overview

This project demonstrates the design and simulation of an Inverting DC-DC Buck-Boost Converter using LTspice. A Buck-Boost Converter is capable of both increasing (boosting) and decreasing (bucking) the magnitude of the input voltage while also reversing its polarity. The circuit uses PWM-controlled switching, an inductor, diode, capacitor, and load resistor to generate a regulated negative output voltage from a positive input supply.

---

## Components Used

- Input Voltage Source (V1)
- PWM Pulse Generator (V2)
- MOSFET (RSL020P03)
- NPN Transistor (2N2222)
- Schottky Diode (1N5817)
- Inductor (100 µH)
- Capacitor (100 µF)
- Load Resistor (40 Ω)

---

## Case 1: Input Voltage = 3V

### Circuit Diagram

<img src="https://github.com/SujalPatil1616/Buck-Boost-Converter/blob/main/Case1%20circuit%20diagram.png" alt="Buck Boost Converter Circuit Case 1" width="700"/>

### Output Waveform

<img src="https://github.com/SujalPatil1616/Buck-Boost-Converter/blob/main/case1%20waveform.png" alt="Buck Boost Converter Waveform Case 1" width="700"/>

### Observation

- Input voltage was set to 3V.
- The converter produced an output voltage of approximately **-6.8V**.
- Since the magnitude of the output voltage is greater than the input voltage, the circuit operated in **Boost Mode**.
- The negative sign indicates that the output polarity is inverted with respect to the input.
- The output waveform gradually settled to a stable negative voltage after a short transient period.

---

## Case 2: Input Voltage = 10V

### Circuit Diagram

<img src="https://github.com/SujalPatil1616/Buck-Boost-Converter/blob/main/Case2%20circuit%20diagram.png" alt="Buck Boost Converter Circuit Case 2" width="700"/>

### Output Waveform

<img src="buck_boost_waveform_case2.png" alt="Buck Boost Converter Waveform Case 2" width="700"/>

### Observation

- Input voltage was set to 10V.
- The converter produced an output voltage of approximately **-5.4V**.
- Since the magnitude of the output voltage is lower than the input voltage, the circuit operated in **Buck Mode**.
- The output voltage remained negative, confirming the inverting nature of the Buck-Boost Converter.
- The waveform reached a stable output value after the initial transient response.

---

## Working Principle

The Buck-Boost Converter operates by repeatedly storing and releasing energy through the inductor. When the MOSFET is switched ON, energy is stored in the magnetic field of the inductor. When the MOSFET is switched OFF, the stored energy is transferred through the diode to the output capacitor and load. By adjusting the PWM duty cycle, the converter can either increase or decrease the output voltage. In the inverting configuration, the output voltage polarity becomes opposite to the input voltage, enabling the generation of negative output voltages from positive input supplies.

---

## Simulation Results

| Input Voltage (Vin) | Output Voltage (Vout) | Operation |
|---------------------|----------------------|-----------|
| 3 V | -6.8 V | Boost + Inverting |
| 10 V | -5.4 V | Buck + Inverting |

---

## Conclusion

The LTspice simulation successfully demonstrates the operation of an Inverting Buck-Boost Converter under two different input conditions. For an input voltage of 3V, the converter generated an output voltage of approximately -6.8V, showing its ability to increase the voltage magnitude while reversing the polarity. For an input voltage of 10V, the converter produced an output voltage of approximately -5.4V, demonstrating voltage step-down operation with negative polarity. These results verify that the Buck-Boost Converter can operate in both Buck and Boost modes while providing an inverted output voltage.

---

## Applications

- Battery-Powered Electronics
- Embedded Systems
- Portable Devices
- Renewable Energy Systems
- Power Supply Design
- Negative Voltage Generation Circuits
- Sensor Interface Circuits
- Industrial Control Systems

---

## Software Used

- LTspice XVII / LTspice 26

---

## Author

**Sujal Patil**  
B.Tech Electronics and Communication Engineering
