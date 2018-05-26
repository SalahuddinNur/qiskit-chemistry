# IBM Quantum Library for Chemistry

## Electronic structure driver for PyQuante2

PyQuante2 is an open-source library for computational chemistry, see https://github.com/rpmuller/pyquante2 for
installation instructions and its licensing terms.

This driver requires PyQuante2 to be installed and available for qiskit_acqua_chemistry to access/call.

## Input file example
To configure a molecule on which to do a chemistry experiment with qiskit_acqua_chemistry create a PYQUANTE section in the input file
as per the example below. Here the molecule, basis set and other options are specified as key value pairs. The 
molecule is a list of atoms in xyz coords separated by semi-colons ';'.  
```
&PYQUANTE
  atoms=H .0 .0 .0; H .0 .0 0.74
  units=Angstrom
  charge=0
  multiplicity=1
  basis=sto3g
&END
```