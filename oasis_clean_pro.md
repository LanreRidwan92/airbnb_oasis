```python
import pandas as pd
```

                                             IMPORTING THE DATASET FROM THE FILES


```python
bn = pd.read_csv(r"C:\Users\Windows 10 Pro\Downloads\A-Oasis_Project_Tasks\AB_NYC_2019.csv")
```


```python
bn
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
      <th>id</th>
      <th>name</th>
      <th>host_id</th>
      <th>host_name</th>
      <th>neighbourhood_group</th>
      <th>neighbourhood</th>
      <th>latitude</th>
      <th>longitude</th>
      <th>room_type</th>
      <th>price</th>
      <th>minimum_nights</th>
      <th>number_of_reviews</th>
      <th>last_review</th>
      <th>reviews_per_month</th>
      <th>calculated_host_listings_count</th>
      <th>availability_365</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2539</td>
      <td>Clean &amp; quiet apt home by the park</td>
      <td>2787</td>
      <td>John</td>
      <td>Brooklyn</td>
      <td>Kensington</td>
      <td>40.64749</td>
      <td>-73.97237</td>
      <td>Private room</td>
      <td>149</td>
      <td>1</td>
      <td>9</td>
      <td>2018-10-19</td>
      <td>0.21</td>
      <td>6</td>
      <td>365</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2595</td>
      <td>Skylit Midtown Castle</td>
      <td>2845</td>
      <td>Jennifer</td>
      <td>Manhattan</td>
      <td>Midtown</td>
      <td>40.75362</td>
      <td>-73.98377</td>
      <td>Entire home/apt</td>
      <td>225</td>
      <td>1</td>
      <td>45</td>
      <td>2019-05-21</td>
      <td>0.38</td>
      <td>2</td>
      <td>355</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3647</td>
      <td>THE VILLAGE OF HARLEM....NEW YORK !</td>
      <td>4632</td>
      <td>Elisabeth</td>
      <td>Manhattan</td>
      <td>Harlem</td>
      <td>40.80902</td>
      <td>-73.94190</td>
      <td>Private room</td>
      <td>150</td>
      <td>3</td>
      <td>0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1</td>
      <td>365</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3831</td>
      <td>Cozy Entire Floor of Brownstone</td>
      <td>4869</td>
      <td>LisaRoxanne</td>
      <td>Brooklyn</td>
      <td>Clinton Hill</td>
      <td>40.68514</td>
      <td>-73.95976</td>
      <td>Entire home/apt</td>
      <td>89</td>
      <td>1</td>
      <td>270</td>
      <td>2019-07-05</td>
      <td>4.64</td>
      <td>1</td>
      <td>194</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5022</td>
      <td>Entire Apt: Spacious Studio/Loft by central park</td>
      <td>7192</td>
      <td>Laura</td>
      <td>Manhattan</td>
      <td>East Harlem</td>
      <td>40.79851</td>
      <td>-73.94399</td>
      <td>Entire home/apt</td>
      <td>80</td>
      <td>10</td>
      <td>9</td>
      <td>2018-11-19</td>
      <td>0.10</td>
      <td>1</td>
      <td>0</td>
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
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>48890</th>
      <td>36484665</td>
      <td>Charming one bedroom - newly renovated rowhouse</td>
      <td>8232441</td>
      <td>Sabrina</td>
      <td>Brooklyn</td>
      <td>Bedford-Stuyvesant</td>
      <td>40.67853</td>
      <td>-73.94995</td>
      <td>Private room</td>
      <td>70</td>
      <td>2</td>
      <td>0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2</td>
      <td>9</td>
    </tr>
    <tr>
      <th>48891</th>
      <td>36485057</td>
      <td>Affordable room in Bushwick/East Williamsburg</td>
      <td>6570630</td>
      <td>Marisol</td>
      <td>Brooklyn</td>
      <td>Bushwick</td>
      <td>40.70184</td>
      <td>-73.93317</td>
      <td>Private room</td>
      <td>40</td>
      <td>4</td>
      <td>0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2</td>
      <td>36</td>
    </tr>
    <tr>
      <th>48892</th>
      <td>36485431</td>
      <td>Sunny Studio at Historical Neighborhood</td>
      <td>23492952</td>
      <td>Ilgar &amp; Aysel</td>
      <td>Manhattan</td>
      <td>Harlem</td>
      <td>40.81475</td>
      <td>-73.94867</td>
      <td>Entire home/apt</td>
      <td>115</td>
      <td>10</td>
      <td>0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1</td>
      <td>27</td>
    </tr>
    <tr>
      <th>48893</th>
      <td>36485609</td>
      <td>43rd St. Time Square-cozy single bed</td>
      <td>30985759</td>
      <td>Taz</td>
      <td>Manhattan</td>
      <td>Hell's Kitchen</td>
      <td>40.75751</td>
      <td>-73.99112</td>
      <td>Shared room</td>
      <td>55</td>
      <td>1</td>
      <td>0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>6</td>
      <td>2</td>
    </tr>
    <tr>
      <th>48894</th>
      <td>36487245</td>
      <td>Trendy duplex in the very heart of Hell's Kitchen</td>
      <td>68119814</td>
      <td>Christophe</td>
      <td>Manhattan</td>
      <td>Hell's Kitchen</td>
      <td>40.76404</td>
      <td>-73.98933</td>
      <td>Private room</td>
      <td>90</td>
      <td>7</td>
      <td>0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1</td>
      <td>23</td>
    </tr>
  </tbody>
</table>
<p>48895 rows × 16 columns</p>
</div>



                                             CHECKING THE DUPLCATES VALUES


```python
bn.duplicated()
```




    0        False
    1        False
    2        False
    3        False
    4        False
             ...  
    48890    False
    48891    False
    48892    False
    48893    False
    48894    False
    Length: 48895, dtype: bool




```python
bn.describe
```




    <bound method NDFrame.describe of              id                                               name   host_id  \
    0          2539                 Clean & quiet apt home by the park      2787   
    1          2595                              Skylit Midtown Castle      2845   
    2          3647                THE VILLAGE OF HARLEM....NEW YORK !      4632   
    3          3831                    Cozy Entire Floor of Brownstone      4869   
    4          5022   Entire Apt: Spacious Studio/Loft by central park      7192   
    ...         ...                                                ...       ...   
    48890  36484665    Charming one bedroom - newly renovated rowhouse   8232441   
    48891  36485057      Affordable room in Bushwick/East Williamsburg   6570630   
    48892  36485431            Sunny Studio at Historical Neighborhood  23492952   
    48893  36485609               43rd St. Time Square-cozy single bed  30985759   
    48894  36487245  Trendy duplex in the very heart of Hell's Kitchen  68119814   
    
               host_name neighbourhood_group       neighbourhood  latitude  \
    0               John            Brooklyn          Kensington  40.64749   
    1           Jennifer           Manhattan             Midtown  40.75362   
    2          Elisabeth           Manhattan              Harlem  40.80902   
    3        LisaRoxanne            Brooklyn        Clinton Hill  40.68514   
    4              Laura           Manhattan         East Harlem  40.79851   
    ...              ...                 ...                 ...       ...   
    48890        Sabrina            Brooklyn  Bedford-Stuyvesant  40.67853   
    48891        Marisol            Brooklyn            Bushwick  40.70184   
    48892  Ilgar & Aysel           Manhattan              Harlem  40.81475   
    48893            Taz           Manhattan      Hell's Kitchen  40.75751   
    48894     Christophe           Manhattan      Hell's Kitchen  40.76404   
    
           longitude        room_type  price  minimum_nights  number_of_reviews  \
    0      -73.97237     Private room    149               1                  9   
    1      -73.98377  Entire home/apt    225               1                 45   
    2      -73.94190     Private room    150               3                  0   
    3      -73.95976  Entire home/apt     89               1                270   
    4      -73.94399  Entire home/apt     80              10                  9   
    ...          ...              ...    ...             ...                ...   
    48890  -73.94995     Private room     70               2                  0   
    48891  -73.93317     Private room     40               4                  0   
    48892  -73.94867  Entire home/apt    115              10                  0   
    48893  -73.99112      Shared room     55               1                  0   
    48894  -73.98933     Private room     90               7                  0   
    
          last_review  reviews_per_month  calculated_host_listings_count  \
    0      2018-10-19               0.21                               6   
    1      2019-05-21               0.38                               2   
    2             NaN                NaN                               1   
    3      2019-07-05               4.64                               1   
    4      2018-11-19               0.10                               1   
    ...           ...                ...                             ...   
    48890         NaN                NaN                               2   
    48891         NaN                NaN                               2   
    48892         NaN                NaN                               1   
    48893         NaN                NaN                               6   
    48894         NaN                NaN                               1   
    
           availability_365  
    0                   365  
    1                   355  
    2                   365  
    3                   194  
    4                     0  
    ...                 ...  
    48890                 9  
    48891                36  
    48892                27  
    48893                 2  
    48894                23  
    
    [48895 rows x 16 columns]>



                                                 CHECKING THE NULL VALUES


```python
bn.isnull().sum()
```




    id                                    0
    name                                 16
    host_id                               0
    host_name                            21
    neighbourhood_group                   0
    neighbourhood                         0
    latitude                              0
    longitude                             0
    room_type                             0
    price                                 0
    minimum_nights                        0
    number_of_reviews                     0
    last_review                       10052
    reviews_per_month                 10052
    calculated_host_listings_count        0
    availability_365                      0
    dtype: int64




```python
bn.drop_duplicates
```




    <bound method DataFrame.drop_duplicates of              id                                               name   host_id  \
    0          2539                 Clean & quiet apt home by the park      2787   
    1          2595                              Skylit Midtown Castle      2845   
    2          3647                THE VILLAGE OF HARLEM....NEW YORK !      4632   
    3          3831                    Cozy Entire Floor of Brownstone      4869   
    4          5022   Entire Apt: Spacious Studio/Loft by central park      7192   
    ...         ...                                                ...       ...   
    48890  36484665    Charming one bedroom - newly renovated rowhouse   8232441   
    48891  36485057      Affordable room in Bushwick/East Williamsburg   6570630   
    48892  36485431            Sunny Studio at Historical Neighborhood  23492952   
    48893  36485609               43rd St. Time Square-cozy single bed  30985759   
    48894  36487245  Trendy duplex in the very heart of Hell's Kitchen  68119814   
    
               host_name neighbourhood_group       neighbourhood  latitude  \
    0               John            Brooklyn          Kensington  40.64749   
    1           Jennifer           Manhattan             Midtown  40.75362   
    2          Elisabeth           Manhattan              Harlem  40.80902   
    3        LisaRoxanne            Brooklyn        Clinton Hill  40.68514   
    4              Laura           Manhattan         East Harlem  40.79851   
    ...              ...                 ...                 ...       ...   
    48890        Sabrina            Brooklyn  Bedford-Stuyvesant  40.67853   
    48891        Marisol            Brooklyn            Bushwick  40.70184   
    48892  Ilgar & Aysel           Manhattan              Harlem  40.81475   
    48893            Taz           Manhattan      Hell's Kitchen  40.75751   
    48894     Christophe           Manhattan      Hell's Kitchen  40.76404   
    
           longitude        room_type  price  minimum_nights  number_of_reviews  \
    0      -73.97237     Private room    149               1                  9   
    1      -73.98377  Entire home/apt    225               1                 45   
    2      -73.94190     Private room    150               3                  0   
    3      -73.95976  Entire home/apt     89               1                270   
    4      -73.94399  Entire home/apt     80              10                  9   
    ...          ...              ...    ...             ...                ...   
    48890  -73.94995     Private room     70               2                  0   
    48891  -73.93317     Private room     40               4                  0   
    48892  -73.94867  Entire home/apt    115              10                  0   
    48893  -73.99112      Shared room     55               1                  0   
    48894  -73.98933     Private room     90               7                  0   
    
          last_review  reviews_per_month  calculated_host_listings_count  \
    0      2018-10-19               0.21                               6   
    1      2019-05-21               0.38                               2   
    2             NaN                NaN                               1   
    3      2019-07-05               4.64                               1   
    4      2018-11-19               0.10                               1   
    ...           ...                ...                             ...   
    48890         NaN                NaN                               2   
    48891         NaN                NaN                               2   
    48892         NaN                NaN                               1   
    48893         NaN                NaN                               6   
    48894         NaN                NaN                               1   
    
           availability_365  
    0                   365  
    1                   355  
    2                   365  
    3                   194  
    4                     0  
    ...                 ...  
    48890                 9  
    48891                36  
    48892                27  
    48893                 2  
    48894                23  
    
    [48895 rows x 16 columns]>




```python
bn.head(3)
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
      <th>id</th>
      <th>name</th>
      <th>host_id</th>
      <th>host_name</th>
      <th>neighbourhood_group</th>
      <th>neighbourhood</th>
      <th>latitude</th>
      <th>longitude</th>
      <th>room_type</th>
      <th>price</th>
      <th>minimum_nights</th>
      <th>number_of_reviews</th>
      <th>last_review</th>
      <th>reviews_per_month</th>
      <th>calculated_host_listings_count</th>
      <th>availability_365</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2539</td>
      <td>Clean &amp; quiet apt home by the park</td>
      <td>2787</td>
      <td>John</td>
      <td>Brooklyn</td>
      <td>Kensington</td>
      <td>40.64749</td>
      <td>-73.97237</td>
      <td>Private room</td>
      <td>149</td>
      <td>1</td>
      <td>9</td>
      <td>2018-10-19</td>
      <td>0.21</td>
      <td>6</td>
      <td>365</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2595</td>
      <td>Skylit Midtown Castle</td>
      <td>2845</td>
      <td>Jennifer</td>
      <td>Manhattan</td>
      <td>Midtown</td>
      <td>40.75362</td>
      <td>-73.98377</td>
      <td>Entire home/apt</td>
      <td>225</td>
      <td>1</td>
      <td>45</td>
      <td>2019-05-21</td>
      <td>0.38</td>
      <td>2</td>
      <td>355</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3647</td>
      <td>THE VILLAGE OF HARLEM....NEW YORK !</td>
      <td>4632</td>
      <td>Elisabeth</td>
      <td>Manhattan</td>
      <td>Harlem</td>
      <td>40.80902</td>
      <td>-73.94190</td>
      <td>Private room</td>
      <td>150</td>
      <td>3</td>
      <td>0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1</td>
      <td>365</td>
    </tr>
  </tbody>
