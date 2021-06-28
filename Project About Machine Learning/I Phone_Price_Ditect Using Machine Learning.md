# IPhone Price Ditect

## This Problem :

Check the future I phone version Price

## Tools :

Using Python (pandas,sklearn)

Main idea is Machin Learning


## The Solution :

```python
import pandas as pd
from sklearn.linear_model import LinearRegression
data = pd.read_csv('iphone_price.csv')
model=LinearRegression()
print(data.plot.bar())
model.fit(data[['version']],data[['price']])
print(model.predict([[20]]))
print(model.predict([[30]]))
```
