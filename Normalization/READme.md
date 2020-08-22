The jupyter notebook is used to normalize spectrum of the stars. It reads a file and lets you decide if you want to fit it. 
If you enter yes it will give you the option of what wavelength range to fit. If you like the fit you can save it but if 
you don't you can keep fitting it. Ones you are satisfied with the fit you can save it and move on to another range of the
same spectrum or go to the next star spectrum. 

How does the code go about fitting the spectrum?
It takes the data points in the wavelength range you have decided to fit. It finds relative maximum using "argrelmax" function 
from the "scipy.signal" library. The found point ar fitted by a 3rd degree polynomial. The fit is divided out of the data resulting 
in a normalized star spectrum. Since the fits are done within ranges of an overall spectrum the corresponding wavelenght ranges, 
relative maximum, and polynomial  fits and parameters are saved in various files. The files are saved to be used in later analysis.
