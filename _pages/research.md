---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

## 10kV SiC switch from stacked 3.3kV SiC MOSFETs

- **Three series-stacked 3.3kV MOSFETs, each stage with its own gate driver, active dv/dt control and 12kV-isolated supply. Scalable to higher voltage levels.
- **Active dv/dt control mechanism powered from the gate driver’s own supply, so no extra isolated supply is needed.
- **Tested upto 6kV and 50A in continuous operation with voltage spread between devices stayed within 300V, against up to 1.5kV with no control at 4 kV. 

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
