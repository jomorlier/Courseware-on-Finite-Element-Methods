## Courseware on Finite Element Methods
This courseware on Finite Element Methods addresses standard and advanced Finite Element formulations for shear-deformable lightweight structures of the Timoshenko beam and Reissner-Minldin plate types.\
\
Moreover, the interactive courseware uses extensively the MATLAB&reg; Live Editor and the Symbolic Math Toolbox&trade; for the development and the presentation.\
\
Additionally, a comprehensive (but not exhaustive) set of MATLAB Grader assignments for this material exist. These assignments touch upon the topics mentioned in each of the chapters in the courseware syllabus. Please reach out to Andreas Apostolatos ([aapostol@mathworks.com](aapostol@mathworks.com)) to request access to the underlying MATLAB Grader assignments.

## Owner/s
Andreas Apostolatos, PhD ([aapostol@mathworks.com](aapostol@mathworks.com))

## Contents
The repository contains the following Live Scripts and folders:

- **``CoursewareonFiniteElementMethods.prj``**\
This is the MATLAB project file which sets up all necessary dependencies

- **``main.mlx``**\
This is the main document that can be used to navigate to the rest of the Live Scripts in the repository

- **``main_unitTests.mlx``**\
This is the Live Script that executes the unit tests

- **``1_BasisFunctions/``**\
This folder contains the Live Script addressing the construction of the Finite Element basis functions
  - **``main_Chapter1_BasisFunctions.mlx``**
![](https://git@github.com/andreasapostolatos/Courseware-on-Finite-Element-Methods.git/animations/basis_functions.gif)

- **``2_TimoshenkoBeam/``**\
This folder contains the Live Script addressing the variational formulation and Finite Element approximation of the Timoshenko beam problem
  - **``main_Chapter2_ALinearStraightTimoshenkoBeamElement.mlx``**

- **``3_ReissnerMindlinPlate/``**\
This folder contains the Live Scripts addressing the variational formulation and Finite Element approximation of the Reissner-Mindlin plate problem
  - **``3_ReissnerMindlinPlate.mlx``**

- **``4_TransverseShearLocking/``**\
This folder contains the Live Scripts highlighting and addressing the transverse-shear locking:
  - **``main_Chapter4_Locking_Timoshenko_beam.mlx``**
  - **``main_Chapter4_Locking_ReissnerMindlin_cantilever_plate.mlx``**
  - **``main_Chapter4_Locking_ReissnerMindlin_TwoSidedClampedPlate.mlx``**

- **``5_WeakDirichletBoundaryConditions/``**\
This folder contains the Live Script addressing the weak application of Dirichlet boundary conditions for the Timoshenko beam problem
  - **``main_Chapter5_WeakBoundaryConditions_TimoshenkoBeam.mlx``**

- **``6_HellingerReissnerFormulation/``**\
This folder contains the Live Scripts addressing the variational formulation of the Timoshenko beam problem by means of the Hellinger-Reissner principle
  - **``main_Chapter6_HellingerReissnerFormulation_TimoshenkoBeam.mlx``**
  - **``main_Chapter6_HellingerReissnerFormulation_TimoshenkoBeam_Study.mlx``**

- **``AppexA_EfficiencyConsiderations/``**\
This folder contains the Live Scripts demonstrating the runtime performance speedup by using page-wise computation of the element stiffness matrices and sparse assembly
  - **``main_AppexA_EfficiencyCondiderationsReissnerMindlinPlate.mlx``**
  - **``main_AppexA_EfficiencyCondiderationsTimoshenkoBeam.mlx``**

- **``TimoshenkoBeam/``**\
This folder contains all functions needed for the Finite Element discretization of the Timoshenko beam problem

- **``EulerBernoulliBeam/``**\
This folder contains all functions needed for the Finite Element discretization of the Bernoulli beam problem

- **``ReissnerMindlinPlate/``**\
This folder contains all functions needed for the Finite Element discretization of the Reissner-Mindlin plate problem

- **``utilityFunctions/``**\
This folder contains all auxiliary functions, such the computation of the basis functions, functions related to visualization and functions for the numerical integration among others

- **``unitTest/``**\
This folder contains all classes and functions needed for the unit testing performed by means of the Live Script ``main_unitTests.mlx``

## Concepts
Finite Element Methods, lightweight structures, Timoshenko beam, Reissner-Mindlin plate, transverse-shear locking, high-order basis functions, assumed natural strain, Hellinger-Reissner principle, slenderness study, convergence study, analytical solutions, Live Functions, Local Functions, Symbolic Math Toolbox&trade, plotting, unit-testing, Git-integration, ...

## Suggested Audience
All engineering disciplines, such as, civil engineers, mechanical engineers, etc.

## Time
20 minutes

## Workflow
Firstly, open the project file CoursewareonFiniteElementMethods.prj to have all the folder dependencies resolved. Then, open Live Script **main.mlx**, go to Section **Quick guide**, select any of the desirable Live Scripts from the list, and hit Run!

## Unit-testing framework
To run the unit tests for this courseware, just type the following commands in the Command Window of MATLAB\
``>> suite = matlab.unittest.TestSuite.fromProject("CoursewareonFiniteElementMethods.prj");``\
``>> run(suite)``\
Alternatively, start the project and then run the file ``main_unitTests.mlx``

## Release last tested
R2022b

## TODO
List out whatever you think is yet to be done here. Maybe someone else already has done this and can share it with you.

## Revision History
Add a short description of your changes here.