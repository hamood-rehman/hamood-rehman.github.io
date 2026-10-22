---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* **Ph.D. in Electrical Engineering**, University of Arkansas, Fayetteville, 2024–present
  * Advisor: Dr. Xiaoqing Song. GPA 4.0/4.0
  * Research focus: medium-voltage SiC MOSFET-based switches and integrated power converters
* **M.S. in Electrical Engineering**, GIK Institute, Pakistan, 2017–2019
  * Thesis: *Switched-Inductor Type Optimum Efficient DC-DC Buck-Boost Converter: Topology, Efficiency Analysis, and Control*

Experience
======
* **Graduate Researcher**, Power Switch Lab, NSF GRAPES Research Center, University of Arkansas, 2024–present
  * Designed and built a signal-, power-, and control-integrated 10 kV SiC switch from three series-connected 3.3 kV SiC MOSFETs
  * Developed a two-stage, multichannel isolated auxiliary power supply with 12 kV insulation capability
  * Proposed and experimentally validated a dv/dt control technique using a low-voltage BJT as a variable resistor in the Kelvin-source path, for voltage balancing in series-connected SiC MOSFETs
  * Quantified the impact of device- and circuit-level parameter variation on dynamic voltage balancing using machine-learning-assisted sensitivity analysis
  * Currently scaling the design to a 20 kV switch with 6.5 kV SiC MOSFETs and a single-stage, multichannel RF-switched auxiliary supply with 20 kV isolation
  * Earlier project (2024–2025): 650 V GaN three-level flying-capacitor inverter building block. Developed single-phase-shift modulation for the three-phase inverter on a TI TMS320F28379D DSP and designed the output LC filter with ripple, THD, and resonance considerations
* **Power Electronics Intern**, Tesla Energy, Palo Alto, CA, Summer 2026
  * Power Conversion Hub team
  * Troubleshot hardware issues on Powerwall 3 at an 800 V DC bus
  * Characterized the thermal and gain behavior of GFCI magnetic cores from several vendors across temperature
  * Built a MATLAB/Simulink tool for efficiency analysis of a split-phase DC–AC inverter using triangular current mode (TCM) control of interleaved T-type legs
* **Laboratory Instructor**, GIK Institute, Pakistan, 2020–2024
  * Upgraded the Linear Control Systems and DSP labs with Siemens S7-1214C PLCs and OMAP-L138 DSP kits; redesigned lab manuals, trainer boards, and instructional material

Skills
======
* **Power hardware:** power stages, custom SiC/GaN gate drivers, isolated gate-driver and auxiliary power supplies, PCB magnetics, multilayer high-voltage PCB layout for low parasitics and EMC
* **Test and characterization:** double- and multi-pulse testing, static and dynamic characterization of wide-bandgap devices (Keysight B1505A), impedance analysis (Keysight E4990A), Tektronix MSO5 series oscilloscopes
* **Simulation and design:** LTspice, PSpice, PLECS, MATLAB/Simulink, ANSYS Maxwell, Q3D, HFSS and Simplorer, Altium Designer, SolidWorks
* **Control and embedded:** PI/PID design for current- and voltage-mode control, digital PWM and real-time control on TI C2000 DSPs (Code Composer Studio), C and Embedded C, Siemens PLC (TIA Portal)
* **Data and optimization:** Python (Gaussian-process regression, tree ensembles, SHAP, Sobol), PSO, GA, NSGA-III

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
