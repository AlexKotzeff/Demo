```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns 
```


```python
df = pd.read_csv("2019HappinessData.csv")
```


```python
dfCategories = df.drop(["Overall rank", "Score"], axis=1)
sns.boxplot(data=dfCategories)
plt.xticks(rotation=-90)
plt.ylabel("Rating")
plt.xlabel("Categories")
plt.title("Distribution of Scoring For Each Category")
```




    Text(0.5, 1.0, 'Distribution of Scoring For Each Category')






![png](Demo_files/Demo_2_1.png)




```python

```
