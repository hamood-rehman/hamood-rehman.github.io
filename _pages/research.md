---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

## 10 kV SiC switch from stacked 3.3 kV MOSFETs, scaling to 20 kV

*Ph.D. project: 20 kV High Voltage SiC Switch for Next Generation Energy Conversion and Grid Modernization. Paper accepted for oral presentation at IEEE APEC 2027.*

- Three Wolfspeed 3.3 kV / 52 A SiC MOSFETs in series, with signal, power, and control integrated at every stage. Each device has its own board with a gate driver, V<sub>DS</sub> sensing, a local dv/dt controller, and a two-stage, multichannel isolated auxiliary supply rated for 12 kV insulation. The boards stack modularly, so blocking voltage scales with the number of stages and the isolation rating of the supply.
- **Voltage balancing:** a low-voltage NPN BJT in each MOSFET's Kelvin-source path acts as a voltage-controlled resistor during the turn-off Miller plateau. V<sub>DS</sub> is sampled and held on every pulse, and a PI loop sets the BJT base drive to slow or speed that device's turn-off dv/dt on the next pulse. Because the BJT emitter sits at the MOSFET source, the controller shares the gate driver's rail, so no additional isolated supply is needed per device.
- **Status:** the 10 kV-rated prototype is built, and the balancing method has been validated experimentally on it at reduced bus voltage. The 20 kV version is the current design effort, using 6.5 kV-class devices and a single-stage, multichannel RF-switched auxiliary supply with 20 kV isolation. It has not yet been built or tested.

<figure>
  <img src="{{ base_path }}/images/research/stacked-switch.svg" alt="Block diagram of the series-stacked SiC switch and its per-stage voltage-balancing loop">
  <figcaption>Architecture of the stacked switch (left) and the dv/dt balancing loop on each stage (right).</figcaption>
</figure>

## Which device mismatches actually cause voltage imbalance?

*IEEE APEC 2026, oral presentation*

- Characterized five Wolfspeed 3.3 kV SiC MOSFETs (V<sub>th</sub>, g<sub>m</sub>, C<sub>gs</sub>, C<sub>gd</sub>, C<sub>ds</sub>) and recorded 448 double-pulse measurements on series-connected pairs from 1 to 4 kV and 10 to 40 A, across device-position and gate-driver configurations.
- Fit a Gaussian-process surrogate to the measurements (test R² ≈ 0.95), then used Sobol indices and SHAP values to separate individual effects from interactions.
- **Result:** imbalance is driven mainly by interactions between mismatches rather than by any single one. C<sub>gs</sub> and V<sub>th</sub> mismatch carry roughly 50% and 30% of the SHAP attribution, and g<sub>m</sub> mismatch was negligible under the tested conditions. The practical takeaway is to screen devices for series stacks on C<sub>gs</sub> and V<sub>th</sub> first.

<figure>
  <img src="{{ base_path }}/images/research/shap-attribution.svg" alt="Bar chart: share of SHAP attribution to dynamic voltage imbalance. Cgs mismatch about 50 percent, Vth about 30 percent, Cgd about 13 percent, Cds about 7 percent, gm negligible.">
</figure>

## Wireless gate-driver power supply for medium-voltage SiC MOSFETs

*IEEE ECCE 2025*

- 6 W, +15 V / −5 V supply: GaN full-bridge inverter at 2.8 MHz, PCB air-core transformer with a 12.7 mm gap (about 38 kV theoretical air insulation), and full-bridge rectifiers.
- Compared four compensation networks (S-S, LCC-S, S/S-CL, LCL-S) on identical hardware while double-pulse testing a 3.3 kV SiC MOSFET at a 2.5 kV bus, measuring coupling capacitance, output stability under dv/dt, and thermal behavior.
- **Result:** the matching network and rectifier, not only the transformer gap and insulation, change coupling capacitance and common-mode immunity. Networks with fewer reactive elements held up better under high dv/dt.

<figure>
  <img src="{{ base_path }}/images/research/wpt-gdps-prototype.jpg" alt="Wireless gate-driver power supply prototype: GaN H-bridge, fixture for resonant networks, 128 by 116 mm PCB air-core transformer with 12.7 mm gap, and -5 V and +15 V rectifier outputs">
  <figcaption>Prototype: GaN H-bridge, fixture for the resonant networks, PCB air-core transformer, and the −5 V / +15 V rectifier outputs.</figcaption>
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
