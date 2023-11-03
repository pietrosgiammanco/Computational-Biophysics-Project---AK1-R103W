# File description
In this folder is located the original pdb file downloaded from ProteinDataBank.

# File Processing
The raw file was loaded into Chimera and all non-protein atoms were removed; there were no extra chains to remove.
The inspection of the sequence revealed the presence of some missing residues at the head and tail of the sequence. Comparing the sequence with the one in the UniProt database returned a perfect match and no residues needed correction.
Before applying the mutation a copy of this file was saved as WT_2C9Y.pdb, then the command 'swap aa trp :103' was used to mutate the protein (now saved as R103W_2C9Y.pdb)
While trying to build the topologies with gromacs some residues were found having some missing atoms, thus the files were repaired with the 'swap aa' command in Chimera until no errors occurred.
