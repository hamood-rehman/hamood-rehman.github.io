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

## Wireless gate-driver power supply for medium-voltage SiC MOSFETs

- 6 W, +15 V / −5 V supply: GaN full-bridge inverter at 2.8 MHz, PCB air-core transformer with a 12.7 mm gap (about 38kV theoretical air insulation), and full-bridge rectifiers.
- Compared four compensation networks (S-S, LCC-S, S/S-CL, LCL-S) on identical hardware while double-pulse testing a 3.3 kV SiC MOSFET at a 2.5 kV bus, measuring coupling capacitance, output stability under dv/dt, and thermal behavior.

<figure>
  <img src="{{ base_path }}/images/research/wpt-gdps-prototype.jpg" alt="Wireless gate-driver power supply prototype" style="width: 100%; height: auto; display: block;">
</figure>

## BJT-based active dv/dt control 

-  A low-voltage NPN BJT is inserted into the MOSFET’s Kelvin source path, and its conduction is actively controlled by a closed-loop PI controller, modulating its equivalent on-state resistance.
-  Controls gate-current in the SiC gate-source discharge path during turn-off.

<figure>
  <img src="{{ base_path }}/images/research/npn.png" alt="BJT based dv/dt control" style="width: 100%; height: auto; display: block;">
</figure>

## ‘Impact Factor’ of parameters variations on voltage-balancing

- Series-connected SiC MOSFETs experience dynamic voltage-imbalance.
- A quantitative 'Impact Factor' is proposed to identify parameters that affect the voltage-imbalance.
- Experimental validation conducted with 3.3kV SiC MOSFETs with at 1kV/2kV/3kV/4kV DC bus voltages and 10A/20A/30A/40A switching currents to get high fidelity experimental data.

<figure>
  <img src="{{ base_path }}/images/research/IF.png" alt="Bar chart: share of SHAP attribution to dynamic voltage imbalance." style="width: 1000%; height: 800%; display: block;">
</figure>

