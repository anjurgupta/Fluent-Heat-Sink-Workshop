# Electronics Cooling with ANSYS Fluent: A Hands-On Experiential Workshop

Heat Sink CFD Workshop: Comparative Analysis of No Heat Sink, Rectangular Fins, and Triangular Fins
This detailed tutorial is designed for faculty and instructors to adopt for undergraduate or early graduate instruction in heat transfer, thermal management, or applied computational fluid dynamics. The materials, structure, and learning outcomes are fully aligned with ABET criteria, Bloom’s Taxonomy, and open educational resource best practice—ensuring your students achieve authentic, transferable engineering skills. 

## Overview

This workshop guides students through the process of computationally modeling, simulating, and comparing three heat sink configurations for electronics cooling:

Flat plate with no heat sink
Plate with rectangular fins
Plate with triangular fins

Students use ANSYS Fluent (Student or Academic versions) and provided reference files to perform geometry creation, meshing, physics setup, simulation, and data interpretation. The objective is a rigorous comparison of thermal performance, material efficiency, and practical design trade-offs for forced convection air cooling in an electronics context.

## Learning Objectives

By the end of this workshop, participants will be able to:

Create and import 3D CAD geometries for flat, rectangular-finned, and triangular-finned heat sinks in ANSYS Fluent (Apply)

Generate and refine high-quality surface and volume meshes, including boundary layer treatment and mesh diagnostics (Apply, Analyze)

Set up conjugate heat transfer simulations, choosing appropriate materials and boundary conditions (Apply)

Run and converge steady-state forced convection simulations, diagnosing solution errors and interpreting residual plots (Apply, Analyze)

Extract and interpret temperature, velocity, and heat flux results for each design (Analyze, Evaluate)

Compare and contrast the thermal and material performance of alternative geometries using quantitative results (Evaluate)

Justify recommendations for design selection based on simulation evidence and practical considerations (Evaluate, Create)

Relate outcomes to sustainability and manufacturing constraints in thermal management (Evaluate, Create)

## Software Requirements

### ANSYS Fluent Student Edition - Completely Free

- **Download**: [https://www.ansys.com/academic/students](https://www.ansys.com/academic/students)
- **License**: No license required for student version
- **Limitations**: 512,000 cell maximum (more than sufficient for this workshop)
- **Platforms**: Windows 64-bit
- **Disk space**: 15-20 GB for full ANSYS Student installation

## Prerequisites

- Completed undergraduate heat transfer course (conduction and convection fundamentals)
- Basic understanding of forced convection and Newton's Law of Cooling
- Familiarity with engineering problem-solving approaches
- No prior CFD experience required

## Quick Start Guide

### For Students

1. **Download ANSYS Student**: Visit [ansys.com/academic/students](https://www.ansys.com/academic/students) (free download, no license needed)
2. **Clone this repository**: 
   ```bash
   git clone https://github.com/anjurgupta/Fluent-Heat-Sink-Workshop 

## Problem Specifications

### System Configuration
- Overall base plate dimensions: 36 cm × 36 cm × 3 mm
- Material: Aluminum (k = 237 W/(m·K), ρ = 2719 kg/m³, cp = 871 J/(kg·K))
- Compartment 1: Passive devices (negligible heat dissipation, q ≈ 0 W)
- Compartment 2: Active devices (total heat dissipation Q = 40 W)

### Flow Conditions
- Cooling fluid: Atmospheric air
- Inlet temperature: T∞ = 35°C (308.15 K)
- Flow velocity: u∞ = 4 m/s
- Flow direction: Air encounters passive compartment first, then active compartment

### Design Configurations

**Baseline: Flat Bottom Heat Sink**
- Simple flat plate (36 cm × 36 cm)
- Surface area: 0.1296 m²

**Enhanced Design 1: Rectangular Fins**
- 10 longitudinal fins
- Dimensions: 30 mm height × 3 mm thickness × 30 mm spacing
- Surface area increase: approximately 2.7× baseline

**Enhanced Design 2: Triangular Fins**
- 10 longitudinal triangular fins
- Dimensions: 30 mm height × 30 mm base width (tapered to point)
- Surface area increase: approximately 2.5× baseline
- Material volume: approximately 50% of rectangular fins

## License

All educational content, geometry files, and documentation in this repository are licensed under the Creative Commons Attribution 4.0 International License (CC BY 4.0).

You are free to:
- **Share**: Copy and redistribute the material in any medium or format
- **Adapt**: Remix, transform, and build upon the material for any purpose, even commercially

Under the following terms:
- **Attribution**: You must give appropriate credit, provide a link to the license, and indicate if changes were made

## Citation

If you use these materials in your teaching or research, please cite:

```
[Anju R Gupta]. (2025). Electronics Cooling with ANSYS Fluent: A Hands-On Experiential Workshop. 
GitHub repository. https://github.com/anjurgupta/fluent-electronics-cooling-workshop
```

**Questions or suggestions?** 
- Open an issue in this repository
- Contact: anju.gupta@utoledo.edu

**Adopting this workshop at your institution?** 
I would love to hear about it! Please let us know so we can build a community of practice.

## Acknowledgments

- Problem adapted from Çengel, Y. A., & Ghajar, A. J. (2020. *Heat and Mass Transfer: Fundamentals and Applications* (6th ed.). McGraw-Hill.
- ANSYS for providing free Student software that enables accessible engineering education worldwide

## Additional Resources

### Heat Transfer Fundamentals
- Bergman, T. L., Lavine, A. S., Incropera, F. P., & DeWitt, D. P. (2011). *Fundamentals of Heat and Mass Transfer* (7th ed.). Wiley.
- Çengel, Y. A., & Ghajar, A. J. (2020). *Heat and Mass Transfer: Fundamentals and Applications* (6th ed.). McGraw-Hill.

### CFD and Thermal Management
- Versteeg, H. K., & Malalasekera, W. (2007). *An Introduction to Computational Fluid Dynamics: The Finite Volume Method* (2nd ed.). Pearson.
- Incropera, F. P. (2011). *Introduction to Heat Transfer* (6th ed.). Wiley.

### ANSYS Fluent Resources
- ANSYS Fluent User's Guide (included with software installation)
- ANSYS Innovation Courses: [https://innovationspace.ansys.com](https://innovationspace.ansys.com)


