---
layout: archive
title: "Resume"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Highlights
======
* Seasoned RF Front End architect for battery driven mobile and access point reference design.
* Optical communication module and silicon experience such as ROSA/TOSA, Laser/photo diode, TIA, Laser Driver, CDR, Equalizer.
* Low power architect for Qualcomm’s reference design.
* RF simulation for WiFi, BT, LAA, 5G NR-U, UWB coexistence, including antenna sharing and Rx desense solving. 
* Applied machine learning algorithm on modem SoC dynamic rail voltage scaling for power saving.
* Data driven decision making: MSSQL and MySQL database experience with large engineering data analysis skill.
* Software and tools: SystemVue, Matlab, ADS, HFSS, Spotfire, JMP, SPICE, Allegro, C++, Java, python, Unix scripts, iperf, IxChariot etc.

Work experience
======
### SENIOR STAFF, Connectivity Hardware System Architect at [Qualcomm Atheros](https://www.qualcomm.com/home), San Jose
> October 2014 — March 2023
#### Owner of Front-End Module (FEM) qualification process. Owner of Power, thermal KPIs. Owner of reference design RF co-existing FEM KPIs. 

* Driving Mobile RF Front End (RFFE) design, qualification for next generation WiFi7, BT, UWB, and 5G NR-U coexist.
  *	Conducting Rx cascade gain line-up analysis to improve Rx desense. 
  *	Successfully simulated and predicted WiFi7 MLO 5/6G co-exist mode lo spur 2nd order mixer effects caused Rx desense. 
  *	Working on linear/nonlinear/Doherty PA with DPD, memory DPD, CFR, ET, APT, multi modes PA/LNA for low power, cost effective FEM module designs. 
  *	Hands-on validating, charactering, generation internal and external formal reports for every FEM engineering stage. Checking items are EVM, drooping, Mask, ACP, IIP2/3, NF, power efficiency etc. over temperatures and voltages. 
  *	Highly respected individual by FEM vendors and tester vendors. They are using my feedback to guide their design efforts or instrument improvements for meeting KPIs.  
  *	I am the first one who defined Wi-Fi 6E/7 LNA KPIs 3 years ahead of time.
  *	Creating, maintaining FEM MSSQL database (over 1T data/1.5billion records). 
* Partner with Qualcomm’s different technology teams to design innovative digital enhancements to wireless products.
  *	Bringing up 11be/WiFi7 waveforms from Matlab/SystemVue simulation to Lab bench validation for compensating various RF impairments.
  *	Researching PA drooping compensation methods from both silicon process and system baseband. Created a statistic model in MATLAB for estimating the EVM distributions with open loop DPD and improving baseband drooping compensation method based on the PA’s physical thermal nature.
* Working on 4 categories of battery driven mobile system-level low power design. Owner of power, thermal, throughput, latency KPIs over process, voltage, and temperature. 
  *	Lower voltage, current, leakage and frequency.
  *	Shorten the SoC circuit activity time such as power collapse, clock gate etc.
  *	Balance trade-offs on RF coverage, throughput, and power per Day-of-Use cases.
  *	Use CSMA/CA based approach to lower the system wake-up frequency.
* Invented mobile SoC dynamic voltage control algorithm for power saving and throughput improvement based on multivariate machine learning models.
  *	Design of Experiments (DOE) approach from large lab datasets.
  *	Use multivariate machine learning models to calculate the polynomial functions SoC Vmin vs. SoC Process, Tj, and Throughput.
  *	Model results have been validated on three generations of SoC designs.
* Maintaining the pace of per year learning/creating 2 new things in addition to daily work.
  *	2023, Built MSSQL database and implemented off-the-shelf DPD solution. 
  *	2022, Invented sinewave drooping characterization method and enabled SystemVue simulation platform for complex RF co-exist simulation.
  *	2021, Completed 11be compressed PAPR waveform EVM analysis and physically verified 320M BW 11be waveform before SoC RTL releasing. 
  *	2020, Applied multivariate machine learning models to the mobile soc dynamic power rail voltage control algorithm as power saving method and promoted the Wi-Fi 6E FEM golden standard over all FEM vendors.
  *	2019, Invented mobile reference power estimation tool for customers and maintained power thermal KPIs.
  *	2018, Invented access point power estimation tool for customers and created new FEM module evaluation platform.
  *	2017 and before, Architected the 11be FTM DVT solutions and started mission mode performance vs. power evaluation task. 

### PRINCIPAL ENGINEER, ATE ARCHITECT at [Broadcom](https://www.broadcom.com/), Santa Clara
> March 2013 — September 2014
#### Reported to network organization and bought SerDes ATE test for MIPS CPUs and 25GB Switch IC.

* Solved Broadcom IC backend operation challenges after merged with Netlogic’s multi core server CPU business. 
*	Solved 10G, 25G Serdes ATE characterization and mass production test challenge for 144 lanes switch chip.  

### I/O CONSULTANT (CONTRACT) at [AMD](https://www.amd.com/en.html), Markham, Canada
> November 2011 — October 2012
#### Reported to Advantest Test Characterization organization with responsibility for leading complex characterization SerDes ATE solution for APU, GPU, CPU line.

*	Solved PCIE Gen3(8G/s) and GDDR5 ATE test challenges for GPU/APU.

### PRINCIPAL ENGINEER at [Gennum Corp/Semtech](https://www.semtech.com/products/signal-integrity), Burlington, Ontario, Canada
> May 2004 — October 2011
#### Reported to Directors and Sr. VPs with responsibility for leading bare die and final test backend business.

* Led a task force to deliver the 1st generation Thunderbolt cable drivers (CDRs and EQs) project for the Apple Mac Computer. 
*	Built 26.5GHz BW Optical Domain characterization lab(850/1310/1550nm) for ROSA/TOSA/TIA/Laser Driver/limiting AMP.
*	Characterized ROSA family(>10Gb/s) with following items: Voltage, Temperature, URS, SRS, Jitter, Cross point, Swing, Eye heights, Eye amplitude, Optical S-parameter, etc.
*	Hands-on experience on following optical instruments: Optical Source, Modulation Source, optical return loss, tester, optical vector network analyzer, optical power meter, optical attenuators, optical switches, optical spectrum analyzer, all sorts of 850nm/1310nm/1550nm connectors, patch cords, EDFA amplifier. 
*	Invented bare die full speed (>10Gb/s) qualification/HTOL methodology. Kept 100% successful rate on this qualification approach. 



Education
======
* Bachelor degree in Electronic Engineering, major in radio technology, [Xi'an Jiaotong University](http://en.xjtu.edu.cn/), Xi'an, China
* Post graduate studies, major in digital signal process. On leave without completing the degree, [University of Electronic Science and Technology of China](https://en.uestc.edu.cn/), Chengdu, China


Skills
======
* Simulation Tools
  * ADS
  * SystemVue
  * HFSS
  * Matlab
* Software
  * Python
  * JAVA
  * C++
  * VB6
* Data Analysis Tools
  * Spotfire
  * JMP
  * R
  * Octave

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
