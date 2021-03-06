# Varying-coefficient-model-longitudinal-data-adaptive-randomization
Generalized semiparametric varying‐coefficient model for longitudinal data with applications to adaptive treatment randomizations


-----------------------------------------------
Data
-----------------------------------------------
Data set "minimum_data.csv" includes the following variables:
PATID  ID number(recreated)
time1-time23 observation times
cdfour1-cdfour23 cd4 cell counts
age age of Patients
Si time to mutation or interim review
sex 1 Female 0 Male
race1 1 white 0 else
race2 1 black 0 else
RX regime after switching 1 ZDV  2 ZDV+DDI  3 ZDV+DDI+NVP 6 ZDV+DDI 7 ZDV+DDI+NVP
Mutation 1 215-mutation


------------------------------------------------
Code:
------------------------------------------------
1.First please compile the five *.c files to have *.mexw64 in the 64 bit operating system by using the command in Matlab:
mex *.c
2.Change gamma_func.m and theta_n= (line 56 main_1strand.m ) for different form of gamma function.
3.The code starts with main_1strand.m for first randomization and main_2ndrand.m for second randomization
4.If needed, run the bandwidth selection function band.m to select the cross-validation bandwidth.(optional)


------------------------------------------------
Please refer to the paper:
------------------------------------------------
Qi, L., Sun, Y. and Gilbert, P. B. (2016). Generalized Semiparametric Varying-Coeffifficient Model for Longitudinal Data with Applications to Adaptive Treatment Randomizations. To appear in Biometrics.
