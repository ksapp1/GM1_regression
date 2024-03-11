# Gramacidin_regression

INTRODUCTION:

Using multiple Machine Learning algorithms (in sci-kit learn) to determine how lipid environment impacts the hydrogen bonds that form the channel of the GM1 dimer.

This repository contains an Ipython Notebook file that takes input data where the y-values are defined by a property of the channel (in an MD simulation) which is indicative of the "openness" of the chanel and the X-values are defined by properties of the membrane surrounding the channel, which is fit to multiple regression models to predict the continuous channel state and to get the feature importance of the membrane features in the determination of the channel state. 

The data is stored in two files: "data.dat" contains the membrane data and "hbond.dat" contains the channel data. The files both contain completely numeric data and is not missing any values. The data (in data.dat) is stored as: t_s1 t_s2 t_s3 c_s1 c_s2 c_s3, where t_s1: thickness of membrane in first shell and c_u_s1: composition in first shell. The data (in hbond.dat) is the length of the 6 Hydrogen bonds. The sum of these bond lengths are used as y-values.

Support Vector Regression (SVR) and Random Forest (RF) Regression models are used. Multiple parameters are optimized for both algorithms, however given the current amount of data overfitting is not eliminated. 

USAGE:

This is a Jupyter Notebook and can be run as such.
