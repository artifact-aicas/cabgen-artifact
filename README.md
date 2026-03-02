# CABGen (Anonymous Submission)

This repository contains some output benchmark packages from **C**omprehensive layout-aware **A**nalog circuit **B**enchmark **Gen**erator

## Status
An improved version is being prepared to submit to [IEEE SSCS Open-Source Ecosystem “Code-a-Chip”](https://github.com/sscs-ose/sscs-ose-code-a-chip.github.io/tree/main/). Upon acceptance, we will make all materials publicly available and provide a more comprehensive and detailed description. 

### 🛠️ Execution Environment

All experiments were conducted and verified under the following settings to ensure consistency and performance:

* **Operating System**: Ubuntu 22.04.4 LTS
* **Python Version**: 3.11 (A dedicated **Conda environment** is highly recommended)
* **Open PDK and EDA Tools**:
    * **SKY130A**: 
    * **Ngspice**: 
    * **ALIGN**: 
    * **KLayout**: 
    * **Magic**: 
    * **Netgen**:
 
### 📦 Benchmark Package Example

Using a five-transistor OTA as an example to illustrate the benchmark packages.

``` javascript
{   
    "trial": 2,
    "Pkg": {
        "param": ["ckt_param.spice"],
        "const": ["layout_const.json"],
        "pre-sim": ["gain_pre.txt", "phase_pre.txt", "inoise_pre.txt", "transient_pre.txt"],
        "layout": ["FIVE_TRANSISTOR_OTA_0.gds", "FIVE_TRANSISTOR_OTA.lef"],
        "extract": ["FIVE_TRANSISTOR_OTA_0_lvs.spice","FIVE_TRANSISTOR_OTA_0_pex.spice"],
        "drc": ["drc_report.xml"],
        "lvs": ["comp.out"],
        "post-sim": ["gain_post.txt", "phase_post.txt", "inoise_post.txt", "transient_post.txt"]
    }
}
```