</table>
</div>



                                     REMOVING SOME IRRELEVANT CHARACTERS FROM THE VALUES


```python
bn["name"].str.strip("123.,!%$#*-_:;??/}]\|")
```

    <>:1: SyntaxWarning: invalid escape sequence '\|'
    <>:1: SyntaxWarning: invalid escape sequence '\|'
    C:\Users\Windows 10 Pro\AppData\Local\Temp\ipykernel_16812\1309197855.py:1: SyntaxWarning: invalid escape sequence '\|'
      bn["name"].str.strip("123.,!%$#*-_:;??/}]\|")
    




    0                       Clean & quiet apt home by the park
    1                                    Skylit Midtown Castle
    2                       THE VILLAGE OF HARLEM....NEW YORK 
    3                          Cozy Entire Floor of Brownstone
    4         Entire Apt: Spacious Studio/Loft by central park
                                   ...                        
    48890      Charming one bedroom - newly renovated rowhouse
    48891        Affordable room in Bushwick/East Williamsburg
    48892              Sunny Studio at Historical Neighborhood
    48893                 43rd St. Time Square-cozy single bed
    48894    Trendy duplex in the very heart of Hell's Kitchen
    Name: name, Length: 48895, dtype: object




```python
bn["name"] = bn["name"].str.strip("123.,!%$#*-_:;??/}]\|")
```

    <>:1: SyntaxWarning: invalid escape sequence '\|'
    <>:1: SyntaxWarning: invalid escape sequence '\|'
    C:\Users\Windows 10 Pro\AppData\Local\Temp\ipykernel_16812\1340605737.py:1: SyntaxWarning: invalid escape sequence '\|'
      bn["name"] = bn["name"].str.strip("123.,!%$#*-_:;??/}]\|")
    


