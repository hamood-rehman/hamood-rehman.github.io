---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

## 10kV SiC switch from stacked 3.3kV SiC MOSFETs

- Three series-stacked 3.3kV MOSFETs, each stage with its own gate driver, active dv/dt control and 12kV-isolated supply. Scalable to higher voltage levels.
- Active dv/dt control mechanism powered from the gate driver’s own supply, so no extra isolated supply is needed.
- Tested upto 6kV DC bus and 50A switching current in continuous operation with voltage imbalance between devices stayed within 300V, against up to 1.5kV with no control at 4kV DC bus. 

<figure>
  <img src="{{ base_path }}/images/research/10kV Switch.png" alt="10 kV SiC switch architecture" style="width: 500%; height: 250%; display: block;">
</figure>


## ‘Impact Factor’ of Parameters Variations on Voltage Balancing

- Series-connected SiC MOSFETs experience dynamic voltage-imbalance.
- A quantitative 'Impact Factor' is proposed to identify parameters that affect the voltage-imbalance.
- Experimental validation conducted with 3.3kV SiC MOSFETs with at 1kV/2kV/3kV/4kV DC bus voltages and 10A/20A/30A/40A switching currents to get high fidelity experimental data.

<figure>
  <img src="{{ base_path }}/images/research/IF.png" alt="Bar chart: share of SHAP attribution to dynamic voltage imbalance." style="width: 500%; height: 250%; display: block;">
</figure>

## Wireless gate-driver power supply for medium-voltage SiC MOSFETs

- 6 W, +15 V / −5 V supply: GaN full-bridge inverter at 2.8 MHz, PCB air-core transformer with a 12.7 mm gap (about 38kV theoretical air insulation), and full-bridge rectifiers.
- Compared four compensation networks (S-S, LCC-S, S/S-CL, LCL-S) on identical hardware while double-pulse testing a 3.3 kV SiC MOSFET at a 2.5 kV bus, measuring coupling capacitance, output stability under dv/dt, and thermal behavior.

<figure>
  <img src="{{ base_path }}/images/research/wpt-gdps-prototype.jpg" alt="Wireless gate-driver power supply prototype:" style="width: 500%; height: 250%; display: block;">
</figure>

## 650 V GaN three-level flying-capacitor inverter building block

*2024–2025*

- Three-phase, 25 kVA, 800 V DC bus inverter built from 650 V GaN devices.
- Implemented single-phase-shift modulation on a TI TMS320F28379D DSP.
- Designed the output LC filter for ripple, THD, and resonance; output-current THD of about 2.6%.

## Automated air-core PCB transformer design

- Multi-objective optimization of air-core PCB transformers with NSGA-III, verified with ANSYS electromagnetic simulation.

## Switched-inductor buck-boost DC–DC converters

*M.S. research, GIK Institute*

- Topology development, efficiency analysis, and control of a switched-inductor buck-boost converter with a low inductance requirement for low-power applications.
- Published in *IET Power Electronics* (2023) and IEEE IECON 2021.
