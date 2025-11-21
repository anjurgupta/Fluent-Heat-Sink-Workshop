# Electronics Cooling with ANSYS Fluent: A Hands-On Experiential Workshop

This experiential learning workshop uses free ANSYS Fluent Student software to explore thermal management of electronics through computational simulation. The workshop is designed for undergraduate heat transfer students and emphasizes hands-on discovery of heat sink design principles through computational fluid dynamics (CFD) without formal assessment or grading pressure.

## Learning Objectives

By the end of this workshop, students will be able to:

- Create computational meshes appropriate for conjugate heat transfer problems
- Set up and solve forced convection simulations in ANSYS Fluent
- Visualize temperature distributions and heat transfer mechanisms using CFD post-processing tools
- Compare heat sink geometries to inform engineering design decisions
- Discover through simulation why triangular fins offer superior material efficiency compared to rectangular fins

## The Challenge

A telecommunications system consists of two adjacent compartments sharing a common aluminum base plate that functions as an air-cooled heat sink. The system dissipates 40W of heat that must be transferred to atmospheric air flowing at 4 m/s over the base plate at an inlet temperature of 35°C.

**Your mission**: Determine if a flat base plate (36 cm × 36 cm) can keep the electronics within safe operating temperatures. When you discover through simulation that it cannot, design enhanced heat sink geometries and compare their thermal performance.

**Key learning insight**: Through direct computational experience, students discover that triangular fins achieve approximately 95% of rectangular fin performance while using 50% less material—demonstrating engineering optimization principles more powerfully than traditional lectures.

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
   git clone https://github.com/anjurgupta/fluent-electronics-cooling-workshop
   ```



## Learning Outcomes

### Bloom's Taxonomy Alignment

**Apply**: Execute complete CFD workflows from geometry creation through post-processing

**Analyze**: Interpret temperature distributions, velocity fields, and heat transfer mechanisms

**Evaluate**: Compare competing heat sink designs using quantitative simulation evidence

**Create**: Design optimized heat sink configurations balancing multiple objectives (thermal performance, material usage, manufacturability)

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

See the [LICENSE](LICENSE) file for complete details.

## Citation

If you use these materials in your teaching or research, please cite:

```
[Anju R Gupta]. (2025). Electronics Cooling with ANSYS Fluent: A Hands-On Experiential Workshop. 
GitHub repository. https://github.com/anjurgupta/fluent-electronics-cooling-workshop
```

## Contact and Support

**Questions or suggestions?** 
- Open an issue in this repository
- Contact: anju.gupta@utoledo.edu

**Adopting this workshop at your institution?** 
I would love to hear about it! Please let us know so we can build a community of practice.

## Acknowledgments

- Problem adapted from classical heat transfer textbook problems in electronics cooling
- ANSYS for providing free Student software that enables accessible engineering education worldwide

## Additional Resources

### Heat Transfer Fundamentals
- Bergman, T. L., Lavine, A. S., Incropera, F. P., & DeWitt, D. P. (2011). *Fundamentals of Heat and Mass Transfer* (7th ed.). Wiley.
- Çengel, Y. A., & Ghajar, A. J. (2014). *Heat and Mass Transfer: Fundamentals and Applications* (5th ed.). McGraw-Hill.

### CFD and Thermal Management
- Versteeg, H. K., & Malalasekera, W. (2007). *An Introduction to Computational Fluid Dynamics: The Finite Volume Method* (2nd ed.). Pearson.
- Incropera, F. P. (2011). *Introduction to Heat Transfer* (6th ed.). Wiley.

### ANSYS Fluent Resources
- ANSYS Fluent User's Guide (included with software installation)
- ANSYS Innovation Courses: [https://innovationspace.ansys.com](https://innovationspace.ansys.com)

**Ready to begin? Download ANSYS Student and explore computational thermal design through hands-on discovery.**
