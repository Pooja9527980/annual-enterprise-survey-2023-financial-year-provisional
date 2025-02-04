```python
import pandas as pd
df = pd.read_csv(r'annual-enterprise-survey-2023-financial-year-provisional.csv')

```


```python
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_name_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Value</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H01</td>
      <td>Total income</td>
      <td>Financial performance</td>
      <td>930995</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H04</td>
      <td>Sales, government funding, grants and subsidies</td>
      <td>Financial performance</td>
      <td>821630</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H05</td>
      <td>Interest, dividends and donations</td>
      <td>Financial performance</td>
      <td>84354</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H07</td>
      <td>Non-operating income</td>
      <td>Financial performance</td>
      <td>25010</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H08</td>
      <td>Total expenditure</td>
      <td>Financial performance</td>
      <td>832964</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>50980</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H37</td>
      <td>Quick ratio</td>
      <td>Financial ratios</td>
      <td>52</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50981</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H38</td>
      <td>Margin on sales of goods for resale</td>
      <td>Financial ratios</td>
      <td>40</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50982</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H39</td>
      <td>Return on equity</td>
      <td>Financial ratios</td>
      <td>12</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50983</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H40</td>
      <td>Return on total assets</td>
      <td>Financial ratios</td>
      <td>5</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50984</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H41</td>
      <td>Liabilities structure</td>
      <td>Financial ratios</td>
      <td>46</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
  </tbody>
</table>
<p>50985 rows × 10 columns</p>
</div>




```python
df.head()  # Displays first 5 rows

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_name_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Value</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H01</td>
      <td>Total income</td>
      <td>Financial performance</td>
      <td>930995</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H04</td>
      <td>Sales, government funding, grants and subsidies</td>
      <td>Financial performance</td>
      <td>821630</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H05</td>
      <td>Interest, dividends and donations</td>
      <td>Financial performance</td>
      <td>84354</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H07</td>
      <td>Non-operating income</td>
      <td>Financial performance</td>
      <td>25010</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H08</td>
      <td>Total expenditure</td>
      <td>Financial performance</td>
      <td>832964</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.head(10)  # Displays first 10 rows

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_name_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Value</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H01</td>
      <td>Total income</td>
      <td>Financial performance</td>
      <td>930995</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H04</td>
      <td>Sales, government funding, grants and subsidies</td>
      <td>Financial performance</td>
      <td>821630</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H05</td>
      <td>Interest, dividends and donations</td>
      <td>Financial performance</td>
      <td>84354</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H07</td>
      <td>Non-operating income</td>
      <td>Financial performance</td>
      <td>25010</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H08</td>
      <td>Total expenditure</td>
      <td>Financial performance</td>
      <td>832964</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>5</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H09</td>
      <td>Interest and donations</td>
      <td>Financial performance</td>
      <td>55267</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>6</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H10</td>
      <td>Indirect taxes</td>
      <td>Financial performance</td>
      <td>7426</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>7</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H11</td>
      <td>Depreciation</td>
      <td>Financial performance</td>
      <td>30814</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>8</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H12</td>
      <td>Salaries and wages paid</td>
      <td>Financial performance</td>
      <td>147663</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>9</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H13</td>
      <td>Redundancy and severance</td>
      <td>Financial performance</td>
      <td>269</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.tail()  # Displays last 5 rows


