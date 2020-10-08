
two sample data cards are given: datacard_g*
with the corresponding root file: Limit_BinNumberAllBkg*

the root file contains the prediction for different sources of background, signal and observed data ( can input any mock data for expected limits)


combine to be run as:
combine -M AsymptoticLimits DATACARD --name PREFIXNAMEFOROUTPUT  --noFitAsimov
example : combine -M AsymptoticLimits datacard_g1200_chi750LT30cm.txt --name _g1200_chi750LT30cm  --noFitAsimov
gives output: higgsCombine_g1200_chi750LT30cm.AsymptoticLimits.mH120.root

for mass running: python python/RunCombine.py : python/RunCombine.py needs to be tweaked according to the datacard names etc. used

stores output in : limitOutput : this output will be used by plotting tool 



Import note: while making the histograms for signal poits with gluino mass < 1.4 TeV.  weight the cross section by: 0.01 .

because a large amount of signal yields are difficult to fit with with small background. Later in the limit plotting tool the gross section are weighted with 100 (already in code) for getting a proper limit plot.

