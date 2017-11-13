# RandomData
Random Data


import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
# use Pandas to extract data  as a NumPy array
df = pd.read_csv('data.csv', index_col=0)
df.head()


df.hist(bins=10)
plt.xlim([-10,10])
plt.ylim([0,4000])
plt.title("Data")
plt.xlabel("x-value range")
plt.ylabel("Frequency")
plt.show()

#The sd values that correspond to the data given seem evenly distributed between two bins (0.5)&(2.0), the best value
#that would describe this equal spread would be somewhere in the middle at 1.25

#For the data alone, it seams that that the overhelming majority of points lay between (-0.25-0.25) where values outside
#of this range become increasingly more rare as it approaches the endpoints of the distribution


