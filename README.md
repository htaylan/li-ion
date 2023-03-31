# li-ion

The explanation of each column for bonds, angles and dihedrals are given in li_box_with_descriptions.lmpdat 
You can generate lmpdat files from pdb via OpenBabel. (http://openbabel.org/wiki/Category:Installation). Choose input format as pdb and output format as lmpdat.

## How to generate new boxes with different number of PEO and LiTFSI molecules  via inputfile.inp 
1) Change output name (li_box_900.pdb) 
2) structure peo.pdb read the coordinates of one PEO molecule. Change the "number" to desired number of molecules. 
3) inside box defines the size of the initial box. You can increase or decrease size by changing 50 50 50 to e.g. 75 75 75 or 30 30 30. 
4) structure litfsi.pdb read the coordinates of one LiTFSI molecule. Change the "number" to desired number of molecules. 
5) You can modify the size of the inital box in here too. But make sure they are same for the both molecules. 
6) Download packmol.exe, inputfile.inp, make sure they are in the same directory. 
7) Run it with the following command "packmole.exe < inputfile.inp"
