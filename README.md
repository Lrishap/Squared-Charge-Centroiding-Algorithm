SiPM Charge Estimate:
The first part of the code estimates the total amount of charge at individual SiPMs. The properties of Hammamatsu MPPC S14160-6050HS SiPM model is
used based on the specifications provided by the manufacturer. The total number of photons reaching at individual SiPMs for each event is obtained 
from the Geant4 Simulations.

Charge Centroiding Algorithm:
The total charge at each SiPMs relative to the individual position is weighted over the total charge output for each event to calculate the position
of the muon interaction event in the square grid.

Statistical Analysis:
A total of 5000 events were simulated for each spacing of the SiPMs in the grid (5, 10, 15, 20, 25 cm) at the center and the edge of the grid. A 2D histogram 
was obtained based on the calculated (X,Y) position from the centroiding algorithm. The 2D histogram was projected on the X-axis to obtain a Gaussian
fit and FWHM of the fit was calculated. A chi-squared test was performed to check the goodness of fit for the obtained Gaussian fit.

