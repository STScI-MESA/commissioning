# Convert DMS (flight-like) to FITSWriter (ground-like) format

This script takes a configuration file with pairs of FITS header keyword/EngDB mnemonics and queries the EngDB for the first mnemonic value during the exposure and assigns its value to the specified FITS header keyword.
It also makes the transformation from DMS coordinates to Detector coordinates and reshapes data from 4-D to 3-D arrays adding reference output for MIRI data.

## Usage
An example configuration file ``tlm.cfg`` is included.

The script can be run with
``python flight2ground.py tlm.cfg inputs.fits output.fits``
