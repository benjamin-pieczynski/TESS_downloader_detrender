# TESS_downloader_detrender
**About:** This notebook contains code modules that allow for the downloading of time-series photometry data from MAST given a target TIC number. Additional packages include a period finder and data detrender for  ELC implementation.

****

## How to use

After opening the notebook with jupyter notebook

1) Specify the download path and choose a target TIC number for a binary star system with visible transits.

2) Run the cells until reaching the File Reader section.

3) Select the TESS cadence to be considered when conducting light curve analysis.

4) Use the string length module to find the period within a specified range and step size.

5) Adjust the phase plot to fit the primary and secondary eclipses exactly.

6) Use the detrender to produce a detrended light curve centered around the eclipse time. This prepares the file for light curve synthesis codes, such as ELC (Oros & Hauschildt 2000). For the extended width parameter, make sure the extension would cover sufficient area out of eclipse in the phase plot while also not contacting other eclipses.

7) Run the remaining cells to save the detrended data to a file

****

## Dependencies

jupyter notebook

numpy

astroquery

astropy

matplotlib

os

json

requests

pandas

sklearn

scipy

****

## Installation

To install this repository git clone https://github.com/benjamin-pieczynski/TESS_downloader_detrender and open with jupyter notebook

****

## Future additions / improvements

Adding more options to the detrender other than just binary star eclipses.

****
