# Logical Probabilistic Computational Assistant
This is a semi-automated heuristic logical/probabilistic computational assistant to calculate discrete probabilities of logical formulas over detectors. The core functionalities are manipulation of logical formulas, algebraic probabilities, and independence statements. Also included is the code for estimation and analysis of error rates of safety monitors for an underwater vehicle surveying the pipeline. This assistant is implemented in Mathematica using its symbolic manipulation capabilities. 

To start, install Mathematica, load the functions from the top-level notebooks, and proceed to the notebook of interest in one of the directories. Execute it step-by-step. 


Guide to the notebooks: 
* **prob-rules.nb**: the full set of inference rules for algebraic probability and independence statements. 
* **detector-ops.nb**: the definitions of detector and the 3-value linear temporal logic over detectors. 
* **file-ops.nb**: miscellaneous operations over data files, particularly to read monitor statistics and sample monitor traces. 
* **charting-ops.nb**: miscellaneous analysis and visualization functions, including automated binning and confidence intervals. 
* **pr-monitor-analysis** folder: materials for error rate estimation of the PR monitor:
  * **pr-pointestimates-by-d-analysis.nb**: analysis of estimates of the FNR of the PR monitor relative to the window size parameter.
  * **pr-pointestimates-by-datacount-analysis.nb**: analysis of estimates of the FNR of the PR monitor relative to the amount of data provided for the analysis.
  * **pr-stateful-noise-analysis.nb**: analysis of estimates of the FNR of PR monitor for the case of stateful (non-independent) error. 
  * **pr-mse-by-d-chartwall.nb**: error analysis of FNR estimates of PR monitor for each value of window size parameter. 
  * **prediction.nb**: prediction of the PR monitor values using logistic regression (not part of the error rate analysis).
* **rf-monitor-analysis** folder: materials for error rate estimation of the RF monitor:
  * **rf-pointestimates-by-d-analysis.nb**: analysis of estimates of the FPR of the RF monitor relative to the window size parameter.
  * **rf-pointestimates-by-datacount-analysis.nb**: analysis of estimates of the FPR of the RF monitor relative to the amount of data provided for the analysis.
  * **rf-stateful-noise-analysis.nb**: analysis of estimates of the FPR of RF monitor for the case of stateful (non-independent) error. 
  * **rf-mse-by-d-chartwall.nb**: error analysis of FPR estimates of RF monitor for each value of window size parameter. 
* **formula-inference** folder: materials related to inference of error rate formulas:
  * **pr-fnr-automatic.nb**: a universal set of inference rules for formulas of the FNR of the PR monitor. 
  * **pr-fpr-automatic.nb**: a universal set of inference rules for formulas of the FPR of the PR monitor. 
  * **pr-fpr-manual.nb**:  specialized sets of inference rules for formulas of the FPR of the PR monitor. 
* **tests** folder: materials to test and debug the functionality of the computational assistant on simple examples:
  * **fnr-of-conjunction-inference.nb**: lists for inference rules for the FNR of a conjunction of two independent detectors.
  * **fpr-of-conjunction-inference.nb**: lists for inference rules for the FPR of a conjunction of two independent detectors.
  * **umbrella-rain.nb**: a simple probability space with different inference scenarios and lists of rules. 


