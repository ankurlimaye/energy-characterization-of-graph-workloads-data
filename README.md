# *Energy Characterization of Graph Workloads* Data

The `EnergyCharacterizationAverageData.csv` file contains the data analyzed and presented in the "Energy Characterization of Graph Workloads" paper, published in Elsevier's Sustainable Computing: Informatics and Systems Journal.

Each column of the CSV file contains the performance counter data for each GAP kernel executing various input graphs for different system configurations. The `key` column contains the entries in the following format:

*Graph_Kernel*---*Input_Graph*---*Thread_Count*---*Processor_Count*---*Threads_Per_Core*---*Simultaneous_Multithreading_Enabled*

For example, *bc-kron-g20-k4-t1-1s-1tpc-nh* implies *betweenness centrality (bc)* kernel executing the synthetic *kron-g20-k4* input graph, with number of threads = 1, number of processors = 1, and simultaneous multithreading disabled (1 thead per core)