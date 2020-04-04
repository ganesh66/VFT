# VFT

ERROR: u,v are not diverging, by 5th or 6th iteration values are blowing up to infinity.

Possible Reasons Behind the errors:

1.Initializing u1,v1 with RK 1st order messes up the convergence of Adam-Bashforth 2nd order

2.assumption of body force=0 is wrong.
	
	(Try to add gravity in the next commit)

3.assumptions behind using  Fourier-Fourier approximation (i.e F,V are periodic) is invalid.
	
	(Try Chebyshev-Fourier Approximation or  Chebyshev-Chebyshev approximation)
