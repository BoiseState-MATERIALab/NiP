# NiP Bulk Metallic Glasses

## A Dataset of DFT Simulations

The configurations reported in this database were generated using classical molecular dynamics (MD), using an embedded atom model (EAM) potential, as developed by Sheng et al. [1]. Simulations were performed over a range of temperatures and composition (ratio of P vs Ni). The quantum-mechanical total energy of configurations extracted from these MD simulations were then re-computed using density functional theory (DFT) as implemented in the [Quantum ESPRESSO](www.quantum-espresso.org) package [2]. 

More details on the generation of this database and on its use for training neural network interatomic potentials via the AENet package [3] can be found in:

`Md. S. Khan, N. Artith, and O. Andreussi, "Understanding Structure-Composition-Property Relationships of Ni-P Bulk Metallic Glasses", under review (2025)` 

## Authors
**Md. Sharif Khan**, Department of Chemistry and Biochemistry, Boise State University
**Oliviero Andreussi**, Department of Chemistry and Biochemistry, Boise State University

## Structure of the Dataset

The training dataset contains 20,000 structures saved in the XCrySDen structure format (XSF). 

For each .xsf structure we have:
* The total energy from a DFT calculation (Quantum Espresso), with details included in the NiP-qe.in file,
* The simulation cell vectors,
* The number of atoms in the configuration,
* For each atom in the system, the element, Cartesian coordinates, and forces on that atom.

## Acknowledgements
The authors thank Dr. Sundeep Mukherjee for the initial discussions that started this research project. N.A. acknowledges a start-up grant (Dutch Sector Plan) from Utrecht University. We thank Boise State for providing the startup funds that supported this research, together with the NSF CAREER award \#2306929.

## References

[1] H. W. Sheng, E. Ma, M. J. Kramer, "Relating Dynamic Properties to Atomic Structure in Metallic Glasses," *JOM*, vol. 64, no. 2, pp. 856–865, 2012. [https://doi.org/10.1007/s11837-012-0360-y](https://doi.org/10.1007/s11837-012-0360-y)
[2] P. Giannozzi et al., "QUANTUM ESPRESSO: a modular and open-source software project for quantum simulations of materials", J. Phys.: Cond. Mat., 39, 395502 (2009), [https://doi.org/10.1088/0953-8984/21/39/395502](https://doi.org/10.1088/0953-8984/21/39/395502)
[3] J. López-Zorrilla, X. M. Aretxabaleta, I.W. Yeu, I. Etxebarria, H. Manzano, and N. Artrith,"ænet-PyTorch: A GPU-supported implementation for machine learning atomic potentials training", J. Chem. Phys., 158, 164105 (2023), [https://doi.org/10.1063/5.0146803](https://doi.org/10.1063/5.0146803).