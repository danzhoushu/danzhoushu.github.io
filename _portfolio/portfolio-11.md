---
title: "Technologies: Back to basics"
excerpt: "Simplicity, clarity, and a solid foundation <br/><img src='/images/IEEE802_11.png'>"
collection: portfolio
---

This section holds some simplicity, clarity, and a solid foundation concepts about communication system design.

[Keysight signal studio](https://www.keysight.com/us/en/lib/resources/technical-specifications/latest-versions-signal-studio-software-2806906.html) provides details information about IEEE802.11 packets. Downloading and running on PC are free without instruments attached.
<a href="/images/IEEE802_11.png">
    <img 
        src="/images/IEEE802_11.png" 
    >
</a>
*Pic1: IEEE802.11 Packet structure illustration*

<a href="/images/BT_UWB.png">
    <img 
        src="/images/BT_UWB.png" 
    >
</a>
*Pic2: Bluetooth Packet structure and UWB FCC requirements*

The FFT algorithm reduces the computational complexity of the DFT from O(N^2) to O(NlogN), making it faster and more practical to use for large data sets.
<a href="/images/FFT_4.png">
    <img 
        src="/images/FFT_4.png" 
    >
</a>
*Pic3: FFT is a special type of DFT *

The 4 types of amplifier are showed below by using OP-Amp model. They are V/V, I/I, I/V, V/I. The most of Analog IC design circuits today are coming from these 4 types of amp.   
<a href="/images/amp_4.png">
    <img 
        src="/images/amp_4.png" 
    >
</a>
*Pic4: 4 types of amplifier*

Two types of LTE_A system are existing, TDD and FDD. [Keysight signal studio](https://www.keysight.com/us/en/lib/resources/technical-specifications/latest-versions-signal-studio-software-2806906.html) provides details information about these RF packets differences. Downloading and running on PC are free without instruments attached.    
<a href="/images/LTE_A.png">
    <img 
        src="/images/LTE_A.png" 
    >
</a>
*Pic5: Spectrum of LTE-A: TDD vs. FDD*

RX desense could happen by many reasons. Understanding the Rx architect is the first step to solve RF path caused Rx desense.     
<a href="/images/RxDesense_RFpath.png">
    <img 
        src="/images/RxDesense_RFpath.png" 
    >
</a>
*Pic6: Typical Zero-IF receiver RF architect*

By understanding the limitations of the EVM measurement tool, designers can optimize the design of the PA/LNA and create better DPD/CFR algorithms. This can lead to achieving a better trade-off between EVM and DC power conservation.
<a href="/images/EVM_floor_20230305.png">
    <img 
        src="/images/EVM_floor_20230305.png" 
    >
</a>
*Pic7: EVM floor illustration*

Choosing the best DPD algorithm can be challenging as there is no one-size-fits-all solution. It is important to consider individual use cases and other factors of the PA, such as power efficiency over the full RF output power range and over process, voltage, and temperature (PVT).  
<a href="/images/dpd_optimization.png">
    <img 
        src="/images/dpd_optimization.png" 
    >
</a>
*Pic8: Which DpD is better?*

EVM Separation: Deterministic EVM degradation can be improved by digital enhancement  
<a href="/images/EVM_separation.png">
    <img 
        src="/images/EVM_separation.png" 
    >
</a>
*Pic9: EVM separation*

The RF Front-End (RFFE) module packages non-CMOS silicon components such as PA/LNA, filters, switches, and N-duplexers together to achieve better performance with a smaller footprint on the PCB.    
<a href="/images/Module.png">
    <img 
        src="/images/Module.png" 
    >
</a>
*Pic10: RFFE module example*

Low power design is a multi-faceted process, and different teams typically focus on specific areas within the design. As architects, it is important to have a top-down view of the design process and understand which team is responsible for each aspect of the low power design.   
<a href="/images/LowPower.png">
    <img 
        src="/images/LowPower.png" 
    >
</a>
*Pic11: Low power design architect view*

Using a low power rail can effectively reduce ICQ and ICC, resulting in power savings. However, voltage rail ripples can be a major limiting factor when reducing rail voltages. In modern PDN designs, Switched-Mode Power Supplies (SMPS) and Power Management Integrated Circuits (PMIC) are the two typical types of DC-DC converters used. Excessive voltage ripples are mainly due to SMPS's transistor inability to handle Di/Dt in cases of large dynamic current consumption, rather than Dv/Dt.   
<a href="/images/SMPS_basis.png">
    <img 
        src="/images/SMPS_basis.png" 
    >
</a>
*Pic12: Control the voltage ripples of SMPS*

The test data obtained during silicon manufacturing follows a Gaussian Mixture distribution. However, in everyday engineering activities, people often assume these datasets follow a Gaussian distribution and make calculations accordingly. Understanding the difference between these two distribution types can be beneficial for system architects.    
<a href="/images/Gaussian_mixture.png">
    <img 
        src="/images/Gaussian_mixture.png" 
    >
</a>
*Pic13: Gaussian Mixture distribution is the production test dataset statistic model*

I use ChatGPT at home.   
<a href="/images/Bard_vs_ChatGPT.png">
    <img 
        src="/images/Bard_vs_ChatGPT.png" 
    >
</a>
*Pic14: ChatGPT vs. Bard*




