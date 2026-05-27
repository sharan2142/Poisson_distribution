# Fitting Poisson  distribution
# Aim : 

To fit poisson distribution for the arrival of objects per minute from the feeder

# Software required :  

Python and Visual component tool

# Theory:

The Poisson distribution is the discrete probability distribution of the number of events occurring in a given time period, given the average number of times the event occurs over that time period.

If A is mean, then the probability mass function of Poisson distribution is:

<img width="267" height="66" alt="image" src="https://github.com/user-attachments/assets/b67ddb3c-d2c8-41be-810e-fc51d41b5f2e" />

![image](https://user-images.githubusercontent.com/104613195/166248326-fd042076-8b0b-40c4-8b11-1d8e8fcb74db.png)

 Conditions for Poisson Distribution:

1. An event can occur any number of times during a time period.
2. Events occur independently. I
3. The rate of occurrence is constant.
4. The probability of an event occurring is proportional to the length of the time period. 
 
# Procedure :

![image](https://user-images.githubusercontent.com/104613195/166251988-d0c53205-6080-4f7b-ae4c-398178586637.png)

# Experiment :

![image](https://user-images.githubusercontent.com/103921593/230282876-f4a5afbf-cac1-4648-a1b0-c78840638a8e.png)

# Program :
```
import numpy as np
import math
import scipy.stats

for i in
for i in range(M+1):
    c = 0
    for j in range(N):
        if L[j] == i:
            c.append(c)
    X.append(i)

sf = np.sum(f)

for i in range(M+1):
    mean = np.inner(X, p)

print("X Obs.Fr Exp.Fr xi")
print("-----------")

for x in range(M+1):
    p.append(math.exp(-mean) * mean / math.factorial(x))
    E.append(p[x] * sf)

print("%2.3f %4.2f %3.2f")

cal_chi2_sq = sum(xi)

print("Calculated value of Chi square is %4.2f" % cal_chi2_sq)

table_chi2 = scipy.stats.chi2.ppf(0.95, M)

print("Table value of chi level is %4.2f" % table_chi2)

if cal_chi2_sq < table_chi2:
    print("The given data can be fitted in poisson Distribution at 1% LOS")
else:
    print("The given data cannot be fitted in Poisson Distribution at 1% LOS")
```


# Output :
<img width="861" height="510" alt="image" src="https://github.com/user-attachments/assets/01b8037c-e1a6-4076-80fb-a4ddae26f076" />




# Results

The Poisson distribution is fitted for the objects arrived from feeder per minute and the data is tested using Chi-square test. 
 