```python
bn.head()
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
      <th>id</th>
      <th>name</th>
      <th>host_id</th>
      <th>host_name</th>
      <th>neighbourhood_group</th>
      <th>neighbourhood</th>
      <th>latitude</th>
      <th>longitude</th>
      <th>room_type</th>
      <th>price</th>
      <th>minimum_nights</th>
      <th>number_of_reviews</th>
      <th>last_review</th>
      <th>reviews_per_month</th>
      <th>calculated_host_listings_count</th>
      <th>availability_365</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2539</td>
      <td>Clean &amp; quiet apt home by the park</td>
      <td>2787</td>
      <td>John</td>
      <td>Brooklyn</td>
      <td>Kensington</td>
      <td>40.64749</td>
      <td>-73.97237</td>
      <td>Private room</td>
      <td>149</td>
      <td>1</td>
      <td>9</td>
      <td>2018-10-19</td>
      <td>0.21</td>
      <td>6</td>
      <td>365</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2595</td>
      <td>Skylit Midtown Castle</td>
      <td>2845</td>
      <td>Jennifer</td>
      <td>Manhattan</td>
      <td>Midtown</td>
      <td>40.75362</td>
      <td>-73.98377</td>
      <td>Entire home/apt</td>
      <td>225</td>
      <td>1</td>
      <td>45</td>
      <td>2019-05-21</td>
      <td>0.38</td>
      <td>2</td>
      <td>355</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3647</td>
      <td>THE VILLAGE OF HARLEM....NEW YORK</td>
      <td>4632</td>
      <td>Elisabeth</td>
      <td>Manhattan</td>
      <td>Harlem</td>
      <td>40.80902</td>
      <td>-73.94190</td>
      <td>Private room</td>
      <td>150</td>
      <td>3</td>
      <td>0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1</td>
      <td>365</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3831</td>
      <td>Cozy Entire Floor of Brownstone</td>
      <td>4869</td>
      <td>LisaRoxanne</td>
      <td>Brooklyn</td>
      <td>Clinton Hill</td>
      <td>40.68514</td>
      <td>-73.95976</td>
      <td>Entire home/apt</td>
      <td>89</td>
      <td>1</td>
      <td>270</td>
      <td>2019-07-05</td>
      <td>4.64</td>
      <td>1</td>
      <td>194</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5022</td>
      <td>Entire Apt: Spacious Studio/Loft by central park</td>
      <td>7192</td>
      <td>Laura</td>
      <td>Manhattan</td>
      <td>East Harlem</td>
      <td>40.79851</td>
      <td>-73.94399</td>
      <td>Entire home/apt</td>
      <td>80</td>
      <td>10</td>
      <td>9</td>
      <td>2018-11-19</td>
      <td>0.10</td>
      <td>1</td>
      <td>0</td>
    </tr>
  </tbody>
</table>
</div>



                               CHECKING UNIQUE VALUES IN ROOM TYPE COLUMN


```python
bn["room_type"].unique()
```




    array(['Private room', 'Entire home/apt', 'Shared room'], dtype=object)



                                RENAMING SOME VALUES


```python
bn["room_type"].str.replace('Entire home/apt', 'Full Apartment')	
```




    0          Private room
    1        Full Apartment
    2          Private room
    3        Full Apartment
    4        Full Apartment
                  ...      
    48890      Private room
    48891      Private room
    48892    Full Apartment
    48893       Shared room
    48894      Private room
    Name: room_type, Length: 48895, dtype: object




```python
bn["room_type"] = bn["room_type"].str.replace('Entire home/apt', 'Full Apartment')	
```


```python
bn.head(10)
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
      <th>id</th>
      <th>name</th>
      <th>host_id</th>
      <th>host_name</th>
      <th>neighbourhood_group</th>
      <th>neighbourhood</th>
      <th>latitude</th>
      <th>longitude</th>
      <th>room_type</th>
      <th>price</th>
      <th>minimum_nights</th>
      <th>number_of_reviews</th>
      <th>last_review</th>
      <th>reviews_per_month</th>
      <th>calculated_host_listings_count</th>
      <th>availability_365</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2539</td>
      <td>Clean &amp; quiet apt home by the park</td>
      <td>2787</td>
      <td>John</td>
      <td>Brooklyn</td>
      <td>Kensington</td>
      <td>40.64749</td>
      <td>-73.97237</td>
      <td>Private room</td>
      <td>149</td>
      <td>1</td>
      <td>9</td>
      <td>2018-10-19</td>
      <td>0.21</td>
      <td>6</td>
      <td>365</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2595</td>
      <td>Skylit Midtown Castle</td>
      <td>2845</td>
      <td>Jennifer</td>
      <td>Manhattan</td>
      <td>Midtown</td>
      <td>40.75362</td>
      <td>-73.98377</td>
      <td>Full Apartment</td>
      <td>225</td>
      <td>1</td>
      <td>45</td>
      <td>2019-05-21</td>
      <td>0.38</td>
      <td>2</td>
      <td>355</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3647</td>
      <td>THE VILLAGE OF HARLEM....NEW YORK</td>
      <td>4632</td>
      <td>Elisabeth</td>
      <td>Manhattan</td>
      <td>Harlem</td>
      <td>40.80902</td>
      <td>-73.94190</td>
      <td>Private room</td>
      <td>150</td>
      <td>3</td>
      <td>0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>1</td>
      <td>365</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3831</td>
      <td>Cozy Entire Floor of Brownstone</td>
      <td>4869</td>
      <td>LisaRoxanne</td>
      <td>Brooklyn</td>
      <td>Clinton Hill</td>
      <td>40.68514</td>
      <td>-73.95976</td>
      <td>Full Apartment</td>
      <td>89</td>
      <td>1</td>
      <td>270</td>
      <td>2019-07-05</td>
      <td>4.64</td>
      <td>1</td>
      <td>194</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5022</td>
      <td>Entire Apt: Spacious Studio/Loft by central park</td>
      <td>7192</td>
      <td>Laura</td>
      <td>Manhattan</td>
      <td>East Harlem</td>
      <td>40.79851</td>
      <td>-73.94399</td>
      <td>Full Apartment</td>
      <td>80</td>
      <td>10</td>
      <td>9</td>
      <td>2018-11-19</td>
      <td>0.10</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr>
      <th>5</th>
      <td>5099</td>
      <td>Large Cozy 1 BR Apartment In Midtown East</td>
      <td>7322</td>
      <td>Chris</td>
      <td>Manhattan</td>
      <td>Murray Hill</td>
      <td>40.74767</td>
      <td>-73.97500</td>
      <td>Full Apartment</td>
      <td>200</td>
      <td>3</td>
      <td>74</td>
      <td>2019-06-22</td>
      <td>0.59</td>
      <td>1</td>
      <td>129</td>
    </tr>
    <tr>
      <th>6</th>
      <td>5121</td>
      <td>BlissArtsSpace</td>
      <td>7356</td>
      <td>Garon</td>
      <td>Brooklyn</td>
      <td>Bedford-Stuyvesant</td>
      <td>40.68688</td>
      <td>-73.95596</td>
      <td>Private room</td>
      <td>60</td>
      <td>45</td>
      <td>49</td>
      <td>2017-10-05</td>
      <td>0.40</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr>
      <th>7</th>
      <td>5178</td>
      <td>Large Furnished Room Near B'way</td>
      <td>8967</td>
      <td>Shunichi</td>
      <td>Manhattan</td>
      <td>Hell's Kitchen</td>
      <td>40.76489</td>
      <td>-73.98493</td>
      <td>Private room</td>
      <td>79</td>
      <td>2</td>
      <td>430</td>
      <td>2019-06-24</td>
      <td>3.47</td>
      <td>1</td>
      <td>220</td>
    </tr>
    <tr>
      <th>8</th>
      <td>5203</td>
      <td>Cozy Clean Guest Room - Family Apt</td>
      <td>7490</td>
      <td>MaryEllen</td>
      <td>Manhattan</td>
      <td>Upper West Side</td>
      <td>40.80178</td>
      <td>-73.96723</td>
      <td>Private room</td>
      <td>79</td>
      <td>2</td>
      <td>118</td>
      <td>2017-07-21</td>
      <td>0.99</td>
      <td>1</td>
      <td>0</td>
    </tr>
    <tr>
      <th>9</th>
      <td>5238</td>
      <td>Cute &amp; Cozy Lower East Side 1 bdrm</td>
      <td>7549</td>
      <td>Ben</td>
      <td>Manhattan</td>
      <td>Chinatown</td>
      <td>40.71344</td>
      <td>-73.99037</td>
      <td>Full Apartment</td>
      <td>150</td>
      <td>1</td>
      <td>160</td>
      <td>2019-06-09</td>
      <td>1.33</td>
      <td>4</td>
      <td>188</td>
    </tr>
  </tbody>
