# *Energy Characterization of Graph Workloads* Data

The `EnergyCharacterizationAverageData.csv` file contains the GAP benchmark kernels' energy characterization data. The detailed data analysis can be found at:

 - Ankur Limaye, Antonino Tumeo, and Tosiron Adegbjija, "*Energy Characterization of Graph Workloads*," in Sustainable Computing: Informatics and Systems Journal.
 - The paper was presented at the 11th International Green and Sustainable Computing Conference (IGSC '20), 19 -- 22 October 2020.

## Experimental Setup

Our experimental setup was:
- Six GAP benchmark kernels -- *bc*, *bfs*, *cc*, *pr*, *sssp*, and *tc*
- Twelve input graphs -- 
	- 9 synthetic Kronecker graphs with varying scales and degrees (*kron-g20-k4*, *kron-g20-k8*, *kron-g20-k16*, *kron-g22-k4*, *kron-g22-k8*, *kron-g22-k16*, *kron-g24-k4*, *kron-g24-k8*, and *kron-g24-k16*)
	- 3 real-world graphs: *road*, *twitter*, and *road*
- Four system configurations -- *Single-socket Multithreading (SS-MT)*, *Single-socket Simultaneous Multithreading (SS-SMT)*, *Dual-socket Multithreading (DS-MT)*, and *Dual-socket Simultaneous Multithreading (DS-SMT)*

## Data Format

Each column of the CSV file contains the performance counter data for each GAP kernel executing various input graphs for the different system configurations. The `key` column contains the entries in the following format:

*Kernel*---*Graph*---*#Threads*---*#Processors*---*Threads/Core*---*Simultaneous_Multithreading_Enabled?*

For example, *bc-kron-g20-k4-t1-1s-1tpc-nh* implies *bc* kernel executing the *kron-g20-k4* input graph, with #threads = 1, #processors = 1, and simultaneous multithreading disabled (i.e., 1 thead per core)
