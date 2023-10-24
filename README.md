# NiP

## Structure of data.ascii files

First sections are summmary of descriptors used (not fully understood yet)

For each .xsf structure we have
* A misterious line with an integer number (84 or 85 in our case, not sure what it is)
* A line with the path+filename
    '/bsuhome/mdsharifkhan/scratch/khan/nip/pytorch_training/screening/xsf/nip_1400_1.xsf'
* A line with number of atoms and number of atom types
    96           2
* A line with the energy/atom of that configuration
   82.116713019096807     
* For each atom in the system (96 in our case)
    * A line with the atom type 
        1
    * Two lines with the Cartesian coordinates and the forces on that atom
       1.8352002409498394        1.7772295420213304        3.0008403876088163     
       7.4717800528864869E-002  0.94356426406430416       -4.4902259829329112E-002
    * A line with the number of symmetry functions
       44
    * The values of the symmetry functions
       32.544199479547466        3.4987752098567797      ...
