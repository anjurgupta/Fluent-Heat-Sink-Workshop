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
   git clone https://github.com/yourusername/fluent-electronics-cooling-workshop
   ```
3. **Review heat transfer basics**: Read `reference-materials/convection-review.pdf`
4. **Day 1**: Follow step-by-step instructions in `workshop-materials/day1-meshing/student-handout-day1.pdf`
5. **Day 2**: Follow step-by-step instructions in `workshop-materials/day2-solution/student-handout-day2.pdf`

### For Instructors

1. **Review pedagogy framework**: Read `pedagogy-documentation/experiential-learning-framework.md` to understand the educational philosophy
2. **Study facilitation guides**: 
   - `workshop-materials/day1-meshing/instructor-guide-day1.md`
   - `workshop-materials/day2-solution/instructor-guide-day2.md`
3. **Test geometry files**: Load and verify all `.scdoc` files work in your ANSYS installation
4. **Prepare lab environment**: Ensure ANSYS Student is installed on lab computers or students bring laptops with software pre-installed

## Repository Structure

```
fluent-electronics-cooling-workshop/
│
├── README.md                          # This file
├── LICENSE                            # Creative Commons CC-BY-4.0
├── CONTRIBUTING.md                    # Guidelines for contributions
│
├── workshop-materials/
│   ├── day1-meshing/
│   │   ├── instructor-guide-day1.md       # Facilitation tips and timing guidance
│   │   ├── student-handout-day1.pdf       # Step-by-step instructions for students
│   │   ├── slides-introduction.pdf        # Opening presentation materials
│   │   └── mesh-quality-checklist.pdf     # Self-assessment tool
│   │
│   ├── day2-solution/
│   │   ├── instructor-guide-day2.md       # Solution setup walkthrough
│   │   ├── student-handout-day2.pdf       # Boundary condition reference guide
│   │   ├── slides-heat-sinks.pdf          # Fin geometry concepts presentation
│   │   └── results-comparison-template.xlsx  # Data collection spreadsheet
│   │
│   └── reference-materials/
│       ├── convection-review.pdf          # Heat transfer fundamentals refresher
│       ├── fluent-basics-guide.pdf        # Interface navigation primer
│       └── heat-sink-design-primer.pdf    # Extended reading on thermal management
│
├── geometry-files/
│   ├── baseline-flat-plate.scdoc          # SpaceClaim geometry files
│   ├── rectangular-fins.scdoc
│   ├── triangular-fins.scdoc
│   └── README.md                          # Geometry specifications and dimensions
│
├── sample-meshes/                         # Pre-generated meshes for reference
│   ├── baseline-coarse.msh
│   ├── baseline-medium.msh
│   ├── rectangular-fins.msh
│   ├── triangular-fins.msh
│   └── mesh-metrics-summary.pdf           # Quality metrics for each mesh
│
├── tutorial-videos/                       # Links to screen capture tutorials
│   ├── 01-geometry-creation.md
│   ├── 02-meshing-workflow.md
│   ├── 03-solution-setup.md
│   └── 04-postprocessing.md
│
├── sample-results/                        # Instructor solutions for troubleshooting
│   ├── baseline-results/
│   │   ├── temperature-contours.png
│   │   ├── velocity-vectors.png
│   │   └── quantitative-summary.txt
│   ├── rectangular-fins-results/
│   └── triangular-fins-results/
│
└── pedagogy-documentation/
    ├── learning-objectives.md             # Bloom's taxonomy alignment
    ├── facilitation-tips.md               # Handling common student questions
    ├── experiential-learning-framework.md # Educational theory background
    └── adaptation-guide.md                # Modifying for different contexts
