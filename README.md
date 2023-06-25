# MOFKit
A script for remove solvents molecule in MOFs framwork

[usage]: rm_mof_solvents.py [-h] [-d SKIN_DISTANCE] [-s] [-m] cif_in output_path

        positional arguments:
        cif_in                input MOF cif file
        output_path           Output filepath
        
        optional arguments:
        -h, --help            show this help message and exit
        -d SKIN_DISTANCE, --skin_distance SKIN_DISTANCE
                                The skin distance(coefficient) you want to use
                                (default=0.25). 
                                Because there are two ways to determine whether a bond is between two atoms.
                                1) skin_distance 0.25 
                                2) coefficient  1.2 (recommend !) 
                                Both methods are preserved in this script
        -s, --solvent         Display the solvent molecules was found but not removed and create new cif file 
        -c, --cmp             Compare with the existing solvent list, if it does not exist, do not delete the molecule