```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_name_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Value</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>50980</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H37</td>
      <td>Quick ratio</td>
      <td>Financial ratios</td>
      <td>52</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50981</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H38</td>
      <td>Margin on sales of goods for resale</td>
      <td>Financial ratios</td>
      <td>40</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50982</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H39</td>
      <td>Return on equity</td>
      <td>Financial ratios</td>
      <td>12</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50983</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H40</td>
      <td>Return on total assets</td>
      <td>Financial ratios</td>
      <td>5</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50984</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H41</td>
      <td>Liabilities structure</td>
      <td>Financial ratios</td>
      <td>46</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.tail(3)  # Displays last 3 rows
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_name_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Value</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>50982</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H39</td>
      <td>Return on equity</td>
      <td>Financial ratios</td>
      <td>12</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50983</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H40</td>
      <td>Return on total assets</td>
      <td>Financial ratios</td>
      <td>5</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50984</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H41</td>
      <td>Liabilities structure</td>
      <td>Financial ratios</td>
      <td>46</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.info()

```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 50985 entries, 0 to 50984
    Data columns (total 10 columns):
     #   Column                       Non-Null Count  Dtype 
    ---  ------                       --------------  ----- 
     0   Year                         50985 non-null  int64 
     1   Industry_aggregation_NZSIOC  50985 non-null  object
     2   Industry_code_NZSIOC         50985 non-null  object
     3   Industry_name_NZSIOC         50985 non-null  object
     4   Units                        50985 non-null  object
     5   Variable_code                50985 non-null  object
     6   Variable_name                50985 non-null  object
     7   Variable_category            50985 non-null  object
     8   Value                        50985 non-null  object
     9   Industry_code_ANZSIC06       50985 non-null  object
    dtypes: int64(1), object(9)
    memory usage: 3.9+ MB
    


```python
df.describe()

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>50985.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>2018.000000</td>
    </tr>
    <tr>
      <th>std</th>
      <td>3.162309</td>
    </tr>
    <tr>
      <th>min</th>
      <td>2013.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>2015.000000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>2018.000000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>2021.000000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>2023.000000</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.sort_values('Value', ascending=False)  # Sort by salary in descending order
df.sort_values(['Industry_name_NZSIOC', 'Units'], ascending=[True, False])  # Sort by department and age


```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_name_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Value</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2681</th>
      <td>2023</td>
      <td>Level 4</td>
      <td>GH211</td>
      <td>Accommodation</td>
      <td>Percentage</td>
      <td>H36</td>
      <td>Current ratio</td>
      <td>Financial ratios</td>
      <td>69</td>
      <td>ANZSIC06 group H440</td>
    </tr>
    <tr>
      <th>2682</th>
      <td>2023</td>
      <td>Level 4</td>
      <td>GH211</td>
      <td>Accommodation</td>
      <td>Percentage</td>
      <td>H37</td>
      <td>Quick ratio</td>
      <td>Financial ratios</td>
      <td>66</td>
      <td>ANZSIC06 group H440</td>
    </tr>
    <tr>
      <th>2683</th>
      <td>2023</td>
      <td>Level 4</td>
      <td>GH211</td>
      <td>Accommodation</td>
      <td>Percentage</td>
      <td>H38</td>
      <td>Margin on sales of goods for resale</td>
      <td>Financial ratios</td>
      <td>60</td>
      <td>ANZSIC06 group H440</td>
    </tr>
    <tr>
      <th>2684</th>
      <td>2023</td>
      <td>Level 4</td>
      <td>GH211</td>
      <td>Accommodation</td>
      <td>Percentage</td>
      <td>H39</td>
      <td>Return on equity</td>
      <td>Financial ratios</td>
      <td>13</td>
      <td>ANZSIC06 group H440</td>
    </tr>
    <tr>
      <th>2685</th>
      <td>2023</td>
      <td>Level 4</td>
      <td>GH211</td>
      <td>Accommodation</td>
      <td>Percentage</td>
      <td>H40</td>
      <td>Return on total assets</td>
      <td>Financial ratios</td>
      <td>5</td>
      <td>ANZSIC06 group H440</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>42454</th>
      <td>2014</td>
      <td>Level 4</td>
      <td>CC311</td>
      <td>Wood Product Manufacturing</td>
      <td>Dollars</td>
      <td>H35</td>
      <td>Surplus per employee count</td>
      <td>Financial ratios</td>
      <td>5,600</td>
      <td>ANZSIC06 groups C141 and C149</td>
    </tr>
    <tr>
      <th>47052</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>CC31</td>
      <td>Wood Product Manufacturing</td>
      <td>Dollars</td>
      <td>H34</td>
      <td>Total income per employee count</td>
      <td>Financial ratios</td>
      <td>281,700</td>
      <td>ANZSIC06 groups C141 and C149</td>
    </tr>
    <tr>
      <th>47053</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>CC31</td>
      <td>Wood Product Manufacturing</td>
      <td>Dollars</td>
      <td>H35</td>
      <td>Surplus per employee count</td>
      <td>Financial ratios</td>
      <td>6,300</td>
      <td>ANZSIC06 groups C141 and C149</td>
    </tr>
    <tr>
      <th>47088</th>
      <td>2013</td>
      <td>Level 4</td>
      <td>CC311</td>
      <td>Wood Product Manufacturing</td>
      <td>Dollars</td>
      <td>H34</td>
      <td>Total income per employee count</td>
      <td>Financial ratios</td>
      <td>281,700</td>
      <td>ANZSIC06 groups C141 and C149</td>
    </tr>
    <tr>
      <th>47089</th>
      <td>2013</td>
      <td>Level 4</td>
      <td>CC311</td>
      <td>Wood Product Manufacturing</td>
      <td>Dollars</td>
      <td>H35</td>
      <td>Surplus per employee count</td>
      <td>Financial ratios</td>
      <td>6,300</td>
      <td>ANZSIC06 groups C141 and C149</td>
    </tr>
  </tbody>
