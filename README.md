# seaborn.py
import pandas as pd
import seaborn as sb
from matplotlib import pyplot as plt
df=sb.load_dataset('tips')
print(df.to_string())
g=sb.FacetGrid(df,col= "time")
g.map(plt.hist,"tip")
plt.show()
