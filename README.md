# CoolGirl2210
EPM2210 Variant of the COOLGIRL - Ultimate Multigame Cartridge for the Famicom

Supports ALL COOLGIRL mappers in a single cartridge.

Upgrades:

1. EPM1270 → EPM2210: The upgraded CPLD allows support for ALL mappers.

2. 3.3V Power: Switched from an LDO to a DC-DC converter. This allows the cartridge to run on cheaper Famicom clones (e.g., the Subor D99, which uses USB power and only supplies 500mA!).

3. SRAM: Replaced the very expensive FM18L08 chip with the cheaper LY62256.

4. CHR-RAM: Relocated the STSOP-32 footprint to allow easier CHR-RAM troubleshooting.

5. Flash Expansion: Reserved footprint for the S70GL02GT for future upgrades (utilizing `hardware` bank switching to switch between the upper 1G and lower 1G).

6. Resistors: Changed from 0402x4 chip resistor arrays to 0603x4 for easier DIY assembly.

7. Level Shifters: Changed from a single SN74ALVC164245 to two SN74LVC8T245 for easier DIY assembly.

8. Assembly: All optional components are placed on the bottom layer, allowing for SMT assembly on the top layer only.

Due to a factory defect in some EPM2210 chips, EPM2210 may have no output on the D4 and C4 pins.
**It is strongly recommended to run EPM2210TEST to verify ALL pins after soldering the EPM2210.**
(Use φ2(M2) as the clock input, located at the D3-LL4148 positive pin.)

PCB files and Gerbers are pending, awaiting approval from Alexey Cluster.


![CoolGirl-2210-top.jpg](CoolGirl-2210-top.jpg)

![CoolGirl-2210-bottom.jpg](CoolGirl-2210-bottom.jpg)

![CoolGirl-2210-withbox.jpg](CoolGirl-2210-withbox.jpg)

S70GL02 localtion(Expensive, not verify)

![CoolGirl-2210-top-S70GL02.png](CoolGirl-2210-top-S70GL02.png)

Original COOLGIRL Design:

* [COOLGIRL - ultimate multigame cartridge for Famicom](https://github.com/ClusterM/coolgirl-famicom-multicart)