</table>
<p>50985 rows × 10 columns</p>
</div>




```python
df.loc[0]  # Select the first row
df.loc[0, 'Industry_name_NZSIOC']  # Select the name of the first row
df.loc[df['Year'] > 2013]  # Select rows where age is greater than 30

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_name_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Value</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H01</td>
      <td>Total income</td>
      <td>Financial performance</td>
      <td>930995</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H04</td>
      <td>Sales, government funding, grants and subsidies</td>
      <td>Financial performance</td>
      <td>821630</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H05</td>
      <td>Interest, dividends and donations</td>
      <td>Financial performance</td>
      <td>84354</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H07</td>
      <td>Non-operating income</td>
      <td>Financial performance</td>
      <td>25010</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H08</td>
      <td>Total expenditure</td>
      <td>Financial performance</td>
      <td>832964</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>46345</th>
      <td>2014</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food Product Manufacturing</td>
      <td>Percentage</td>
      <td>H37</td>
      <td>Quick ratio</td>
      <td>Financial ratios</td>
      <td>50</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>46346</th>
      <td>2014</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food Product Manufacturing</td>
      <td>Percentage</td>
      <td>H38</td>
      <td>Margin on sales of goods for resale</td>
      <td>Financial ratios</td>
      <td>40</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>46347</th>
      <td>2014</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food Product Manufacturing</td>
      <td>Percentage</td>
      <td>H39</td>
      <td>Return on equity</td>
      <td>Financial ratios</td>
      <td>4</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>46348</th>
      <td>2014</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food Product Manufacturing</td>
      <td>Percentage</td>
      <td>H40</td>
      <td>Return on total assets</td>
      <td>Financial ratios</td>
      <td>2</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>46349</th>
      <td>2014</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food Product Manufacturing</td>
      <td>Percentage</td>
      <td>H41</td>
      <td>Liabilities structure</td>
      <td>Financial ratios</td>
      <td>44</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
  </tbody>
</table>
<p>46350 rows × 10 columns</p>
</div>




```python
df.iloc[0]  # Select the first row
df.iloc[0, 1]  # Select the value in the first row, second column
df.iloc[:, 1]  # Select all rows in the second column

```




    0        Level 1
    1        Level 1
    2        Level 1
    3        Level 1
    4        Level 1
              ...   
    50980    Level 3
    50981    Level 3
    50982    Level 3
    50983    Level 3
    50984    Level 3
    Name: Industry_aggregation_NZSIOC, Length: 50985, dtype: object



## 10. DataFrame.drop() - Drop rows or columns


```python
df.drop('Value', axis=1)  # Drop the 'Value' column


