---
permalink: /
title: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am third-year Ph.D. student in [Power Switch Lab](https://psl.uark.edu/sample-page/) at the [Grid Connected Advanced Power Electronic Systems (GRAPES)](https://grapes.uapower.group/) research center at the University of Arkansas, Fayetteville, under the guidance of Dr. [Xiaoqing Song](https://scholar.google.com/citations?user=WZ3UPGAAAAAJ&hl=zh-CN). I obtained my MS degree from [Ghulam Ishaq Khan Institute of Engineering Sciences and Technology](https://giki.edu.pk/), Paksitan in 2019, and BS degree from [University of Engineering and Technology](https://www.uetpeshawar.edu.pk/), Peshawar, Pakistan, in 2016.

During my Ph.D., I have worked on medium-voltage SiC-based high-voltage switch and GaN-based multilevel inverter. In summer 2026, I was a power electronics intern at Tesla Energy in Palo Alto, CA, on the Power Conversion Hub team where I studied Tesla's residential Powerwall 3 and tested and fixed hardware issues in its inverter stage and ground-fault current interrupter . Prior to pursuing Ph.D., I was a laboratory lecturer at GIK Institute, Pakistan, where I upgraded the Linear Control Systems and DSP labs with Siemens PLCs and DSP kits.

Research interests
======

- **Series-connected SiC MOSFET switches** for 10–20 kV applications such as medium-voltage converters, data-center power, and solid-state circuit breakers
- **Active dv/dt control** for dynamic voltage balancing without snubbers or extra isolated supplies
- **Isolated gate-driver power supplies** with high insulation and low coupling capacitance
- **Measurement-driven sensitivity analysis** that links device parameter spread to switching behavior

I am interested in simplifying the power-stage design of medium-voltage power converters. One of the options has been to replace the unnecessary multi-level architectures of switching legs with single half-bridge operation. To realize that, high-voltage monolithic devices are required.

I am interested in developing high-voltage SiC switch using low-voltage MOSFETs and adopting that approach instead of multi-level approach in medium-voltage power converters. But discrete devices above ~15kV are still mostly research parts. However, discrete 3.3kV and 6.5kV SiC MOSFETs are readily available. So, stacking low-voltage devices gives a practical high-voltage switch, as long as every device stays within its safe voltage during all operation conditions. That is the hard part because small mismatches in MOSFET's intrinsic parameters, gate driver output voltage-level and timing, and layout parasitics cause large voltage imbalance during switching transitions. My goal is to develop low-cost, high-voltage SiC switch architectures that offer above 20kV voltage-blocking capability while achieving high power-density and reliable operation.

See my [Research]({{ site.baseurl }}/research/) and [Publications]({{ site.baseurl }}/publications/).

