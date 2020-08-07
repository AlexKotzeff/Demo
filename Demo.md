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


<img width="727" alt="Demo2" src="https://user-images.githubusercontent.com/67394270/89647136-0b4ef880-d88b-11ea-8e35-620d84cb9b49.png">




```python

```
