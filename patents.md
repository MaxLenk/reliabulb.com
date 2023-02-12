---
layout: page
title: Patents
permalink: patents

patents:
-   number: 10143052
    string: "10,143,052"
    name: Light Emitting Diode (LED) Warm on Dim Circuit
     	
-   number: 9107273
    string: "9,107,273"
    name: End-of-Life Bulb Circuitry
    
-   number: 9030118
    string: "9,030,118"
    name: Single Inductor Control of Multi-Color LED Systems
    
-   number: 8853921
    string: "8,853,921"
    name: Heat Removal Design for LED Bulbs
    
-   number: 8816594
    string: "8,816,594"
    name: 3-Way LED Bulb
    
-   number: 8796922
    string: "8,796,922"
    name: Phosphor-Containing LED Light Bulb
    
-   number: 8786169
    string: "8,786,169"
    name: Anti-Reflective Coatings for Light Bulbs
    
-   number: 8760066
    string: "8,760,066"
    name: Constant Power LED Circuit
    
-   number: 8754594
    string: "8,754,594"
    name: Thermal Protection Circuit for an LED Bulb
    
-   number: 8752984
    string: "8,752,984"
    name: Glass LED Light Bulbs
    
-   number: 8704442
    string: "8,704,442"
    name: Method of Lght Dispersion and Preferential Scattering of Certain Wavelengths of Light for Light-Emitting Diodes and Bulbs Constructed Therefrom
    
-   number: 8702257
    string: "8,702,257"
    name: Plastic LED Bulb
    
-   number: 8638033
    string: "8,638,033"
    name: Phosphor-Containing LED Light Bulb
    
-   number: 8598794
    string: "8,598,794"
    name: White AC LED
    
-   number: 8569949
    string: "8,569,949"
    name: Method of Lght Dispersion and Preferential Scattering of Certain Wavelengths of Light for Light-Emitting Diodes and Bulbs Constructed Therefrom
    
-   number: 8552654
    string: "8,552,654"
    name: Single Inductor Control of Multi-Color LED Systems
    
-   number: 8547002
    string: "8,547,002"
    name: Heat Removal Design for LED Bulbs
    
-   number: 8471445
    string: "8,471,445"
    name: Anti-Reflective Coatings for Light Bulbs
    
-   number: 8450927
    string: "8,450,927"
    name: Phosphor-Containing LED Light Bulb
    
-   number: 8439528
    string: "8,439,528"
    name: Glass LED Light Bulbs
    
-   number: 8283877
    string: "8,283,877"
    name: Thermal Protection Circuit for an LED Bulb
    
-   number: 8278837
    string: "8,278,837"
    name: Single Inductor Control of Mluti-Color LED Systems
    
-   number: 8198819
    string: "8,198,819"
    name: 3-Way LED Bulb
    
-   number: 8193702
    string: "8,193,702"
    name: Method of Lght Dispersion and Preferential Scattering of Certain Wavelengths of Light for Light-Emitting Diodes and Bulbs Constructed Therefrom
    
-   number: 6538516
    string: "6,538,516"
    name: System and Method for Synchronizing Multiple Phase-Lock Loops or Other Synchronizable Oscillators Without Using a Master Clock Signal
    
-   number: 6531851
    string: "6,531,851"
    name: Linear Regulator Circuit and Method
    
-   number: 6528976
    string: "6,528,976"
    name: FET Sensing Programmable Active Droop for Power Supplies
    
-   number: 6222352
    string: "6,222,352"
    name: Multiple Voltage Output Buck Converter with a Single Inductor
    
-   number: 6104170
    string: "6,104,170"
    name: Method and Circuit for Preventing Oscillations in a Battery Charger
    
-   number: 5844440
    string: "5,844,440"
    name: Circuitry for Inrush and Current Limiting
    
-   number: 5594324
    string: "5,594,324"
    name: Stabilized Power Converter Having Quantized Duty Cycle
    
-   number: 5477132
    string: "5,477,132"
    name: Multi-Sectioned Power Converter having Current-Sharing Controller
    
-   number: 5359280
    string: "5,359,280"
    name: Bilateral Power Converter for a Satellite Power System
    
-   number: 5233287
    string: "5,233,287"
    name: Current Limiting Bilateral Converter Having a Ground Referenced Current Sensor
    
-   number: 4894567
    string: "4,894,567"
    name: Active Snubber Circuit
    
-   number: 3971372
    string: "3,971,372"
    name: Oxygen-Generating Apparatus for Scuba Diving

---

<div class="font-sans pl-32 pt-4 pb-16 prose-{{site.theme-color}}">
    {% for patent in page.patents %}
        <div>
            {{patent.string}}:
            <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/{{patent.number}}" 
            target="_blank" rel="noopener noreferrer"> 
                "{{patent.name}}"
            </a>
        </div>
    {% endfor %}
</div>
