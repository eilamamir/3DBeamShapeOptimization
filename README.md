# 3DBeamShapeOptimization
Please read this readme notes carefully prior to using the supplied code:

1. General
The provided code with all subroutines is the code used for the paper: "Free form shape optimization of three dimensional beams using cross section analysis"
in https://doi.org/10.1016/j.ijsolstr.2023.112331. two main functions are added: 1) 'SingleBeam.m' and 2) 'SingleBeamEigen.m'. The first solves the compliance
minimization problem and the second solves the fundamental frequency maximization problem. Follow the help for instructions (or the comments at the beginning of the function).

2.Terms and Conditions:

	2.1 If you found this material useful for your research and you wish to report your study. Please cite the aforementioned paper.
	2.2 The supplied code uses the BECAS software, a third party software with a license only for the aforementioned study.
	Using this software for your study is allowed only with proper license or agreement from the supplier. Please visit https://becas.dtu.dk/licensing for further details.
	2.3 The supplied code uses licensed MMA subroutines in MATLAB format. MMA is a licensed software, for term and conditions of use please refer to the specific 			commercial or academic agreement made with Professor Krister Svanberg from KTH university at: krille@math.kth.se. or via researchgate at: 	https://www.researchgate.net/profile/Krister-Svanberg.
	2.4 The supplied code uses the function inpoly.m by Darren Engwirda. The terms of use of this function is by properly citing
	IMPORTANT: Unauthorized use of the BECAS software or the MMA subroutines may result in infringement of intellectual property rights

3. Operating:
 
	Inside the SingleBeam.m and SingleBeamEigen.m some internal functions are cascaded, yet it also uses some external functions, located at the 'Misc' directory.
	For further details see the readme file in 'Misc'.

	It calls the BECAS subroutines in order to calculate the cross section properties. These functions are located in 'BECASv3.3' directory.

	In addition, the sensitivities as well as the constitutive calculation of the cross section is calculated using subroutines located at 'BeamCalcBECAS' directory.

	As the shape optimization is based on bspline modeling of cross sections, some essential subroutines are located in the 'bsplines' directory.

	Finally, as the shape optimization is based on the gradient approach and uses the Method of Moving Asymptotes for the convex approximation, the required 	subroutines are located at 'MMA subroutines' directory.
	
4. Disclaimer:

	The supplied code has been debugged with the best effort of the provider. Yet, it still may have programming and unintended issues which has not yet screened out. 	The 	provider shall not be held responsible for any inadvertent errors or omissions, due to those issues.
