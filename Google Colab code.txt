import pandas as pd
import matplotlib.pylab as plt
import numpy as np
import scipy as sp

#Time data
x=np.array([0,1,2,3,4,5,6])
#Signal data
y=np.array([0, 10, 50, 40, 35, 20, 10])

plt.plot(x,y)


I = sp.integrate.simpson(y,x=x)
T = sp.integrate.simpson(y*x,x=x)
Tau = T/I
Q = sp.integrate.simpson(y*x**2,x=x)
Theta = np.lib.scimath.sqrt(Q/I - Tau**2)
A = I/(2*Theta)
print ('AUC = ', I)
print ('Signal Time = ', Tau)
print ('Signal Duration = ', Theta)
print ('Amplitude = ', A)