```

## Pedagogical Innovation

This workshop embodies experiential learning principles:

### Learning by Doing
Students construct knowledge through hands-on CFD simulation rather than passive lecture consumption.

### Productive Struggle
The discovery that a flat plate cannot adequately cool the electronics creates authentic motivation for heat sink design exploration.

### No Assessment Pressure
The informal learning environment encourages experimentation and risk-taking without concern for grades.

### Student-Centered Approach
The instructor facilitates discovery rather than delivering content. Students drive their own exploration and learning.

### Real-World Problem
Electronics thermal management mirrors authentic industry challenges in telecommunications, computing, and power electronics.

### Educational Framework
Aligns with Kolb's Experiential Learning Cycle and constructivist pedagogy. Students progress through:
- **Experience**: CFD simulation of heat sink configurations
- **Reflection**: Why did certain designs fail or succeed?
- **Conceptualization**: Understanding heat transfer principles
- **Experimentation**: Testing new design variations

## Workshop Structure

### Day 1: Geometry and Meshing (3-4 hours)

**Session 1.1: Introduction** (30 minutes)
- CFD fundamentals and thermal management overview
- Real-world applications of electronics cooling
- Workshop objectives and expectations

**Session 1.2: Software Setup** (20 minutes)
- ANSYS Student installation verification
- Interface navigation and workspace familiarization

**Session 1.3: Geometry Creation** (60 minutes)
- Create baseline flat plate heat sink in SpaceClaim
- Design rectangular fin configuration
- Design triangular fin configuration
- Define flow domain and boundary surfaces

**Session 1.4: Mesh Generation** (90 minutes)
- Meshing strategy for conjugate heat transfer
- Boundary layer mesh requirements
- Generating meshes for all three geometries
- Understanding mesh quality metrics

**Session 1.5: Quality Verification** (30 minutes)
- Self-assessment using provided checklist
- Peer review of mesh quality
- Troubleshooting common meshing issues

### Day 2: Solution and Design Comparison (3-4 hours)

**Session 2.1: Physics Setup** (60 minutes)
- Solver configuration (pressure-based, steady-state)
- Turbulence modeling selection
- Material properties for air and aluminum
- Boundary condition specification
- Heat source definition

**Session 2.2: Solution and Convergence** (45 minutes)
- Solution initialization
- Monitoring convergence criteria
- Troubleshooting convergence issues
- Understanding residual plots

**Session 2.3: Post-Processing** (60 minutes)
- Creating temperature contours and velocity vectors
- Quantitative data extraction
- Heat transfer coefficient calculations
- Energy balance verification
- **The Discovery Moment**: Realizing flat plate temperature exceeds safe limits

**Session 2.4: Heat Sink Comparison** (75 minutes)
- Solving rectangular fin configuration
- Solving triangular fin configuration
- Comparative analysis of thermal performance
- Material efficiency calculations
- **Engineering Insight**: Triangular fins offer superior material efficiency

**Session 2.5: Free Exploration** (Optional, 30 minutes)
- Parametric studies: fin spacing, height, number
- Velocity variations
- Alternative materials

## Learning Outcomes

### Bloom's Taxonomy Alignment

**Apply**: Execute complete CFD workflows from geometry creation through post-processing

**Analyze**: Interpret temperature distributions, velocity fields, and heat transfer mechanisms

**Evaluate**: Compare competing heat sink designs using quantitative simulation evidence

**Create**: Design optimized heat sink configurations balancing multiple objectives (thermal performance, material usage, manufacturability)

Detailed learning objectives with assessment criteria available in `pedagogy-documentation/learning-objectives.md`

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

## Transferability and Adoption

### Why This Workshop is Highly Adoptable

**Zero Software Cost**: ANSYS Student is completely free with no license requirements

**Minimal Hardware Requirements**: Runs on typical student laptops with Windows 64-bit

**Comprehensive Open Materials**: All necessary resources provided in this GitHub repository

**Flexible Integration Options**: 
- Standalone 2-day workshop
- Integrated module within heat transfer course
- Summer outreach program
- Senior capstone preparation

**Scalable**: Suitable for 10-30 students with single instructor

**No Prerequisites**: Appropriate for first exposure to CFD simulation

**Replicable Results**: Well-posed problem with predictable outcomes

### Potential Adaptations

- Other thermal problems: heat exchangers, building HVAC, battery thermal management
- Other CFD applications: aerodynamics, microfluidics, mixing processes
- Different software platforms: OpenFOAM for open-source alternative
- Online/hybrid delivery using screen sharing and virtual collaboration tools
- Extension to graduate-level optimization techniques

## Contributing

This is an open educational resource and contributions are welcome:

- Additional geometry configurations or design challenges
- Extended tutorial materials and worked examples
- Video tutorials and screencasts
- Translations to other languages
- Adaptations for different engineering contexts
- Troubleshooting guides for common student issues

Please see `CONTRIBUTING.md` for detailed guidelines on how to contribute to this project.

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
[Your Name]. (2025). Electronics Cooling with ANSYS Fluent: A Hands-On Experiential Workshop. 
GitHub repository. https://github.com/yourusername/fluent-electronics-cooling-workshop
```

## Contact and Support

**Questions or suggestions?** 
- Open an issue in this repository
- Contact: [your email or institutional contact]

**Adopting this workshop at your institution?** 
We'd love to hear about it! Please let us know so we can build a community of practice.

## Acknowledgments

- Problem adapted from classical heat transfer textbook problems in electronics cooling
- ANSYS for providing free Student software that enables accessible engineering education worldwide
- Engineering education community for developing experiential learning pedagogies
- [Your institution] for supporting innovative undergraduate curriculum development

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

### Experiential Learning in Engineering Education
- Kolb, D. A. (1984). *Experiential Learning: Experience as the Source of Learning and Development*. Prentice Hall.
- Prince, M. J., & Felder, R. M. (2006). Inductive teaching and learning methods: Definitions, comparisons, and research bases. *Journal of Engineering Education*, 95(2), 123-138.

---

**Ready to begin? Download ANSYS Student and explore computational thermal design through hands-on discovery.**
