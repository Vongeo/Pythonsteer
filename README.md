# Pythonsteer
import numpy as np

ax = np.array([4, 2, 5, 4, 5, 3, 3, 3]);
vt = np.array([1, 3, 4, 5, 5, 5, 4, 3]);
rdes = 2;
print(ax)
print(vt)

rreal = ax / vt**2
print(rreal)

steerangl = 0

for i in range(0,len(ax)) :
    if rreal[i] < rdes:
        steerangl += 1      
    elif  rreal[i] > rdes:
        steerangl -= 1
    else:
        steerangl = steerangle
        
print (steerangl)
