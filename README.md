# Survivor Selection in a Crossoverless Evolutionary Algorithm

This repository presents the code used for the Evo* conference submittion: Survivor Selection in a
Crossoverless Evolutionary Algorithm.

the file structure is as follows

- config.py : all configurations set for running the experiments
- run.py    : The "init" class for the experiments to run, this class calls to specific PPA processes and checks if the experiments are done

- classes:
    - Benchmark.py          : all benchmark functions implemented
    - DataExporter.py       : at the end of a run, results are exported to csv using this class
    - Heritage.py           : during a run all data is stored in this class
    - Individual.py         : the class that represents an individual in the search space with all its properties (objective value, fitness value, inputs, etc)
    - PPAProcess.py         : the class containing all plant propagation algorithm components, called upon by the run.py
    - SurvivorSelection.py  : All implemented survivor selection methods
- Extras : contains the heatmap in 2d of the survivor selection mehtods and 5 benchmark [2d] benchmark functions in 2 dimensions
- notebooks:
    - analysis.ipynb : the notebook used for analysing data and exporting graphs
