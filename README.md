# GMDA: Foundations of Geometric Methods in Data Analysis
### Supervisors: 
#### * [Frédéric Cazals, Inria ABS](https://team.inria.fr/abs/team-members/homepage-frederic-cazals/)
#### * [Fred Chazal, Inria DataShape](https://geometrica.saclay.inria.fr/team/Fred.Chazal/)

# Project: Circumventing distance concentration phenomena

# Description:
Several strategies can be developed to deal with distance concentration phenomena. One of them, consists in using suitable norms, and to project to lower dimensional spaces. Another one, consists in using a biasing potential which aims at focusing on the most informative distances only. In this project, we aim at applying the latter to a diﬀerent molecular data set, namely an ensemble of conformations of a protein model known as BLN69. In a nutshell, BLN69 is a linear chain of 69 beads; since each bead has 3 cartesian coordinates, a conformation is deﬁned by a point in dimension d = 3×69 = 207. To each conformation, one can also associate an energy, which will be given along with the conformations. Finally, to measure the distance between two conformations, we shall use the least root mean square deviation.

`persistance.R:` cretating persistance diagrams and saving the birth/death coordinates of the components in a dataframe.
`Report.ipynb:` going through two tasks showcasing the importance of persistance diagrams to classify low energy conformations and measure the 'distance' between them.
`Topo.ipynb:` data exploration, introducing the Kabsch algorithm to introduce a geometrical notion of __distance__ between conformations and 2D/3D projections using t-sne to motivate the intuition behind this analysis.

![Persistance diagram example][persistance.jpeg]