</table>
</div>



                                         REMOVING NaN VALUES


```python
bn.fillna('')
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
      <th>id</th>
      <th>name</th>
      <th>host_id</th>
      <th>host_name</th>
      <th>neighbourhood_group</th>
      <th>neighbourhood</th>
      <th>latitude</th>
      <th>longitude</th>
      <th>room_type</th>
      <th>price</th>
      <th>minimum_nights</th>
      <th>number_of_reviews</th>
      <th>last_review</th>
      <th>reviews_per_month</th>
      <th>calculated_host_listings_count</th>
      <th>availability_365</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2539</td>
      <td>Clean &amp; quiet apt home by the park</td>
      <td>2787</td>
      <td>John</td>
      <td>Brooklyn</td>
      <td>Kensington</td>
      <td>40.64749</td>
      <td>-73.97237</td>
      <td>Private room</td>
      <td>149</td>
      <td>1</td>
      <td>9</td>
      <td>2018-10-19</td>
      <td>0.21</td>
      <td>6</td>
      <td>365</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2595</td>
      <td>Skylit Midtown Castle</td>
      <td>2845</td>
      <td>Jennifer</td>
      <td>Manhattan</td>
      <td>Midtown</td>
      <td>40.75362</td>
      <td>-73.98377</td>
      <td>Full Apartment</td>
      <td>225</td>
      <td>1</td>
      <td>45</td>
      <td>2019-05-21</td>
      <td>0.38</td>
      <td>2</td>
      <td>355</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3647</td>
      <td>THE VILLAGE OF HARLEM....NEW YORK</td>
      <td>4632</td>
      <td>Elisabeth</td>
      <td>Manhattan</td>
      <td>Harlem</td>
      <td>40.80902</td>
      <td>-73.94190</td>
      <td>Private room</td>
      <td>150</td>
      <td>3</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>1</td>
      <td>365</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3831</td>
      <td>Cozy Entire Floor of Brownstone</td>
      <td>4869</td>
      <td>LisaRoxanne</td>
      <td>Brooklyn</td>
      <td>Clinton Hill</td>
      <td>40.68514</td>
      <td>-73.95976</td>
      <td>Full Apartment</td>
      <td>89</td>
      <td>1</td>
      <td>270</td>
      <td>2019-07-05</td>
      <td>4.64</td>
      <td>1</td>
      <td>194</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5022</td>
      <td>Entire Apt: Spacious Studio/Loft by central park</td>
      <td>7192</td>
      <td>Laura</td>
      <td>Manhattan</td>
      <td>East Harlem</td>
      <td>40.79851</td>
      <td>-73.94399</td>
      <td>Full Apartment</td>
      <td>80</td>
      <td>10</td>
      <td>9</td>
      <td>2018-11-19</td>
      <td>0.1</td>
      <td>1</td>
      <td>0</td>
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
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>48890</th>
      <td>36484665</td>
      <td>Charming one bedroom - newly renovated rowhouse</td>
      <td>8232441</td>
      <td>Sabrina</td>
      <td>Brooklyn</td>
      <td>Bedford-Stuyvesant</td>
      <td>40.67853</td>
      <td>-73.94995</td>
      <td>Private room</td>
      <td>70</td>
      <td>2</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>2</td>
      <td>9</td>
    </tr>
    <tr>
      <th>48891</th>
      <td>36485057</td>
      <td>Affordable room in Bushwick/East Williamsburg</td>
      <td>6570630</td>
      <td>Marisol</td>
      <td>Brooklyn</td>
      <td>Bushwick</td>
      <td>40.70184</td>
      <td>-73.93317</td>
      <td>Private room</td>
      <td>40</td>
      <td>4</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>2</td>
      <td>36</td>
    </tr>
    <tr>
      <th>48892</th>
      <td>36485431</td>
      <td>Sunny Studio at Historical Neighborhood</td>
      <td>23492952</td>
      <td>Ilgar &amp; Aysel</td>
      <td>Manhattan</td>
      <td>Harlem</td>
      <td>40.81475</td>
      <td>-73.94867</td>
      <td>Full Apartment</td>
      <td>115</td>
      <td>10</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>1</td>
      <td>27</td>
    </tr>
    <tr>
      <th>48893</th>
      <td>36485609</td>
      <td>43rd St. Time Square-cozy single bed</td>
      <td>30985759</td>
      <td>Taz</td>
      <td>Manhattan</td>
      <td>Hell's Kitchen</td>
      <td>40.75751</td>
      <td>-73.99112</td>
      <td>Shared room</td>
      <td>55</td>
      <td>1</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>6</td>
      <td>2</td>
    </tr>
    <tr>
      <th>48894</th>
      <td>36487245</td>
      <td>Trendy duplex in the very heart of Hell's Kitchen</td>
      <td>68119814</td>
      <td>Christophe</td>
      <td>Manhattan</td>
      <td>Hell's Kitchen</td>
      <td>40.76404</td>
      <td>-73.98933</td>
      <td>Private room</td>
      <td>90</td>
      <td>7</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>1</td>
      <td>23</td>
    </tr>
  </tbody>
</table>
<p>48895 rows × 16 columns</p>
</div>




```python
bn = bn.fillna('')
```


```python
bn.head(2)
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
      <th>id</th>
      <th>name</th>
      <th>host_id</th>
      <th>host_name</th>
      <th>neighbourhood_group</th>
      <th>neighbourhood</th>
      <th>latitude</th>
      <th>longitude</th>
      <th>room_type</th>
      <th>price</th>
      <th>minimum_nights</th>
      <th>number_of_reviews</th>
      <th>last_review</th>
      <th>reviews_per_month</th>
      <th>calculated_host_listings_count</th>
      <th>availability_365</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2539</td>
      <td>Clean &amp; quiet apt home by the park</td>
      <td>2787</td>
      <td>John</td>
      <td>Brooklyn</td>
      <td>Kensington</td>
      <td>40.64749</td>
      <td>-73.97237</td>
      <td>Private room</td>
      <td>149</td>
      <td>1</td>
      <td>9</td>
      <td>2018-10-19</td>
      <td>0.21</td>
      <td>6</td>
      <td>365</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2595</td>
      <td>Skylit Midtown Castle</td>
      <td>2845</td>
      <td>Jennifer</td>
      <td>Manhattan</td>
      <td>Midtown</td>
      <td>40.75362</td>
      <td>-73.98377</td>
      <td>Full Apartment</td>
      <td>225</td>
      <td>1</td>
      <td>45</td>
      <td>2019-05-21</td>
      <td>0.38</td>
      <td>2</td>
      <td>355</td>
    </tr>
  </tbody>