```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_name_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Value</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H04</td>
      <td>Sales, government funding, grants and subsidies</td>
      <td>Financial performance</td>
      <td>821630</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H05</td>
      <td>Interest, dividends and donations</td>
      <td>Financial performance</td>
      <td>84354</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H07</td>
      <td>Non-operating income</td>
      <td>Financial performance</td>
      <td>25010</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H08</td>
      <td>Total expenditure</td>
      <td>Financial performance</td>
      <td>832964</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>5</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H09</td>
      <td>Interest and donations</td>
      <td>Financial performance</td>
      <td>55267</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>50980</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H37</td>
      <td>Quick ratio</td>
      <td>Financial ratios</td>
      <td>52</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50981</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H38</td>
      <td>Margin on sales of goods for resale</td>
      <td>Financial ratios</td>
      <td>40</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50982</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H39</td>
      <td>Return on equity</td>
      <td>Financial ratios</td>
      <td>12</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50983</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H40</td>
      <td>Return on total assets</td>
      <td>Financial ratios</td>
      <td>5</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50984</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H41</td>
      <td>Liabilities structure</td>
      <td>Financial ratios</td>
      <td>46</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
  </tbody>
</table>
<p>50984 rows × 10 columns</p>
</div>




```python
df.drop(0, axis=0)  # Drop the first row (index 0)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_name_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Value</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H04</td>
      <td>Sales, government funding, grants and subsidies</td>
      <td>Financial performance</td>
      <td>821630821630821630821630821630821630</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H05</td>
      <td>Interest, dividends and donations</td>
      <td>Financial performance</td>
      <td>843548435484354843548435484354</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H07</td>
      <td>Non-operating income</td>
      <td>Financial performance</td>
      <td>250102501025010250102501025010</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H08</td>
      <td>Total expenditure</td>
      <td>Financial performance</td>
      <td>832964832964832964832964832964832964</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>5</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H09</td>
      <td>Interest and donations</td>
      <td>Financial performance</td>
      <td>552675526755267552675526755267</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>50980</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H37</td>
      <td>Quick ratio</td>
      <td>Financial ratios</td>
      <td>525252525252</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50981</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H38</td>
      <td>Margin on sales of goods for resale</td>
      <td>Financial ratios</td>
      <td>404040404040</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50982</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H39</td>
      <td>Return on equity</td>
      <td>Financial ratios</td>
      <td>121212121212</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50983</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H40</td>
      <td>Return on total assets</td>
      <td>Financial ratios</td>
      <td>555555</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50984</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H41</td>
      <td>Liabilities structure</td>
      <td>Financial ratios</td>
      <td>464646464646</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
  </tbody>
</table>
<p>50984 rows × 10 columns</p>
</div>



## 11. DataFrame.isnull() - Check for missing values


```python
df.isnull()  # Returns True for missing values
df.isnull().sum()  # Count missing values in each column

```




    Year                           0
    Industry_aggregation_NZSIOC    0
    Industry_code_NZSIOC           0
    Industry_name_NZSIOC           0
    Units                          0
    Variable_code                  0
    Variable_name                  0
    Variable_category              0
    Value                          0
    Industry_code_ANZSIC06         0
    dtype: int64



## 12. DataFrame.fillna() - Fill missing values


