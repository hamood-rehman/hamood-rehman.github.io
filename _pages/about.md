---
permalink: /
title: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I'm a third-year Ph.D. student in Electrical Engineering at the University of Arkansas, Fayetteville, working in the Power Switch Lab at the NSF GRAPES Research Center under the supervision of Dr. Xiaoqing Song. I build medium-voltage SiC switching hardware: active dv/dt control for series-connected SiC MOSFETs, and the isolated gate drivers and auxiliary power supplies that medium-voltage devices need. My current project is a 20 kV SiC switch made from series-stacked 6.5 kV MOSFETs, with the gate driver, isolated supply, and dv/dt control integrated at every stage.

In summer 2026 I was a power electronics intern at Tesla Energy in Palo Alto, CA, on the Power Conversion Hub team. I troubleshot hardware issues on Powerwall 3 at an 800 V DC bus, characterized the thermal and gain behavior of ground-fault circuit interrupter (GFCI) magnetic cores from several vendors across temperature, and built a MATLAB/Simulink tool for efficiency analysis of a split-phase DC–AC inverter using triangular current mode (TCM) control of interleaved T-type legs.

Before my Ph.D., I was a Laboratory Instructor at GIK Institute, Pakistan (2020–2024), where I upgraded the Linear Control Systems and DSP labs with Siemens PLCs and DSP kits. I received my M.S. in Electrical Engineering from GIK Institute in 2019, with a thesis on switched-inductor buck-boost DC–DC converters that was later published in *IET Power Electronics*.

Research interests
======

- **Series-connected SiC MOSFET switches** for 10–20 kV applications such as medium-voltage converters, data-center power, and solid-state circuit breakers
- **Active dv/dt control** for dynamic voltage balancing without snubbers or extra isolated supplies
- **Isolated gate-driver power supplies** with high insulation and low coupling capacitance
- **Measurement-driven sensitivity analysis** that links device parameter spread to switching behavior

SiC devices rated above about 15 kV are still mostly research parts, while 3.3 kV and 6.5 kV MOSFETs are readily available. Stacking them gives a practical high-voltage switch, as long as every device stays within its safe voltage during fast transients. That is the hard part: small mismatches in device parameters, gate drive, layout parasitics, or timing produce large voltage imbalance at SiC switching speeds. More on the [Research]({{ site.baseurl }}/research/) and [Publications]({{ site.baseurl }}/publications/) pages.

News
======

- **2026:** Paper on a 10 kV SiC switch built from voltage-balanced 3.3 kV MOSFETs accepted for oral presentation at IEEE APEC 2027, New Orleans, LA.
- **Summer 2026:** Power electronics intern, Tesla Energy, Palo Alto, CA.
- **2026:** Oral presentation at IEEE APEC 2026, San Antonio, TX, on how device-parameter mismatch drives dynamic voltage imbalance in series-connected SiC MOSFETs.
- **2025:** Paper on matching networks for wireless gate-driver power supplies presented at IEEE ECCE 2025, Philadelphia, PA.
