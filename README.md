# GMDA: Foundations of Geometric Methods in Data Analysis
### Supervisors:
#### - [Frédéric Cazals, Inria ABS](https://team.inria.fr/abs/team-members/homepage-frederic-cazals/)
#### - [Fred Chazal, Inria DataShape](https://geometrica.saclay.inria.fr/team/Fred.Chazal/)

# Project: Circumventing distance concentration phenomena

# Description:
Several strategies can be developed to deal with distance concentration phenomena. One of them, consists in using suitable norms, and to project to lower dimensional spaces. Another one, consists in using a biasing potential which aims at focusing on the most informative distances only. In this project, we aim at applying the latter to a diﬀerent molecular data set, namely an ensemble of conformations of a protein model known as BLN69. In a nutshell, BLN69 is a linear chain of 69 beads; since each bead has 3 cartesian coordinates, a conformation is deﬁned by a point in dimension d = 3×69 = 207. To each conformation, one can also associate an energy, which will be given along with the conformations. Finally, to measure the distance between two conformations, we shall use the least root mean square deviation.

# Content:
`persistance.R:` cretating persistance diagrams and saving the birth/death coordinates of the components in a dataframe.

`Report.ipynb:` going through two tasks showcasing the importance of persistance diagrams to classify low energy conformations and measure the 'distance' between them.

`Topology.ipynb:` data exploration, introducing the Kabsch algorithm to introduce a geometrical notion of __distance__ between conformations and 2D/3D projections using t-sne to motivate the intuition behind this analysis.

## - Persistence diagram example
![Persistence diagram example](https://github.com/AlaaMahi/GMDA/blob/master/Persistance.jpeg "Persistence diagram example")

# Metrics:
## Root-mean-square-deviaton :
In bioinformatics, the root-mean-square deviation of atomic positions (or simply root-mean-square deviation, RMSD) is the measure of the average distance between the atoms (usually the backbone atoms) of superimposed proteins. Note that RMSD calculation can be applied to other, non-protein molecules, such as small organic molecules. In the study of globular protein conformations, one customarily measures the similarity in three-dimensional structure by the RMSD of the Cα atomic coordinates after optimal rigid body superposition.

## Kabsch algorithm :
The Kabsch algorithm, named after Wolfgang Kabsch, is a method for calculating the optimal rotation matrix that minimizes the RMSD (root mean squared deviation) between two paired sets of points. It is useful in graphics, cheminformatics to compare molecular structures, and also bioinformatics for comparing protein structures (in particular, see root-mean-square deviation (bioinformatics)). The algorithm only computes the rotation matrix, but it also requires the computation of a translation vector. When both the translation and rotation are actually performed, the algorithm is sometimes called partial Procrustes superimposition.
