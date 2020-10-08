

In script: python/plotLimit_copyexp.py
Update L.178 : mGo = int(x[x.find('_g')+2:x.find('_chi')])
Update L.179 : mLSP = int(x[x.find('_chi')+4:x.find('_30cm.As')])

some .Draw/.Write options are commented out (to not draw the observed limit)


copy the computed liioutput files: cp ../CompLimit/limitOutput/higgsCombine_g* test/limitOutput/

Run as : python python/plotLimit_copyexp.py 'test'     :  test is the string taken by the variable 'pattern' in code.


Outputs from the higgs combine for 30cm are stored for a mock run of the code.