```python
df.fillna(0)  # Fill missing values with 0

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_name_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Value</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H01</td>
      <td>Total income</td>
      <td>Financial performance</td>
      <td>930995</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H04</td>
      <td>Sales, government funding, grants and subsidies</td>
      <td>Financial performance</td>
      <td>821630</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H05</td>
      <td>Interest, dividends and donations</td>
      <td>Financial performance</td>
      <td>84354</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H07</td>
      <td>Non-operating income</td>
      <td>Financial performance</td>
      <td>25010</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H08</td>
      <td>Total expenditure</td>
      <td>Financial performance</td>
      <td>832964</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>50980</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H37</td>
      <td>Quick ratio</td>
      <td>Financial ratios</td>
      <td>52</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50981</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H38</td>
      <td>Margin on sales of goods for resale</td>
      <td>Financial ratios</td>
      <td>40</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50982</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H39</td>
      <td>Return on equity</td>
      <td>Financial ratios</td>
      <td>12</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50983</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H40</td>
      <td>Return on total assets</td>
      <td>Financial ratios</td>
      <td>5</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50984</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H41</td>
      <td>Liabilities structure</td>
      <td>Financial ratios</td>
      <td>46</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
  </tbody>
</table>
<p>50985 rows × 10 columns</p>
</div>



## 13. DataFrame.apply() - Apply a function along an axis


```python
df['Value'] = df['Value'].apply(lambda x: x * 3)  
```


```python
df.apply(len)  # Apply len() function to each column (get column lengths)
```




    Year                           50985
    Industry_aggregation_NZSIOC    50985
    Industry_code_NZSIOC           50985
    Industry_name_NZSIOC           50985
    Units                          50985
    Variable_code                  50985
    Variable_name                  50985
    Variable_category              50985
    Value                          50985
    Industry_code_ANZSIC06         50985
    dtype: int64



## 14. DataFrame.merge() - Merge two DataFrames


```python
df1 = pd.DataFrame({'ID': [1, 2, 3], 'Industry_name_NZSIOC': ['Food product manufacturing', 'Fresh Product', 'Vegetables Industry']})
df2 = pd.DataFrame({'ID': [1, 2, 4], 'Value': [28, 34, 45]})
merged_df = pd.merge(df1, df2, on='ID')

```


```python
df1
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ID</th>
      <th>Industry_name_NZSIOC</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>Food product manufacturing</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>Fresh Product</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>Vegetables Industry</td>
    </tr>
  </tbody>
</table>
</div>




```python
df2
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>ID</th>
      <th>Value</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>28</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>34</td>
    </tr>
    <tr>
      <th>2</th>
      <td>4</td>
      <td>45</td>
    </tr>
  </tbody>
</table>
</div>



## 15. DataFrame.set_index() - Set a column as the index


```python
df.set_index('Industry_name_NZSIOC')  # Set the 'Industry_name_NZSIOC' column as the index

```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Value</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
    <tr>
      <th>Industry_name_NZSIOC</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>All industries</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>Dollars (millions)</td>
      <td>H01</td>
      <td>Total income</td>
      <td>Financial performance</td>
      <td>9309959309959309959309959309959309959309959309...</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>All industries</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>Dollars (millions)</td>
      <td>H04</td>
      <td>Sales, government funding, grants and subsidies</td>
      <td>Financial performance</td>
      <td>8216308216308216308216308216308216308216308216...</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>All industries</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>Dollars (millions)</td>
      <td>H05</td>
      <td>Interest, dividends and donations</td>
      <td>Financial performance</td>
      <td>8435484354843548435484354843548435484354843548...</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>All industries</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>Dollars (millions)</td>
      <td>H07</td>
      <td>Non-operating income</td>
      <td>Financial performance</td>
      <td>2501025010250102501025010250102501025010250102...</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>All industries</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>Dollars (millions)</td>
      <td>H08</td>
      <td>Total expenditure</td>
      <td>Financial performance</td>
      <td>8329648329648329648329648329648329648329648329...</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>Food product manufacturing</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Percentage</td>
      <td>H37</td>
      <td>Quick ratio</td>
      <td>Financial ratios</td>
      <td>5252525252525252525252525252525252525252525252...</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>Food product manufacturing</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Percentage</td>
      <td>H38</td>
      <td>Margin on sales of goods for resale</td>
      <td>Financial ratios</td>
      <td>4040404040404040404040404040404040404040404040...</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>Food product manufacturing</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Percentage</td>
      <td>H39</td>
      <td>Return on equity</td>
      <td>Financial ratios</td>
      <td>1212121212121212121212121212121212121212121212...</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>Food product manufacturing</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Percentage</td>
      <td>H40</td>
      <td>Return on total assets</td>
      <td>Financial ratios</td>
      <td>5555555555555555555555555555555555555555555555...</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>Food product manufacturing</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Percentage</td>
      <td>H41</td>
      <td>Liabilities structure</td>
      <td>Financial ratios</td>
      <td>4646464646464646464646464646464646464646464646...</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
  </tbody>
</table>
<p>50985 rows × 9 columns</p>
</div>



## 16. DataFrame.rename() - Rename columns or index labels


```python
df.rename(columns={'Value': 'Industry_code_NZSIOC'}, inplace=True)  # Rename 'Value' column

