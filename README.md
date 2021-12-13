# ADD_CMAP for ff99OL3_CMAP1
## Add CMAP parameters into original AMBER prmtop file
This script is used to add CMAP parameters into the prmtop file which is generated by tleap module of AMBER packages. This script provides interacting command lines to add CMAP parameters to the residues of interest and the silent mode to skip these interacting command lines and add CMAP parameters to all residues.

Usage: ./ADD-CMAP -p amber.prmtop -c CMAP_parameters -o amber_addCMAP.prmtop [-s]

```
Explanation:
-p      Required.
        Input AMBER PRMTOP file generated with tleap or xleap.
-o      Required.
        Output AMBER PRMTOP file with CMAP energy term.
-c      Optional.
        Specify user edited CMAP parameter file.
        Default CMAP file is ./CMAP_parameter.
-s      Silent Mode, optional.
        Run the script silently without any interacting UI.
        Note: In silent mode, all the proteins/RNAs in the PRMTOP would
        be considered to be added.

-h      Show this help information.
-v      Show version information.
```
**Note: When adding the ff99OL3_CMAP1.para, do not use silent mode and do not add environmentally specific parameters.**
