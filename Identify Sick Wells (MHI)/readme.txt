This notebook can be used to compare wells from same field to identify poor performing wells

## Heterogeneity Index
As a way to recognize candidate for well intervention or workover jobs, using historical production data, we can create an analysis that creates a dimensionless calculated variable used to compare the behavior of individual wells in a group, using the average behavior of the group of wells as reference. Or widely known as Heterogeneity Index

HI = 0 are the wells that behaves like the average
HI > 0 are the wells that behaves above the average
HI < 0 are the wells that behaves below the average
But to know more about how the behavior changes along the production lifetime of a well, we need to calculate calculate the cumulative of the heterogeneity index. Then, we can plot the cum HI values of 2 variables (e.g. oil and water) in a scatter plot for each date to see anomalous behavior.

Each point on the above plot represents one well on a certain date. It is 2 heterogeneity analysis against each other, the running sum of the water HI vs the running sum of the oil HI. There will be 4 quadrants (where each well we can color code based on the latest date quadrant) that we can use as an analysis method for early stage of workover/well intervention opportunity identification:
Region of High Water and Low/High Oil: Wells need further investigaton on water problems. Could be candidate for WSO jobs
Region of Low Water and Low Oil: Wells need further investigation on its surrounding reservoir properties or completion. Could be candidate for acidizing/stimulation
Region of Low Water and High Oil: Wells are high oil producer, no further action needed
Beside its quadrant, the trace lines can also give us insight. Wells that were previously inside the Low Water quadrant but at some point rapidly changes to High water quadrants could be a sign of water encroachment problems (Coning/Cusping, Channeling, Casing/Tubing/Packer leaks, Flow behing Casing, Moving WOC, Watered Out Layer, etc.)
Conventional HI can give extreme values (between -1 and infinity, i.e. it can be very high should the well is far above average). From SPE-138229-MS, the paper proposed a modified version that normalize the monthly HI values
                             


We can find a python code which takes data from a .csv that contains each well's daily oil and water production rate along with the reservoir sand it produces. It then calculates the cum MHI for oil and water for each respective reservoir sand (since reservoir layer can be a determining factor that differentiate production performance.


#MODIFIED_HETEROGENEITY_INDEX_PLOT #MODIFIED_HETEROGENEITY_INDEX_PLOTS #MODIFIED_HETEROGENEITY_INDEX #PLOTS 


























#datascience #data #dataanalytics #machinelearning #dataanalysis #datascientist #artificialintelligence #python #bigdata #dataviz #ai #deeplearning #analytics #technology #programming #dataanalyst #businessintelligence #pythonprogramming #coding #business #statistics #datamining #tech #computerscience #database #powerbi #tableau #bigdataanalytics #bhfyp


#PETROLEUM_ENGINEERING #PETROLEUM_ENGINEER #SOCIETY_OF_PETROLEUM_ENGINEERS #PETROLEUM_ENGINEERS #PETROLEUM_ENGINEERING_TECHNOLOGY #OFFICIALLY_PETROLEUM_ENGINEER #PETROLEUM_ENGINEERING_ONLINE_TUTORING #PETROLEUM_ENGINEERING #PETROLEUM_ENGINEERING #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #STARS #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #STARS #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #STARS #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #STARS #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #STARS #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #STARS #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #STARS #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #STARS #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #STARS #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #STARS #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION #CMG #IMEX #STARS #KAPPA #RESERVOIR_SIMULATION #RESERVOIR_ENGINEERING #RESERVOIR_ENGINEER #RESERVOIR #RESERVOIRSIMULATOR #SIMULATION