```


```python
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Year</th>
      <th>Industry_aggregation_NZSIOC</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_name_NZSIOC</th>
      <th>Units</th>
      <th>Variable_code</th>
      <th>Variable_name</th>
      <th>Variable_category</th>
      <th>Industry_code_NZSIOC</th>
      <th>Industry_code_ANZSIC06</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H01</td>
      <td>Total income</td>
      <td>Financial performance</td>
      <td>9309959309959309959309959309959309959309959309...</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H04</td>
      <td>Sales, government funding, grants and subsidies</td>
      <td>Financial performance</td>
      <td>8216308216308216308216308216308216308216308216...</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H05</td>
      <td>Interest, dividends and donations</td>
      <td>Financial performance</td>
      <td>8435484354843548435484354843548435484354843548...</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H07</td>
      <td>Non-operating income</td>
      <td>Financial performance</td>
      <td>2501025010250102501025010250102501025010250102...</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2023</td>
      <td>Level 1</td>
      <td>99999</td>
      <td>All industries</td>
      <td>Dollars (millions)</td>
      <td>H08</td>
      <td>Total expenditure</td>
      <td>Financial performance</td>
      <td>8329648329648329648329648329648329648329648329...</td>
      <td>ANZSIC06 divisions A-S (excluding classes K633...</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>50980</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H37</td>
      <td>Quick ratio</td>
      <td>Financial ratios</td>
      <td>5252525252525252525252525252525252525252525252...</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50981</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H38</td>
      <td>Margin on sales of goods for resale</td>
      <td>Financial ratios</td>
      <td>4040404040404040404040404040404040404040404040...</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50982</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H39</td>
      <td>Return on equity</td>
      <td>Financial ratios</td>
      <td>1212121212121212121212121212121212121212121212...</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50983</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H40</td>
      <td>Return on total assets</td>
      <td>Financial ratios</td>
      <td>5555555555555555555555555555555555555555555555...</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
    <tr>
      <th>50984</th>
      <td>2013</td>
      <td>Level 3</td>
      <td>ZZ11</td>
      <td>Food product manufacturing</td>
      <td>Percentage</td>
      <td>H41</td>
      <td>Liabilities structure</td>
      <td>Financial ratios</td>
      <td>4646464646464646464646464646464646464646464646...</td>
      <td>ANZSIC06 groups C111, C112, C113, C114, C115, ...</td>
    </tr>
  </tbody>
</table>
<p>50985 rows × 10 columns</p>
</div>



## 17. DataFrame.concat() - Concatenate DataFrames


```python
df1 = pd.DataFrame({'A': [1, 2]})
df2 = pd.DataFrame({'B': [3, 4]})
concatenated_df = pd.concat([df1, df2], axis=1)  # Concatenate along columns

```


```python
df1
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>A</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python
df2
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>B</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>3</td>
    </tr>
    <tr>
      <th>1</th>
      <td>4</td>
    </tr>
  </tbody>
</table>
</div>




```python

```
