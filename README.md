# Qhack-qnyble

This is the repository for the development of Xanadu's Qhack Open hackathon challenge. Our team, qnyble, is conformed by:
- Saasha Joshi (saashajoshi08@gmail.com)
- Tristan Zaborniak (tsmzaborniak@gmail.com)
- Juan Giraldo (juanfer021299@gmail.com)

## Project description

RNAs are nucleotide polymers fundamental to a diversity of elementary biological functions, including the (de)coding and regulation of genes, protein construction, cellular signaling, and catalysis [1]. Integral to these roles is the capacity and propensity of RNAs to self-interact through hydrogen-bond base-pairing between nucleotides and fold into specific, stable structures [2]. This folded structure of an RNA along with its primary sequence chemistry combine to dictate its interactions with other biomolecules [3]. Understanding and predicting RNA folding is thus a pressing interest of the biological sciences, basic and applied [4, 5].

RNA folding prediction from primary sequence information alone remains challenging classically, viewed from both the standpoints of chemical dynamics and combinatorial optimization of free energy. Quantum approaches, with their demonstrable advantage in both of these realms, therefore lend themselves well to the RNA folding problem. To our knowledge, only one attempt has been made to map RNA folding to quantum computing, via quantum annealing [6]. With this project, we seek to: (1) modify the Hamiltonian presented therein to better reflect the underlying chemistry of base-pairing, and (2) optimize the free parameters of the Hamiltonian against a suite of RNAs with known structures. Expanding on (2), we aim to implement and test our Hamiltonian with the quantum annealing hardware of D-Wave, and demonstrate a parallel approach with gate-based hardware via QAOA, using the very same Hamiltonian.


## Project organization

The first part of this project is located in the file: qrna_folding_annealing.ipynb, where we use D-wave's SDK, Ocean, to build the annealing solution for the RNA folding problem. For the gate-based implementation we created the file: qrna_folding_qaoa.ipynb where we use the QAOA implementation of Qiskit to find the optimal solution for the proposed Hamiltonian. Lastly we added a folder containing a dataset with multiple RNA from bpRNA sequences of different size (from 20 to 400 bases) and type (known to contain pseudoknots, pseudoknot-free). These are used as inputs for each implementation of our methodology.

## References

[1] J. Li and C. Liu, “Coding or noncoding, the converging concepts of RNAs,” Frontiers in
Genetics, vol. 10, May 2019.    
[2] G.L.Conn and D.E.Draper,“RNAstructure,”Current Opinion in Structural Biology,vol.8,
no. 3, pp. 278–285, Jun. 1998.    
[3] S. R. Holbrook, “RNA structure: the long and the short of it,” Current Opinion in Structural
Biology, vol. 15, no. 3, pp. 302–308, Jun. 2005.     
[4] M. D. Disney, “Targeting RNA with small molecules to capture opportunities at the intersec-
tion of chemistry, biology, and medicine,” Journal of the American Chemical Society, vol.
141, no. 17, pp. 6776–6790, Mar. 2019.   
[5] N. G. Walter and L. E. Maquat, “Introduction—RNA: From single molecules to medicine,”
Chemical Reviews, vol. 118, no. 8, pp. 4117–4119, Apr. 2018.    
[6] D. M. Fox, C. M. MacDermaid, A. M. Schreij, M. Zwierzyna, and R. C.
Walker, “RNA folding using quantum computers,” May 2021.    


