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
---

{% for patent in page.patents %}
<div>
    {{patent.string}}:
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/{{patent.number}}" 
    target="_blank" rel="noopener noreferrer"> 
        "{{patent.name}}"
    </a>
</div>
{% endfor %}

<!-- <p>
    10,143,052: 
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/10143052">
        "Light Emitting Diode (LED) Warm on Dim Circuit"
    </a>
    <br> 	
    9,107,273: "End-of-Life Bulb Circuitry"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/9107273">
    </a>
    <br>
    9,030,118: "Single Inductor Control of Multi-Color LED Systems"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/9030118">
    </a>
    <br>
    8,853,921: "Heat Removal Design for LED Bulbs"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8853921">
    </a>
    <br>
    8,816,594: "3-Way LED Bulb"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8816594">
    </a>
    <br>
    8,796,922: "Phosphor-Containing LED Light Bulb"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8796922">
    </a>
    <br>
    8,786,169: "Anit-Reflective Coatings for Light Bulbs"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8786169">
    </a>
    <br>
    8,760,066: "Constant Power LED Circuit"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8760066">
    </a>
    <br>
    8,754,594: "Thermal Protection Circuit for an LED Bulb"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8754594">
    </a>
    <br>
    8,752,984: "Glass LED Light Bulbs"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8752984">
    </a>
    <br>
    8,704,442: "Method of Light Dispersion and Preferential Scattering of Certain Wavelengths of Light for Light-Emitting Diodes and Bulbs Constructed Therefrom"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8704442">
    </a>
    <br>
    8,702,257: "Plastic LED Bulb"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8702257">
    </a>
    <br>
    8,638,033: "Phosphor-Containing LED Light Bulb"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8638033">
    </a>
    <br>
    8,598,794: "White AC LED"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8598794">
    </a>
    <br>
    8,569,949: "Method of Light Dispersion and Preferential Scattering of Certain Wavelengths of Light for Light-Emitting Diodes and Bulbs Constructed Therefrom"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8569949">
    </a>
    <br>
    8,552,654: "Single Inductor Control of Multi-Color LED Systems"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8552654">
    </a>
    <br>
    8,547,002: "Heat Removal Design for LED Bulbs"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8547002">
    </a>
    <br>
    8,471,445: "Anti-Reflective Coatings for Light Bulbs"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8471445">
    </a>
    <br>
    8,450,927: "Phosphor-Containing LED Light Bulb"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8450927">
    </a>
    <br>
    8,439,528: "Glass LED Light Bulbs:
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8439528">
    </a>
    <br>
    8,283,877: "Thermal Protection Circuit for an LED Bulb"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8283877">
    </a>
    <br>
    8,278,837: "Single Inductor Control of Mluti-Color LED Systems"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8278837">
    </a>
    <br>
    8,198,819: "3-Way LED Bulb"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8198819">
    </a>
    <br>
    8,193,702: "Method of Light Dispersion and Preferential Scattering of Certain Wavelengths of Light for Light-Emitting Diodes and Bulbs Constructed Therefrom"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/8193702">
    </a>
    <br>
    6,538,516: "System and Method for Synchronizing Multiple Phase-Lock Loops or Other Synchronizable Oscillators Without Using a Master Clock Signal"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/6538516">
    </a>
    <br>
    6,531,851: "Linear Regulator Circuit and Method"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/6531851">
    </a>
    <br>
    6,528,976: "FET Sensing Programmable Active Droop for Power Supplies"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/6528976">
    </a>
    <br>
    6,222,352: "Multiple Voltage Output Buck Converter with a Single Inductor"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/6222352">
    </a>
    <br>
    6,104,170: "Method and Circuit for Preventing Oscillations in a Battery Charger"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/6104170">
    </a>
    <br>
    5,844,440: "Circuitry for Inrush and Current Limiting"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/5844440">
    </a>
    <br>
    5,594,324: "Stabilized Power Converter Having Quantized Duty Cycle"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/5594324">
    </a>
    <br>
    5,477,132: "Multi-Sectioned Power Converter having Current-Sharing Controller"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/5477132">
    </a>
    <br>
    5,359,280: "Bilateral Power Converter for a Satellite Power System"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/5359280">
    </a>
    <br>
    5,233,287: "Current Limiting Bilateral Converter Having a Ground Referenced Current Sensor"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/5233287">
    </a>
    <br>
    4,894,567: "Active Snubber Circuit"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/4894567">
    </a>
    <br>
    3,971,372: "Oxygen-Generating Apparatus for Scuba Diving"
    <a href="https://image-ppubs.uspto.gov/dirsearch-public/print/downloadPdf/3971372">
    </a>
    <br>
</p> -->