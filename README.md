# Hybrid Rocket Engine Demonstrator

![Test firing with shock diamonds](docs/shock_diamond.png)

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
- 📊 `NW25-643729_Poster.pdf` → Project poster (concise overview)  
- 📖 `NW25-643729_Finale_Arbeit.pdf` → Full technical paper (90+ pages, detailed methodology & results)  
- 📂 `docs/` → Additional images, CAD renders, and test data (to be added)  

---

## Authors
- **Sacha Bumann**  
- **Samuel Gebhard**  

With the support of:  
- *Gymnase de Morges*  
- **EPFL Rocket Team** (advice & mentoring)  

---

## License
This repository is provided for **educational and research purposes**.  
Feel free to explore, learn, and build upon our work 🚀


