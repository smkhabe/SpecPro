# Write Up for Data Chunking Project

## Goal
- Take input files and produce output files in desired format. Refer the following pointers for more details.
	- `PI_TPC.zip` will have some files, each file with performance data.
	- Your job is to take these files and produce output files in certain format.
- For data filtration and format requirements, refer the files in the `OutputData` directory.
- The project is self explanatory, to simplify it further, some hints are in the following section. 



## General Hints

- Each input file starts with `PerfReport` prefix, this performance report comes from multiple storage arrays (prefixed with SVC). 
- Overall, the program should: 
	- Combine all Host, Disks, ManagedDisks, Nodes, etc. and put them in their respective files (refer `OutputData` directory for the individual file structure).
	- Each corresponding file should ideally have data worth of 5-minute timeframe.
	- You can generate as many files as required to meet above two conditions, there is no upper limit.
- Final outcome: 
	- One should be able to run a script via CLI and produce consolidated desired data in a custom `OutputData` directory.
	- The input data, output data directories should be user configurable. 