</table>
</div>



                                          STANDARDIZE COLUMNS NAME BY RENAME IT


```python
bn.rename(columns = {'id': 'Apartment_Id'}, inplace=True)
bn.rename(columns = {'name': 'Name'}, inplace=True)
bn.rename(columns = {'host_id': 'Host_Id'}, inplace=True)
bn.rename(columns = {'host_name': 'Host_Name'}, inplace=True)
bn.rename(columns = {'neighbourhood_group': 'City'}, inplace=True)
bn.rename(columns = {'neighbourhood': 'Neighbourhood'}, inplace=True)
bn.rename(columns = {'latitude': 'Latitude'}, inplace=True)
bn.rename(columns = {'longitude': 'Longitude'}, inplace=True)
bn.rename(columns = {'room_type': 'Room_Type'}, inplace=True)
bn.rename(columns = {'price': 'Price'}, inplace=True)
bn.rename(columns = {'minimum_nights': 'Minimum_Nights'}, inplace=True)
bn.rename(columns = {'number_of_reviews': 'Total_Reviews'}, inplace=True)
bn.rename(columns = {'last_review': 'Last_Review'}, inplace=True)
bn.rename(columns = {'reviews_per_month': 'Monthly_Review'}, inplace=True)
bn.rename(columns = {'calculated_host_listings_count': 'Calculated_Host_Listings_Count'}, inplace=True)
bn.rename(columns = {'availability_365': 'Availability_365'}, inplace=True)

```


