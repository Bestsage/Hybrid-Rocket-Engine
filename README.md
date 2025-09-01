# Hybrid Rocket Engine Demonstrator

[![License: Educational](https://img.shields.io/badge/License-Educational-blue.svg)](LICENSE)
[![Project Status: Complete](https://img.shields.io/badge/Project%20Status-Complete-brightgreen.svg)]()
[![Documentation](https://img.shields.io/badge/docs-available-blue.svg)](docs/)

![Test firing with shock diamonds](docs/shock_diamond.png)

## Table of Contents
- [Overview](#overview)
- [Abstract](#abstract)
- [Technical Specifications](#technical-specifications)
- [Test Results Gallery](#test-results-gallery)
- [Versioning System](#versioning-system)
- [Key Features](#key-features)
- [Repository Contents](#repository-contents)
- [Safety Considerations](#safety-considerations)
- [How to Use This Repository](#how-to-use-this-repository)
- [Citation](#citation)
- [Authors](#authors)
- [License](#license)

## Overview
This repository documents the **design, construction, and testing** of a **hybrid rocket engine demonstrator**, developed as part of our *Travail de maturité* and presented at the **Swiss National Contest**.  

Hybrid propulsion combines a **liquid oxidizer** with a **solid fuel grain**, offering a **middle ground** between:
- Simplicity and accessibility of **solid rockets**
- Performance and controllability of **bi-liquid engines**

Our objective:  
👉 Build a **reliable, efficient engine** with limited resources, able to theoretically propel a model rocket.

---

## Abstract
Over 9 months, we applied an **iterative engineering process**:  
- **Design**: CAD modeling (Fusion 360), rendering (Blender), combustion simulations (RocketCEA).  
- **Construction**: Machined steel combustion chamber, graphite nozzle, ABS/ASA fuel grains.  
- **Instrumentation**: Custom-built static test bench with Arduino-based data acquisition (thrust, pressure, temperature).  
- **Testing**: 18 static firings, continuously improving injector design, nozzle geometry, and fuel formulation.  

**Results**:  
- Stable thrust plateau of **40 N** (peak **43 N**) during 5-second burns  
- Combustion chamber pressure remained constant  
- Temperature < **150 °C** (no thermal risk observed)  
- **16 out of 18 successful tests** → high system reliability  
- Supersonic exhaust confirmed (visible shock diamonds)  

These results confirm that **hybrid propulsion is a viable option for model rocketry**, balancing performance, cost, and safety.

---

## Technical Specifications

### Engine Performance (Latest Configuration: V3-1-1)
| Parameter | Value | Unit |
|-----------|-------|------|
| **Maximum Thrust** | 10.65 | N |
| **Average Thrust** | 9.22 | N |
| **Burn Time** | 5.0 | seconds |
| **Total Impulse** | 46.09 | N⋅s |
| **Specific Impulse** | 22.27 | seconds |
| **Chamber Pressure** | 5.84 (avg), 6.76 (max) | bar |

### Physical Specifications
| Component | Specification |
|-----------|--------------|
| **Combustion Chamber** | Machined steel, custom design |
| **Nozzle** | Graphite, throat diameter 5mm, exit 24mm |
| **Fuel Grain** | ABS/ASA plastic, star-shaped geometry |
| **Oxidizer** | Gaseous oxygen at 9 bar |
| **Injector** | Custom 3.5mm diameter orifice |

### Test Configuration
- **Fuel Mass**: 44g initial, 27g consumed (61% burn efficiency)
- **O/F Ratio**: 6.8:1 (oxygen to fuel)
- **Operating Temperature**: <150°C (safe thermal limits)
- **Success Rate**: 89% (16/18 successful tests)

---

## Test Results Gallery

### Performance Data by Version
- **[Version 1 Tests](docs/v1/)** - Initial proof of concept
- **[Version 2 Tests](docs/v2/)** - Improved injector design  
- **[Version 3 Tests](docs/v3/)** - Optimized nozzle geometry

### Key Test Results
| Test ID | Thrust (N) | Burn Time (s) | Chamber Pressure (bar) | Status |
|---------|------------|---------------|------------------------|---------|
| V3-1-1 | 10.65 peak | 5.0 | 6.76 max | ✅ Success |
| V3-1-2 | TBD | TBD | TBD | ✅ Success |
| V3-2-1 | TBD | TBD | TBD | ✅ Success |

*Note: Each test folder contains detailed telemetry data (.TXT), analysis spreadsheets (.xlsx), temperature plots (.png), and test videos (.MOV)*

---

## Versioning System
All engine prototypes and test runs were indexed as:

VX-Y-Z

  - **X** = Major version (nozzle/injector redesign, new chamber)  
  - **Y** = Minor variant (fuel grain geometry, material)  
  - **Z** = Test number of that configuration  

Example: `V3-1-2` → Engine Version 3, first minor variant, second test.

---

## Key Features
- 🔧 **Custom static test stand**  
- 📈 **Arduino Nano + sensors** for thrust, chamber pressure, temperature  
- ♻️ **Iterative development cycle** (SpaceX-inspired approach: "Test, Fail, Fix, Repeat")  
- 🧪 **Supersonic flow** proven with visible shock diamonds  

---

## Repository Contents
- 📊 `NW25-643729_Finale_Arbeit.pdf` → **Full technical paper** (108 pages with detailed methodology, results, and analysis)  
- 📂 `docs/shock_diamond.png` → Supersonic exhaust visualization showing shock diamonds
- 📂 `docs/v1/` → Version 1 test data (initial proof of concept)
- 📂 `docs/v2/` → Version 2 test data (improved injector design)  
- 📂 `docs/v3/` → Version 3 test data (optimized performance)

### Test Data Structure
Each test folder (`docs/v{X}/v{X}-{Y}/v{X}-{Y}-{Z}/`) contains:
- **Raw telemetry**: `.TXT` files with time-series sensor data
- **Analysis**: `.xlsx` spreadsheets with calculated performance metrics  
- **Visualizations**: `.png` graphs showing thrust, pressure, and temperature
- **Documentation**: Test footage in `.MOV` format

---

## Safety Considerations

⚠️ **IMPORTANT SAFETY NOTICE** ⚠️

This project involves high-pressure systems, combustible materials, and rocket propulsion. **DO NOT attempt to replicate without proper safety training and supervision.**

**Safety measures implemented:**
- Static test stand with blast shields
- Remote ignition and data acquisition
- Fire suppression equipment on-site
- Proper ventilation and outdoor testing
- Personal protective equipment (PPE)
- Emergency shutdown procedures

**For educational use only** - This documentation is provided for learning purposes. Always consult with professionals and follow local regulations before conducting any rocket engine testing.

---

## How to Use This Repository

### Understanding the Test Data
1. **Navigate to test folders**: `docs/v{version}/v{version}-{variant}/v{version}-{variant}-{test}`
2. **Key files in each test folder**:
   - `.TXT` files: Raw sensor data (time, temperature, pressure, thrust)
   - `.xlsx` files: Processed data and analysis
   - `.png` files: Performance graphs and temperature plots
   - `.MOV` files: High-speed test footage
   - `*-output.txt`: Summary results and calculated performance metrics

### Analyzing Performance Data
- Thrust measurements in Newtons (N) and equivalent mass (kg)
- Chamber pressure in bar and Pascals
- Temperature monitoring at multiple points
- Burn time and total impulse calculations
- Fuel consumption and efficiency metrics

### Academic Research
This work represents a comprehensive study of hybrid rocket propulsion suitable for:
- University-level aerospace engineering courses
- High school physics and chemistry demonstrations
- Research into hybrid propulsion systems
- Model rocketry safety and performance analysis

---

## Citation

If you use this work in academic research or educational materials, please cite:

```
Bumann, S., & Gebhard, S. (2024). Hybrid Rocket Engine Demonstrator: 
Design, Construction, and Testing. Swiss National Contest - Travail de maturité. 
Gymnase de Morges. Retrieved from https://github.com/Bestsage/Hybrid-Rocket-Engine
```

**Academic Paper**: The complete 108-page technical documentation is available in `NW25-643729_Finale_Arbeit.pdf`

---

## Authors
- **Sacha Bumann**  
- **Samuel Gebhard**  

With the support of:  
- *Gymnase de Morges*
- dr. Ricardo Perez 
- prof. Gabriel Paciotti
- Daniel Gebhard
---

## License
This repository is provided for **educational and research purposes**.  
Feel free to explore, learn, and build upon our work 🚀


