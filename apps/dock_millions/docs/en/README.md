# Description

By using Autodock-GPU and Vdock, docking results are obtained for more than 5 million small molecules.

# Inputs

- `protein receptor` [5UOR.A_protein.pdb](https://docs.ad3.io/media/apps/dock_millions/examples/input/5UOR.A_protein.pdb)
- Number of iteration : Number of iterations of retraining for docking and machine learning
- Initial screen data : The first docked data, a database clustered using similarity
  - NR10 : similarity < 10, approx. 6,000
  - NR15 : similarity < 15, approx. 35,000
  - NR20 : similarity < 20, approx. 140,000
- Screen data
  - Mcule purchasable : Mcule's instock compounds, approx. 5M
  - Enamine lead-like : Enamine's Real Diversity set, approx. 38.2M
- Docking number of data

# Outputs

- [vdock_screening.dock.BINDING_E.pdbqt](https://docs.ad3.io/media/apps/dock_millions/examples/output/vdock_screening.dock.BINDING_E.pdbqt) : Best ligand 3d file
- [vdock_screening.dock.receptor.pdb](https://docs.ad3.io/media/apps/dock_millions/examples/output/vdock_screening.dock.receptor.pdb) : Protein receptor 3d file
- [vdock_screening.dock.report.tsv](https://docs.ad3.io/media/apps/dock_millions/examples/output/vdock_screening.dock.report.tsv) : Best ligand data

# References

1. Diogo Santos-Martins, Leonardo Solis-Vasquez, Andreas F Tillack, Michel F Sanner, Andreas Koch, Stefano Forli. Accelerating AutoDock4 with GPUs and Gradient-Based Local Search J. Chem. Theory Comput. 2021, 17, 2, 1060–1073
2. Choi, J. & Lee, J. V-Dock: Fast Generation of Novel Drug-like Molecules Using Machine-Learning-Based Docking Score and Molecular Optimization. Int J Mol Sci 22, 11635 (2021). Journal
3. [Mcule database](https://mcule.com/database/)
4. [Enamine database](https://enamine.net/compound-collections/real-compounds/real-database-subsets)