```python
bn.head(5)
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
      <th>Apartment_Id</th>
      <th>Name</th>
      <th>Host_Id</th>
      <th>Host_Name</th>
      <th>City</th>
      <th>Neighbourhood</th>
      <th>Latitude</th>
      <th>Longitude</th>
      <th>Room_Type</th>
      <th>Price</th>
      <th>Minimum_Nights</th>
      <th>Total_Reviews</th>
      <th>Last_Review</th>
      <th>Monthly_Review</th>
      <th>Calculated_Host_Listings_Count</th>
      <th>Availability_365</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2539</td>
      <td>Clean &amp; quiet apt home by the park</td>
      <td>2787</td>
      <td>John</td>
      <td>Brooklyn</td>
      <td>Kensington</td>
      <td>40.64749</td>
      <td>-73.97237</td>
      <td>Private room</td>
      <td>149</td>
      <td>1</td>
      <td>9</td>
      <td>2018-10-19</td>
      <td>0.21</td>
      <td>6</td>
      <td>365</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2595</td>
      <td>Skylit Midtown Castle</td>
      <td>2845</td>
      <td>Jennifer</td>
      <td>Manhattan</td>
      <td>Midtown</td>
      <td>40.75362</td>
      <td>-73.98377</td>
      <td>Full Apartment</td>
      <td>225</td>
      <td>1</td>
      <td>45</td>
      <td>2019-05-21</td>
      <td>0.38</td>
      <td>2</td>
      <td>355</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3647</td>
      <td>THE VILLAGE OF HARLEM....NEW YORK</td>
      <td>4632</td>
      <td>Elisabeth</td>
      <td>Manhattan</td>
      <td>Harlem</td>
      <td>40.80902</td>
      <td>-73.94190</td>
      <td>Private room</td>
      <td>150</td>
      <td>3</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>1</td>
      <td>365</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3831</td>
      <td>Cozy Entire Floor of Brownstone</td>
      <td>4869</td>
      <td>LisaRoxanne</td>
      <td>Brooklyn</td>
      <td>Clinton Hill</td>
      <td>40.68514</td>
      <td>-73.95976</td>
      <td>Full Apartment</td>
      <td>89</td>
      <td>1</td>
      <td>270</td>
      <td>2019-07-05</td>
      <td>4.64</td>
      <td>1</td>
      <td>194</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5022</td>
      <td>Entire Apt: Spacious Studio/Loft by central park</td>
      <td>7192</td>
      <td>Laura</td>
      <td>Manhattan</td>
      <td>East Harlem</td>
      <td>40.79851</td>
      <td>-73.94399</td>
      <td>Full Apartment</td>
      <td>80</td>
      <td>10</td>
      <td>9</td>
      <td>2018-11-19</td>
      <td>0.1</td>
      <td>1</td>
      <td>0</td>
    </tr>
  </tbody>
</table>
</div>




```python
bn["Name"] = bn["Name"].str.lower()
```


```python
bn
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
      <th>Apartment_Id</th>
      <th>Name</th>
      <th>Host_Id</th>
      <th>Host_Name</th>
      <th>City</th>
      <th>Neighbourhood</th>
      <th>Latitude</th>
      <th>Longitude</th>
      <th>Room_Type</th>
      <th>Price</th>
      <th>Minimum_Nights</th>
      <th>Total_Reviews</th>
      <th>Last_Review</th>
      <th>Monthly_Review</th>
      <th>Calculated_Host_Listings_Count</th>
      <th>Availability_365</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2539</td>
      <td>clean &amp; quiet apt home by the park</td>
      <td>2787</td>
      <td>John</td>
      <td>Brooklyn</td>
      <td>Kensington</td>
      <td>40.64749</td>
      <td>-73.97237</td>
      <td>Private room</td>
      <td>149</td>
      <td>1</td>
      <td>9</td>
      <td>2018-10-19</td>
      <td>0.21</td>
      <td>6</td>
      <td>365</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2595</td>
      <td>skylit midtown castle</td>
      <td>2845</td>
      <td>Jennifer</td>
      <td>Manhattan</td>
      <td>Midtown</td>
      <td>40.75362</td>
      <td>-73.98377</td>
      <td>Full Apartment</td>
      <td>225</td>
      <td>1</td>
      <td>45</td>
      <td>2019-05-21</td>
      <td>0.38</td>
      <td>2</td>
      <td>355</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3647</td>
      <td>the village of harlem....new york</td>
      <td>4632</td>
      <td>Elisabeth</td>
      <td>Manhattan</td>
      <td>Harlem</td>
      <td>40.80902</td>
      <td>-73.94190</td>
      <td>Private room</td>
      <td>150</td>
      <td>3</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>1</td>
      <td>365</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3831</td>
      <td>cozy entire floor of brownstone</td>
      <td>4869</td>
      <td>LisaRoxanne</td>
      <td>Brooklyn</td>
      <td>Clinton Hill</td>
      <td>40.68514</td>
      <td>-73.95976</td>
      <td>Full Apartment</td>
      <td>89</td>
      <td>1</td>
      <td>270</td>
      <td>2019-07-05</td>
      <td>4.64</td>
      <td>1</td>
      <td>194</td>
    </tr>
    <tr>
      <th>4</th>
      <td>5022</td>
      <td>entire apt: spacious studio/loft by central park</td>
      <td>7192</td>
      <td>Laura</td>
      <td>Manhattan</td>
      <td>East Harlem</td>
      <td>40.79851</td>
      <td>-73.94399</td>
      <td>Full Apartment</td>
      <td>80</td>
      <td>10</td>
      <td>9</td>
      <td>2018-11-19</td>
      <td>0.1</td>
      <td>1</td>
      <td>0</td>
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
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>48890</th>
      <td>36484665</td>
      <td>charming one bedroom - newly renovated rowhouse</td>
      <td>8232441</td>
      <td>Sabrina</td>
      <td>Brooklyn</td>
      <td>Bedford-Stuyvesant</td>
      <td>40.67853</td>
      <td>-73.94995</td>
      <td>Private room</td>
      <td>70</td>
      <td>2</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>2</td>
      <td>9</td>
    </tr>
    <tr>
      <th>48891</th>
      <td>36485057</td>
      <td>affordable room in bushwick/east williamsburg</td>
      <td>6570630</td>
      <td>Marisol</td>
      <td>Brooklyn</td>
      <td>Bushwick</td>
      <td>40.70184</td>
      <td>-73.93317</td>
      <td>Private room</td>
      <td>40</td>
      <td>4</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>2</td>
      <td>36</td>
    </tr>
    <tr>
      <th>48892</th>
      <td>36485431</td>
      <td>sunny studio at historical neighborhood</td>
      <td>23492952</td>
      <td>Ilgar &amp; Aysel</td>
      <td>Manhattan</td>
      <td>Harlem</td>
      <td>40.81475</td>
      <td>-73.94867</td>
      <td>Full Apartment</td>
      <td>115</td>
      <td>10</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>1</td>
      <td>27</td>
    </tr>
    <tr>
      <th>48893</th>
      <td>36485609</td>
      <td>43rd st. time square-cozy single bed</td>
      <td>30985759</td>
      <td>Taz</td>
      <td>Manhattan</td>
      <td>Hell's Kitchen</td>
      <td>40.75751</td>
      <td>-73.99112</td>
      <td>Shared room</td>
      <td>55</td>
      <td>1</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>6</td>
      <td>2</td>
    </tr>
    <tr>
      <th>48894</th>
      <td>36487245</td>
      <td>trendy duplex in the very heart of hell's kitchen</td>
      <td>68119814</td>
      <td>Christophe</td>
      <td>Manhattan</td>
      <td>Hell's Kitchen</td>
      <td>40.76404</td>
      <td>-73.98933</td>
      <td>Private room</td>
      <td>90</td>
      <td>7</td>
      <td>0</td>
      <td></td>
      <td></td>
      <td>1</td>
      <td>23</td>
    </tr>
  </tbody>
</table>
<p>48895 rows × 16 columns</p>
</div>




```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```
