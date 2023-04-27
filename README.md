# TNG Branch Predictors for SAT Solvers
Team TNG's repository for SAT Solvers

The folder champsim has the champsim applications with all the changes that we have done in the project.

# Code
The code for the LTAGE branch predictor is in LTAGE.bpred in the branch subfolder of champsim. 
The code for the TAGE predictor is in TAGE.bpred in the same folder. 

The codes used for testing by changing the values of alpha(The common ratio in the case of geometric history lengths) can be found in the alpha folder of branch folder. The code for testing the value of number of tables are in the tables folder. The code for testing if the values of tag lengths and index bits can be kept uniform across the number of tagged components is in uniform folder of the branch folder. 

The code for LTAGE with correction filter is in LTAGE_SC.bpred file in the same folder


# Traces
The code for LTAGE has been ran on 8 traces which were given in the [link](https://www.dropbox.com/sh/xs2t9y4cuqlgrlp/AAC9pt2aCq64eiLviUlmWl_aa/front-end-bound?dl=0&subfolder_nav_tracking=1). traces are named 1 to 8 as per the given order in the link itself. 

# Results
The results that we have obtained during the results( ran for all 8 given traces )are in the results_30M folder. The results for various experiments are found in the following folders:
- hashed_perceptron: has the results for the hashed_perceptron branch predictor. 
- Bimodal: has the results for the bimodal branch predictor.
- alpha: has the results for the experiment in which we varied the value of alpha to verify the optimal value. 
- intial: has the results for the original LTAGE predictor with update policy that as mentioned in the paper. 
- TAGE: has the results for the TAGE predictor without loop predictor. 
- tables: has the results obtained by changing the number of tables to 4, 8, 12, 16
- uniform: has the results obtained by assigning uniform values of tag lengths and number of index bits across all the tagged components.

# How to run our code?
- Download the LTAGE.bpred file from our branch folder.
- run it on any trace by using the build_champsim.sh and run_champsim.sh files in the champsim folder. 

# Resources 
- [LTAGE Paper](https://www.irisa.fr/caps/people/seznec/L-TAGE.pdf)
- [Andre Seznec's code for LTAGE](https://jilp.org/cbp2016/program.html) 
- [TAGE-L-SC](https://safari.ethz.ch/digitaltechnik/spring2019/lib/exe/fetch.php?media=tage-sc-l2014seznec.pdf)
- [A PPM- like Tag based predictor](https://inria.hal.science/hal-03406188/document#:~:text=Page%204-,A%20PPM%2Dlike%2C%20tag%2Dbased%20branch%20predictor,a%200%2F1%20final%20prediction.)
- [Another TAGE predictor Paper](http://www.irisa.fr/caps/people/seznec/JILP-COTTAGE.pdf)
- [LTAGE Predictor](https://github.com/KanPard005/RISCY_V_TAGE)
- [TAGE Github Repository](https://github.com/boubinjg/BranchPrediction)

