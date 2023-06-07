import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

data = pd.DataFrame({
    'Variable1' : [0.084193803, 1, 0.495115784, 0.67845266, 0.165485322]
    'Variable2' : [0.117625599, 0.495115784, 1, 0.56345835, 0.35157111]
})  'Variable3' : [0.135320501, 0.678452664, 0.56345835, 1, 0.201353632]

correlation_matrix = data.corr()

sns.heatmap(correlation_matrix, annot=True, cmap='coolwarm')

plt.show()
