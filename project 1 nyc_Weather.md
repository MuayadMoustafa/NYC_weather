```python
import pandas as pd
```


```python
df = pd.read_csv("Desktop/nyc_weather.csv")
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
      <th>EST</th>
      <th>Temperature</th>
      <th>DewPoint</th>
      <th>Humidity</th>
      <th>Sea Level PressureIn</th>
      <th>VisibilityMiles</th>
      <th>WindSpeedMPH</th>
      <th>PrecipitationIn</th>
      <th>CloudCover</th>
      <th>Events</th>
      <th>WindDirDegrees</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1/1/2016</td>
      <td>38</td>
      <td>23</td>
      <td>52</td>
      <td>30.03</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>5</td>
      <td>NaN</td>
      <td>281</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1/2/2016</td>
      <td>36</td>
      <td>18</td>
      <td>46</td>
      <td>30.02</td>
      <td>10</td>
      <td>7.0</td>
      <td>0</td>
      <td>3</td>
      <td>NaN</td>
      <td>275</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1/3/2016</td>
      <td>40</td>
      <td>21</td>
      <td>47</td>
      <td>29.86</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>277</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1/4/2016</td>
      <td>25</td>
      <td>9</td>
      <td>44</td>
      <td>30.05</td>
      <td>10</td>
      <td>9.0</td>
      <td>0</td>
      <td>3</td>
      <td>NaN</td>
      <td>345</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1/5/2016</td>
      <td>20</td>
      <td>-3</td>
      <td>41</td>
      <td>30.57</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>333</td>
    </tr>
    <tr>
      <th>5</th>
      <td>1/6/2016</td>
      <td>33</td>
      <td>4</td>
      <td>35</td>
      <td>30.50</td>
      <td>10</td>
      <td>4.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>259</td>
    </tr>
    <tr>
      <th>6</th>
      <td>1/7/2016</td>
      <td>39</td>
      <td>11</td>
      <td>33</td>
      <td>30.28</td>
      <td>10</td>
      <td>2.0</td>
      <td>0</td>
      <td>3</td>
      <td>NaN</td>
      <td>293</td>
    </tr>
    <tr>
      <th>7</th>
      <td>1/8/2016</td>
      <td>39</td>
      <td>29</td>
      <td>64</td>
      <td>30.20</td>
      <td>10</td>
      <td>4.0</td>
      <td>0</td>
      <td>8</td>
      <td>NaN</td>
      <td>79</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1/9/2016</td>
      <td>44</td>
      <td>38</td>
      <td>77</td>
      <td>30.16</td>
      <td>9</td>
      <td>8.0</td>
      <td>T</td>
      <td>8</td>
      <td>Rain</td>
      <td>76</td>
    </tr>
    <tr>
      <th>9</th>
      <td>1/10/2016</td>
      <td>50</td>
      <td>46</td>
      <td>71</td>
      <td>29.59</td>
      <td>4</td>
      <td>NaN</td>
      <td>1.8</td>
      <td>7</td>
      <td>Rain</td>
      <td>109</td>
    </tr>
    <tr>
      <th>10</th>
      <td>1/11/2016</td>
      <td>33</td>
      <td>8</td>
      <td>37</td>
      <td>29.92</td>
      <td>10</td>
      <td>NaN</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>289</td>
    </tr>
    <tr>
      <th>11</th>
      <td>1/12/2016</td>
      <td>35</td>
      <td>15</td>
      <td>53</td>
      <td>29.85</td>
      <td>10</td>
      <td>6.0</td>
      <td>T</td>
      <td>4</td>
      <td>NaN</td>
      <td>235</td>
    </tr>
    <tr>
      <th>12</th>
      <td>1/13/2016</td>
      <td>26</td>
      <td>4</td>
      <td>42</td>
      <td>29.94</td>
      <td>10</td>
      <td>10.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>284</td>
    </tr>
    <tr>
      <th>13</th>
      <td>1/14/2016</td>
      <td>30</td>
      <td>12</td>
      <td>47</td>
      <td>29.95</td>
      <td>10</td>
      <td>5.0</td>
      <td>T</td>
      <td>7</td>
      <td>NaN</td>
      <td>266</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1/15/2016</td>
      <td>43</td>
      <td>31</td>
      <td>62</td>
      <td>29.82</td>
      <td>9</td>
      <td>5.0</td>
      <td>T</td>
      <td>2</td>
      <td>NaN</td>
      <td>101</td>
    </tr>
    <tr>
      <th>15</th>
      <td>1/16/2016</td>
      <td>47</td>
      <td>37</td>
      <td>70</td>
      <td>29.52</td>
      <td>8</td>
      <td>7.0</td>
      <td>0.24</td>
      <td>7</td>
      <td>Rain</td>
      <td>340</td>
    </tr>
    <tr>
      <th>16</th>
      <td>1/17/2016</td>
      <td>36</td>
      <td>23</td>
      <td>66</td>
      <td>29.78</td>
      <td>8</td>
      <td>6.0</td>
      <td>0.05</td>
      <td>6</td>
      <td>Fog-Snow</td>
      <td>345</td>
    </tr>
    <tr>
      <th>17</th>
      <td>1/18/2016</td>
      <td>25</td>
      <td>6</td>
      <td>53</td>
      <td>29.83</td>
      <td>9</td>
      <td>12.0</td>
      <td>T</td>
      <td>2</td>
      <td>Snow</td>
      <td>293</td>
    </tr>
    <tr>
      <th>18</th>
      <td>1/19/2016</td>
      <td>22</td>
      <td>3</td>
      <td>42</td>
      <td>30.03</td>
      <td>10</td>
      <td>11.0</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>293</td>
    </tr>
    <tr>
      <th>19</th>
      <td>1/20/2016</td>
      <td>32</td>
      <td>15</td>
      <td>49</td>
      <td>30.13</td>
      <td>10</td>
      <td>6.0</td>
      <td>0</td>
      <td>2</td>
      <td>NaN</td>
      <td>302</td>
    </tr>
    <tr>
      <th>20</th>
      <td>1/21/2016</td>
      <td>31</td>
      <td>11</td>
      <td>45</td>
      <td>30.15</td>
      <td>10</td>
      <td>6.0</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>312</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1/22/2016</td>
      <td>26</td>
      <td>6</td>
      <td>41</td>
      <td>30.21</td>
      <td>9</td>
      <td>NaN</td>
      <td>0.01</td>
      <td>3</td>
      <td>Snow</td>
      <td>34</td>
    </tr>
    <tr>
      <th>22</th>
      <td>1/23/2016</td>
      <td>26</td>
      <td>21</td>
      <td>78</td>
      <td>29.77</td>
      <td>1</td>
      <td>16.0</td>
      <td>2.31</td>
      <td>8</td>
      <td>Fog-Snow</td>
      <td>42</td>
    </tr>
    <tr>
      <th>23</th>
      <td>1/24/2016</td>
      <td>28</td>
      <td>11</td>
      <td>53</td>
      <td>29.92</td>
      <td>8</td>
      <td>6.0</td>
      <td>T</td>
      <td>3</td>
      <td>Snow</td>
      <td>327</td>
    </tr>
    <tr>
      <th>24</th>
      <td>1/25/2016</td>
      <td>34</td>
      <td>18</td>
      <td>54</td>
      <td>30.25</td>
      <td>10</td>
      <td>3.0</td>
      <td>0</td>
      <td>2</td>
      <td>NaN</td>
      <td>286</td>
    </tr>
    <tr>
      <th>25</th>
      <td>1/26/2016</td>
      <td>43</td>
      <td>29</td>
      <td>56</td>
      <td>30.03</td>
      <td>10</td>
      <td>7.0</td>
      <td>0</td>
      <td>2</td>
      <td>NaN</td>
      <td>244</td>
    </tr>
    <tr>
      <th>26</th>
      <td>1/27/2016</td>
      <td>41</td>
      <td>22</td>
      <td>45</td>
      <td>30.03</td>
      <td>10</td>
      <td>7.0</td>
      <td>T</td>
      <td>3</td>
      <td>Rain</td>
      <td>311</td>
    </tr>
    <tr>
      <th>27</th>
      <td>1/28/2016</td>
      <td>37</td>
      <td>20</td>
      <td>51</td>
      <td>29.90</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>234</td>
    </tr>
    <tr>
      <th>28</th>
      <td>1/29/2016</td>
      <td>36</td>
      <td>21</td>
      <td>50</td>
      <td>29.58</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>4</td>
      <td>NaN</td>
      <td>298</td>
    </tr>
    <tr>
      <th>29</th>
      <td>1/30/2016</td>
      <td>34</td>
      <td>16</td>
      <td>46</td>
      <td>30.01</td>
      <td>10</td>
      <td>7.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>257</td>
    </tr>
    <tr>
      <th>30</th>
      <td>1/31/2016</td>
      <td>46</td>
      <td>28</td>
      <td>52</td>
      <td>29.90</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>241</td>
    </tr>
  </tbody>
</table>
</div>




```python
df["WindDirDegrees"]
```




    0     281
    1     275
    2     277
    3     345
    4     333
    5     259
    6     293
    7      79
    8      76
    9     109
    10    289
    11    235
    12    284
    13    266
    14    101
    15    340
    16    345
    17    293
    18    293
    19    302
    20    312
    21     34
    22     42
    23    327
    24    286
    25    244
    26    311
    27    234
    28    298
    29    257
    30    241
    Name: WindDirDegrees, dtype: int64




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
      <th>Temperature</th>
      <th>DewPoint</th>
      <th>Humidity</th>
      <th>Sea Level PressureIn</th>
      <th>VisibilityMiles</th>
      <th>WindSpeedMPH</th>
      <th>CloudCover</th>
      <th>WindDirDegrees</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>28.000000</td>
      <td>31.000000</td>
      <td>31.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>34.677419</td>
      <td>17.838710</td>
      <td>51.677419</td>
      <td>29.992903</td>
      <td>9.193548</td>
      <td>6.892857</td>
      <td>3.129032</td>
      <td>247.129032</td>
    </tr>
    <tr>
      <th>std</th>
      <td>7.639315</td>
      <td>11.378626</td>
      <td>11.634395</td>
      <td>0.237237</td>
      <td>1.939405</td>
      <td>2.871821</td>
      <td>2.629853</td>
      <td>92.308086</td>
    </tr>
    <tr>
      <th>min</th>
      <td>20.000000</td>
      <td>-3.000000</td>
      <td>33.000000</td>
      <td>29.520000</td>
      <td>1.000000</td>
      <td>2.000000</td>
      <td>0.000000</td>
      <td>34.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>29.000000</td>
      <td>10.000000</td>
      <td>44.500000</td>
      <td>29.855000</td>
      <td>9.000000</td>
      <td>5.000000</td>
      <td>1.000000</td>
      <td>238.000000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>35.000000</td>
      <td>18.000000</td>
      <td>50.000000</td>
      <td>30.010000</td>
      <td>10.000000</td>
      <td>6.500000</td>
      <td>3.000000</td>
      <td>281.000000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>39.500000</td>
      <td>23.000000</td>
      <td>55.000000</td>
      <td>30.140000</td>
      <td>10.000000</td>
      <td>8.000000</td>
      <td>4.500000</td>
      <td>300.000000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>50.000000</td>
      <td>46.000000</td>
      <td>78.000000</td>
      <td>30.570000</td>
      <td>10.000000</td>
      <td>16.000000</td>
      <td>8.000000</td>
      <td>345.000000</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.head()
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
      <th>EST</th>
      <th>Temperature</th>
      <th>DewPoint</th>
      <th>Humidity</th>
      <th>Sea Level PressureIn</th>
      <th>VisibilityMiles</th>
      <th>WindSpeedMPH</th>
      <th>PrecipitationIn</th>
      <th>CloudCover</th>
      <th>Events</th>
      <th>WindDirDegrees</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1/1/2016</td>
      <td>38</td>
      <td>23</td>
      <td>52</td>
      <td>30.03</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>5</td>
      <td>NaN</td>
      <td>281</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1/2/2016</td>
      <td>36</td>
      <td>18</td>
      <td>46</td>
      <td>30.02</td>
      <td>10</td>
      <td>7.0</td>
      <td>0</td>
      <td>3</td>
      <td>NaN</td>
      <td>275</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1/3/2016</td>
      <td>40</td>
      <td>21</td>
      <td>47</td>
      <td>29.86</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>277</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1/4/2016</td>
      <td>25</td>
      <td>9</td>
      <td>44</td>
      <td>30.05</td>
      <td>10</td>
      <td>9.0</td>
      <td>0</td>
      <td>3</td>
      <td>NaN</td>
      <td>345</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1/5/2016</td>
      <td>20</td>
      <td>-3</td>
      <td>41</td>
      <td>30.57</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>333</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.mean()
```

    C:\Users\Mua\AppData\Local\Temp/ipykernel_9156/3698961737.py:1: FutureWarning: Dropping of nuisance columns in DataFrame reductions (with 'numeric_only=None') is deprecated; in a future version this will raise TypeError.  Select only valid columns before calling the reduction.
      df.mean()
    




    Temperature              34.677419
    DewPoint                 17.838710
    Humidity                 51.677419
    Sea Level PressureIn     29.992903
    VisibilityMiles           9.193548
    WindSpeedMPH              6.892857
    CloudCover                3.129032
    WindDirDegrees          247.129032
    dtype: float64




```python
df.median()
```

    C:\Users\Mua\AppData\Local\Temp/ipykernel_9156/530051474.py:1: FutureWarning: Dropping of nuisance columns in DataFrame reductions (with 'numeric_only=None') is deprecated; in a future version this will raise TypeError.  Select only valid columns before calling the reduction.
      df.median()
    




    Temperature              35.00
    DewPoint                 18.00
    Humidity                 50.00
    Sea Level PressureIn     30.01
    VisibilityMiles          10.00
    WindSpeedMPH              6.50
    CloudCover                3.00
    WindDirDegrees          281.00
    dtype: float64




```python
df.mode()
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
      <th>EST</th>
      <th>Temperature</th>
      <th>DewPoint</th>
      <th>Humidity</th>
      <th>Sea Level PressureIn</th>
      <th>VisibilityMiles</th>
      <th>WindSpeedMPH</th>
      <th>PrecipitationIn</th>
      <th>CloudCover</th>
      <th>Events</th>
      <th>WindDirDegrees</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1/1/2016</td>
      <td>26.0</td>
      <td>11.0</td>
      <td>53.0</td>
      <td>30.03</td>
      <td>10.0</td>
      <td>5.0</td>
      <td>0</td>
      <td>3.0</td>
      <td>Rain</td>
      <td>293.0</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1/10/2016</td>
      <td>36.0</td>
      <td>21.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>6.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1/11/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>7.0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1/12/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1/13/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>5</th>
      <td>1/14/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>6</th>
      <td>1/15/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>7</th>
      <td>1/16/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1/17/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>9</th>
      <td>1/18/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>10</th>
      <td>1/19/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>11</th>
      <td>1/2/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>12</th>
      <td>1/20/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>13</th>
      <td>1/21/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1/22/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>15</th>
      <td>1/23/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>16</th>
      <td>1/24/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>17</th>
      <td>1/25/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>18</th>
      <td>1/26/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>19</th>
      <td>1/27/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>20</th>
      <td>1/28/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1/29/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>22</th>
      <td>1/3/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>23</th>
      <td>1/30/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>24</th>
      <td>1/31/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>25</th>
      <td>1/4/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>26</th>
      <td>1/5/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>27</th>
      <td>1/6/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>28</th>
      <td>1/7/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>29</th>
      <td>1/8/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>30</th>
      <td>1/9/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>




```python
for i in df.Humidity:
    if (i<50):
        print(i)
```

    46
    47
    44
    41
    35
    33
    37
    42
    47
    42
    49
    45
    41
    45
    46
    


```python
df.tail()
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
      <th>EST</th>
      <th>Temperature</th>
      <th>DewPoint</th>
      <th>Humidity</th>
      <th>Sea Level PressureIn</th>
      <th>VisibilityMiles</th>
      <th>WindSpeedMPH</th>
      <th>PrecipitationIn</th>
      <th>CloudCover</th>
      <th>Events</th>
      <th>WindDirDegrees</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>26</th>
      <td>1/27/2016</td>
      <td>41</td>
      <td>22</td>
      <td>45</td>
      <td>30.03</td>
      <td>10</td>
      <td>7.0</td>
      <td>T</td>
      <td>3</td>
      <td>Rain</td>
      <td>311</td>
    </tr>
    <tr>
      <th>27</th>
      <td>1/28/2016</td>
      <td>37</td>
      <td>20</td>
      <td>51</td>
      <td>29.90</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>234</td>
    </tr>
    <tr>
      <th>28</th>
      <td>1/29/2016</td>
      <td>36</td>
      <td>21</td>
      <td>50</td>
      <td>29.58</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>4</td>
      <td>NaN</td>
      <td>298</td>
    </tr>
    <tr>
      <th>29</th>
      <td>1/30/2016</td>
      <td>34</td>
      <td>16</td>
      <td>46</td>
      <td>30.01</td>
      <td>10</td>
      <td>7.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>257</td>
    </tr>
    <tr>
      <th>30</th>
      <td>1/31/2016</td>
      <td>46</td>
      <td>28</td>
      <td>52</td>
      <td>29.90</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>241</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.shape[0]
```




    31




```python
df.columns
```




    Index(['EST', 'Temperature', 'DewPoint', 'Humidity', 'Sea Level PressureIn',
           'VisibilityMiles', 'WindSpeedMPH', 'PrecipitationIn', 'CloudCover',
           'Events', 'WindDirDegrees'],
          dtype='object')




```python
df.index
```




    RangeIndex(start=0, stop=31, step=1)




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
      <th>Temperature</th>
      <th>DewPoint</th>
      <th>Humidity</th>
      <th>Sea Level PressureIn</th>
      <th>VisibilityMiles</th>
      <th>WindSpeedMPH</th>
      <th>CloudCover</th>
      <th>WindDirDegrees</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>28.000000</td>
      <td>31.000000</td>
      <td>31.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>34.677419</td>
      <td>17.838710</td>
      <td>51.677419</td>
      <td>29.992903</td>
      <td>9.193548</td>
      <td>6.892857</td>
      <td>3.129032</td>
      <td>247.129032</td>
    </tr>
    <tr>
      <th>std</th>
      <td>7.639315</td>
      <td>11.378626</td>
      <td>11.634395</td>
      <td>0.237237</td>
      <td>1.939405</td>
      <td>2.871821</td>
      <td>2.629853</td>
      <td>92.308086</td>
    </tr>
    <tr>
      <th>min</th>
      <td>20.000000</td>
      <td>-3.000000</td>
      <td>33.000000</td>
      <td>29.520000</td>
      <td>1.000000</td>
      <td>2.000000</td>
      <td>0.000000</td>
      <td>34.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>29.000000</td>
      <td>10.000000</td>
      <td>44.500000</td>
      <td>29.855000</td>
      <td>9.000000</td>
      <td>5.000000</td>
      <td>1.000000</td>
      <td>238.000000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>35.000000</td>
      <td>18.000000</td>
      <td>50.000000</td>
      <td>30.010000</td>
      <td>10.000000</td>
      <td>6.500000</td>
      <td>3.000000</td>
      <td>281.000000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>39.500000</td>
      <td>23.000000</td>
      <td>55.000000</td>
      <td>30.140000</td>
      <td>10.000000</td>
      <td>8.000000</td>
      <td>4.500000</td>
      <td>300.000000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>50.000000</td>
      <td>46.000000</td>
      <td>78.000000</td>
      <td>30.570000</td>
      <td>10.000000</td>
      <td>16.000000</td>
      <td>8.000000</td>
      <td>345.000000</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.Humidity.mode()
```




    0    53
    dtype: int64




```python
df.describe(include="all")
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
      <th>EST</th>
      <th>Temperature</th>
      <th>DewPoint</th>
      <th>Humidity</th>
      <th>Sea Level PressureIn</th>
      <th>VisibilityMiles</th>
      <th>WindSpeedMPH</th>
      <th>PrecipitationIn</th>
      <th>CloudCover</th>
      <th>Events</th>
      <th>WindDirDegrees</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>31</td>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>31.000000</td>
      <td>28.000000</td>
      <td>31</td>
      <td>31.000000</td>
      <td>9</td>
      <td>31.000000</td>
    </tr>
    <tr>
      <th>unique</th>
      <td>31</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>7</td>
      <td>NaN</td>
      <td>3</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>top</th>
      <td>1/1/2016</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>0</td>
      <td>NaN</td>
      <td>Rain</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>freq</th>
      <td>1</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>19</td>
      <td>NaN</td>
      <td>4</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>NaN</td>
      <td>34.677419</td>
      <td>17.838710</td>
      <td>51.677419</td>
      <td>29.992903</td>
      <td>9.193548</td>
      <td>6.892857</td>
      <td>NaN</td>
      <td>3.129032</td>
      <td>NaN</td>
      <td>247.129032</td>
    </tr>
    <tr>
      <th>std</th>
      <td>NaN</td>
      <td>7.639315</td>
      <td>11.378626</td>
      <td>11.634395</td>
      <td>0.237237</td>
      <td>1.939405</td>
      <td>2.871821</td>
      <td>NaN</td>
      <td>2.629853</td>
      <td>NaN</td>
      <td>92.308086</td>
    </tr>
    <tr>
      <th>min</th>
      <td>NaN</td>
      <td>20.000000</td>
      <td>-3.000000</td>
      <td>33.000000</td>
      <td>29.520000</td>
      <td>1.000000</td>
      <td>2.000000</td>
      <td>NaN</td>
      <td>0.000000</td>
      <td>NaN</td>
      <td>34.000000</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>NaN</td>
      <td>29.000000</td>
      <td>10.000000</td>
      <td>44.500000</td>
      <td>29.855000</td>
      <td>9.000000</td>
      <td>5.000000</td>
      <td>NaN</td>
      <td>1.000000</td>
      <td>NaN</td>
      <td>238.000000</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>NaN</td>
      <td>35.000000</td>
      <td>18.000000</td>
      <td>50.000000</td>
      <td>30.010000</td>
      <td>10.000000</td>
      <td>6.500000</td>
      <td>NaN</td>
      <td>3.000000</td>
      <td>NaN</td>
      <td>281.000000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>NaN</td>
      <td>39.500000</td>
      <td>23.000000</td>
      <td>55.000000</td>
      <td>30.140000</td>
      <td>10.000000</td>
      <td>8.000000</td>
      <td>NaN</td>
      <td>4.500000</td>
      <td>NaN</td>
      <td>300.000000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>NaN</td>
      <td>50.000000</td>
      <td>46.000000</td>
      <td>78.000000</td>
      <td>30.570000</td>
      <td>10.000000</td>
      <td>16.000000</td>
      <td>NaN</td>
      <td>8.000000</td>
      <td>NaN</td>
      <td>345.000000</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.DewPoint.describe()
```




    count    31.000000
    mean     17.838710
    std      11.378626
    min      -3.000000
    25%      10.000000
    50%      18.000000
    75%      23.000000
    max      46.000000
    Name: DewPoint, dtype: float64




```python
df.info()
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 31 entries, 0 to 30
    Data columns (total 11 columns):
     #   Column                Non-Null Count  Dtype  
    ---  ------                --------------  -----  
     0   EST                   31 non-null     object 
     1   Temperature           31 non-null     int64  
     2   DewPoint              31 non-null     int64  
     3   Humidity              31 non-null     int64  
     4   Sea Level PressureIn  31 non-null     float64
     5   VisibilityMiles       31 non-null     int64  
     6   WindSpeedMPH          28 non-null     float64
     7   PrecipitationIn       31 non-null     object 
     8   CloudCover            31 non-null     int64  
     9   Events                9 non-null      object 
     10  WindDirDegrees        31 non-null     int64  
    dtypes: float64(2), int64(6), object(3)
    memory usage: 2.8+ KB
    


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
      <th>EST</th>
      <th>Temperature</th>
      <th>DewPoint</th>
      <th>Humidity</th>
      <th>Sea Level PressureIn</th>
      <th>VisibilityMiles</th>
      <th>WindSpeedMPH</th>
      <th>PrecipitationIn</th>
      <th>CloudCover</th>
      <th>Events</th>
      <th>WindDirDegrees</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1/1/2016</td>
      <td>38</td>
      <td>23</td>
      <td>52</td>
      <td>30.03</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>5</td>
      <td>NaN</td>
      <td>281</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1/2/2016</td>
      <td>36</td>
      <td>18</td>
      <td>46</td>
      <td>30.02</td>
      <td>10</td>
      <td>7.0</td>
      <td>0</td>
      <td>3</td>
      <td>NaN</td>
      <td>275</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1/3/2016</td>
      <td>40</td>
      <td>21</td>
      <td>47</td>
      <td>29.86</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>277</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1/4/2016</td>
      <td>25</td>
      <td>9</td>
      <td>44</td>
      <td>30.05</td>
      <td>10</td>
      <td>9.0</td>
      <td>0</td>
      <td>3</td>
      <td>NaN</td>
      <td>345</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1/5/2016</td>
      <td>20</td>
      <td>-3</td>
      <td>41</td>
      <td>30.57</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>333</td>
    </tr>
    <tr>
      <th>5</th>
      <td>1/6/2016</td>
      <td>33</td>
      <td>4</td>
      <td>35</td>
      <td>30.50</td>
      <td>10</td>
      <td>4.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>259</td>
    </tr>
    <tr>
      <th>6</th>
      <td>1/7/2016</td>
      <td>39</td>
      <td>11</td>
      <td>33</td>
      <td>30.28</td>
      <td>10</td>
      <td>2.0</td>
      <td>0</td>
      <td>3</td>
      <td>NaN</td>
      <td>293</td>
    </tr>
    <tr>
      <th>7</th>
      <td>1/8/2016</td>
      <td>39</td>
      <td>29</td>
      <td>64</td>
      <td>30.20</td>
      <td>10</td>
      <td>4.0</td>
      <td>0</td>
      <td>8</td>
      <td>NaN</td>
      <td>79</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1/9/2016</td>
      <td>44</td>
      <td>38</td>
      <td>77</td>
      <td>30.16</td>
      <td>9</td>
      <td>8.0</td>
      <td>T</td>
      <td>8</td>
      <td>Rain</td>
      <td>76</td>
    </tr>
    <tr>
      <th>9</th>
      <td>1/10/2016</td>
      <td>50</td>
      <td>46</td>
      <td>71</td>
      <td>29.59</td>
      <td>4</td>
      <td>NaN</td>
      <td>1.8</td>
      <td>7</td>
      <td>Rain</td>
      <td>109</td>
    </tr>
    <tr>
      <th>10</th>
      <td>1/11/2016</td>
      <td>33</td>
      <td>8</td>
      <td>37</td>
      <td>29.92</td>
      <td>10</td>
      <td>NaN</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>289</td>
    </tr>
    <tr>
      <th>11</th>
      <td>1/12/2016</td>
      <td>35</td>
      <td>15</td>
      <td>53</td>
      <td>29.85</td>
      <td>10</td>
      <td>6.0</td>
      <td>T</td>
      <td>4</td>
      <td>NaN</td>
      <td>235</td>
    </tr>
    <tr>
      <th>12</th>
      <td>1/13/2016</td>
      <td>26</td>
      <td>4</td>
      <td>42</td>
      <td>29.94</td>
      <td>10</td>
      <td>10.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>284</td>
    </tr>
    <tr>
      <th>13</th>
      <td>1/14/2016</td>
      <td>30</td>
      <td>12</td>
      <td>47</td>
      <td>29.95</td>
      <td>10</td>
      <td>5.0</td>
      <td>T</td>
      <td>7</td>
      <td>NaN</td>
      <td>266</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1/15/2016</td>
      <td>43</td>
      <td>31</td>
      <td>62</td>
      <td>29.82</td>
      <td>9</td>
      <td>5.0</td>
      <td>T</td>
      <td>2</td>
      <td>NaN</td>
      <td>101</td>
    </tr>
    <tr>
      <th>15</th>
      <td>1/16/2016</td>
      <td>47</td>
      <td>37</td>
      <td>70</td>
      <td>29.52</td>
      <td>8</td>
      <td>7.0</td>
      <td>0.24</td>
      <td>7</td>
      <td>Rain</td>
      <td>340</td>
    </tr>
    <tr>
      <th>16</th>
      <td>1/17/2016</td>
      <td>36</td>
      <td>23</td>
      <td>66</td>
      <td>29.78</td>
      <td>8</td>
      <td>6.0</td>
      <td>0.05</td>
      <td>6</td>
      <td>Fog-Snow</td>
      <td>345</td>
    </tr>
    <tr>
      <th>17</th>
      <td>1/18/2016</td>
      <td>25</td>
      <td>6</td>
      <td>53</td>
      <td>29.83</td>
      <td>9</td>
      <td>12.0</td>
      <td>T</td>
      <td>2</td>
      <td>Snow</td>
      <td>293</td>
    </tr>
    <tr>
      <th>18</th>
      <td>1/19/2016</td>
      <td>22</td>
      <td>3</td>
      <td>42</td>
      <td>30.03</td>
      <td>10</td>
      <td>11.0</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>293</td>
    </tr>
    <tr>
      <th>19</th>
      <td>1/20/2016</td>
      <td>32</td>
      <td>15</td>
      <td>49</td>
      <td>30.13</td>
      <td>10</td>
      <td>6.0</td>
      <td>0</td>
      <td>2</td>
      <td>NaN</td>
      <td>302</td>
    </tr>
    <tr>
      <th>20</th>
      <td>1/21/2016</td>
      <td>31</td>
      <td>11</td>
      <td>45</td>
      <td>30.15</td>
      <td>10</td>
      <td>6.0</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>312</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1/22/2016</td>
      <td>26</td>
      <td>6</td>
      <td>41</td>
      <td>30.21</td>
      <td>9</td>
      <td>NaN</td>
      <td>0.01</td>
      <td>3</td>
      <td>Snow</td>
      <td>34</td>
    </tr>
    <tr>
      <th>22</th>
      <td>1/23/2016</td>
      <td>26</td>
      <td>21</td>
      <td>78</td>
      <td>29.77</td>
      <td>1</td>
      <td>16.0</td>
      <td>2.31</td>
      <td>8</td>
      <td>Fog-Snow</td>
      <td>42</td>
    </tr>
    <tr>
      <th>23</th>
      <td>1/24/2016</td>
      <td>28</td>
      <td>11</td>
      <td>53</td>
      <td>29.92</td>
      <td>8</td>
      <td>6.0</td>
      <td>T</td>
      <td>3</td>
      <td>Snow</td>
      <td>327</td>
    </tr>
    <tr>
      <th>24</th>
      <td>1/25/2016</td>
      <td>34</td>
      <td>18</td>
      <td>54</td>
      <td>30.25</td>
      <td>10</td>
      <td>3.0</td>
      <td>0</td>
      <td>2</td>
      <td>NaN</td>
      <td>286</td>
    </tr>
    <tr>
      <th>25</th>
      <td>1/26/2016</td>
      <td>43</td>
      <td>29</td>
      <td>56</td>
      <td>30.03</td>
      <td>10</td>
      <td>7.0</td>
      <td>0</td>
      <td>2</td>
      <td>NaN</td>
      <td>244</td>
    </tr>
    <tr>
      <th>26</th>
      <td>1/27/2016</td>
      <td>41</td>
      <td>22</td>
      <td>45</td>
      <td>30.03</td>
      <td>10</td>
      <td>7.0</td>
      <td>T</td>
      <td>3</td>
      <td>Rain</td>
      <td>311</td>
    </tr>
    <tr>
      <th>27</th>
      <td>1/28/2016</td>
      <td>37</td>
      <td>20</td>
      <td>51</td>
      <td>29.90</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>1</td>
      <td>NaN</td>
      <td>234</td>
    </tr>
    <tr>
      <th>28</th>
      <td>1/29/2016</td>
      <td>36</td>
      <td>21</td>
      <td>50</td>
      <td>29.58</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>4</td>
      <td>NaN</td>
      <td>298</td>
    </tr>
    <tr>
      <th>29</th>
      <td>1/30/2016</td>
      <td>34</td>
      <td>16</td>
      <td>46</td>
      <td>30.01</td>
      <td>10</td>
      <td>7.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>257</td>
    </tr>
    <tr>
      <th>30</th>
      <td>1/31/2016</td>
      <td>46</td>
      <td>28</td>
      <td>52</td>
      <td>29.90</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>0</td>
      <td>NaN</td>
      <td>241</td>
    </tr>
  </tbody>
</table>
</div>




```python
newdf = df.fillna(0)
newdf
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
      <th>EST</th>
      <th>Temperature</th>
      <th>DewPoint</th>
      <th>Humidity</th>
      <th>Sea Level PressureIn</th>
      <th>VisibilityMiles</th>
      <th>WindSpeedMPH</th>
      <th>PrecipitationIn</th>
      <th>CloudCover</th>
      <th>Events</th>
      <th>WindDirDegrees</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1/1/2016</td>
      <td>38</td>
      <td>23</td>
      <td>52</td>
      <td>30.03</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>5</td>
      <td>0</td>
      <td>281</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1/2/2016</td>
      <td>36</td>
      <td>18</td>
      <td>46</td>
      <td>30.02</td>
      <td>10</td>
      <td>7.0</td>
      <td>0</td>
      <td>3</td>
      <td>0</td>
      <td>275</td>
    </tr>
    <tr>
      <th>2</th>
      <td>1/3/2016</td>
      <td>40</td>
      <td>21</td>
      <td>47</td>
      <td>29.86</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>277</td>
    </tr>
    <tr>
      <th>3</th>
      <td>1/4/2016</td>
      <td>25</td>
      <td>9</td>
      <td>44</td>
      <td>30.05</td>
      <td>10</td>
      <td>9.0</td>
      <td>0</td>
      <td>3</td>
      <td>0</td>
      <td>345</td>
    </tr>
    <tr>
      <th>4</th>
      <td>1/5/2016</td>
      <td>20</td>
      <td>-3</td>
      <td>41</td>
      <td>30.57</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>333</td>
    </tr>
    <tr>
      <th>5</th>
      <td>1/6/2016</td>
      <td>33</td>
      <td>4</td>
      <td>35</td>
      <td>30.50</td>
      <td>10</td>
      <td>4.0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>259</td>
    </tr>
    <tr>
      <th>6</th>
      <td>1/7/2016</td>
      <td>39</td>
      <td>11</td>
      <td>33</td>
      <td>30.28</td>
      <td>10</td>
      <td>2.0</td>
      <td>0</td>
      <td>3</td>
      <td>0</td>
      <td>293</td>
    </tr>
    <tr>
      <th>7</th>
      <td>1/8/2016</td>
      <td>39</td>
      <td>29</td>
      <td>64</td>
      <td>30.20</td>
      <td>10</td>
      <td>4.0</td>
      <td>0</td>
      <td>8</td>
      <td>0</td>
      <td>79</td>
    </tr>
    <tr>
      <th>8</th>
      <td>1/9/2016</td>
      <td>44</td>
      <td>38</td>
      <td>77</td>
      <td>30.16</td>
      <td>9</td>
      <td>8.0</td>
      <td>T</td>
      <td>8</td>
      <td>Rain</td>
      <td>76</td>
    </tr>
    <tr>
      <th>9</th>
      <td>1/10/2016</td>
      <td>50</td>
      <td>46</td>
      <td>71</td>
      <td>29.59</td>
      <td>4</td>
      <td>0.0</td>
      <td>1.8</td>
      <td>7</td>
      <td>Rain</td>
      <td>109</td>
    </tr>
    <tr>
      <th>10</th>
      <td>1/11/2016</td>
      <td>33</td>
      <td>8</td>
      <td>37</td>
      <td>29.92</td>
      <td>10</td>
      <td>0.0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>289</td>
    </tr>
    <tr>
      <th>11</th>
      <td>1/12/2016</td>
      <td>35</td>
      <td>15</td>
      <td>53</td>
      <td>29.85</td>
      <td>10</td>
      <td>6.0</td>
      <td>T</td>
      <td>4</td>
      <td>0</td>
      <td>235</td>
    </tr>
    <tr>
      <th>12</th>
      <td>1/13/2016</td>
      <td>26</td>
      <td>4</td>
      <td>42</td>
      <td>29.94</td>
      <td>10</td>
      <td>10.0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>284</td>
    </tr>
    <tr>
      <th>13</th>
      <td>1/14/2016</td>
      <td>30</td>
      <td>12</td>
      <td>47</td>
      <td>29.95</td>
      <td>10</td>
      <td>5.0</td>
      <td>T</td>
      <td>7</td>
      <td>0</td>
      <td>266</td>
    </tr>
    <tr>
      <th>14</th>
      <td>1/15/2016</td>
      <td>43</td>
      <td>31</td>
      <td>62</td>
      <td>29.82</td>
      <td>9</td>
      <td>5.0</td>
      <td>T</td>
      <td>2</td>
      <td>0</td>
      <td>101</td>
    </tr>
    <tr>
      <th>15</th>
      <td>1/16/2016</td>
      <td>47</td>
      <td>37</td>
      <td>70</td>
      <td>29.52</td>
      <td>8</td>
      <td>7.0</td>
      <td>0.24</td>
      <td>7</td>
      <td>Rain</td>
      <td>340</td>
    </tr>
    <tr>
      <th>16</th>
      <td>1/17/2016</td>
      <td>36</td>
      <td>23</td>
      <td>66</td>
      <td>29.78</td>
      <td>8</td>
      <td>6.0</td>
      <td>0.05</td>
      <td>6</td>
      <td>Fog-Snow</td>
      <td>345</td>
    </tr>
    <tr>
      <th>17</th>
      <td>1/18/2016</td>
      <td>25</td>
      <td>6</td>
      <td>53</td>
      <td>29.83</td>
      <td>9</td>
      <td>12.0</td>
      <td>T</td>
      <td>2</td>
      <td>Snow</td>
      <td>293</td>
    </tr>
    <tr>
      <th>18</th>
      <td>1/19/2016</td>
      <td>22</td>
      <td>3</td>
      <td>42</td>
      <td>30.03</td>
      <td>10</td>
      <td>11.0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>293</td>
    </tr>
    <tr>
      <th>19</th>
      <td>1/20/2016</td>
      <td>32</td>
      <td>15</td>
      <td>49</td>
      <td>30.13</td>
      <td>10</td>
      <td>6.0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>302</td>
    </tr>
    <tr>
      <th>20</th>
      <td>1/21/2016</td>
      <td>31</td>
      <td>11</td>
      <td>45</td>
      <td>30.15</td>
      <td>10</td>
      <td>6.0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>312</td>
    </tr>
    <tr>
      <th>21</th>
      <td>1/22/2016</td>
      <td>26</td>
      <td>6</td>
      <td>41</td>
      <td>30.21</td>
      <td>9</td>
      <td>0.0</td>
      <td>0.01</td>
      <td>3</td>
      <td>Snow</td>
      <td>34</td>
    </tr>
    <tr>
      <th>22</th>
      <td>1/23/2016</td>
      <td>26</td>
      <td>21</td>
      <td>78</td>
      <td>29.77</td>
      <td>1</td>
      <td>16.0</td>
      <td>2.31</td>
      <td>8</td>
      <td>Fog-Snow</td>
      <td>42</td>
    </tr>
    <tr>
      <th>23</th>
      <td>1/24/2016</td>
      <td>28</td>
      <td>11</td>
      <td>53</td>
      <td>29.92</td>
      <td>8</td>
      <td>6.0</td>
      <td>T</td>
      <td>3</td>
      <td>Snow</td>
      <td>327</td>
    </tr>
    <tr>
      <th>24</th>
      <td>1/25/2016</td>
      <td>34</td>
      <td>18</td>
      <td>54</td>
      <td>30.25</td>
      <td>10</td>
      <td>3.0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>286</td>
    </tr>
    <tr>
      <th>25</th>
      <td>1/26/2016</td>
      <td>43</td>
      <td>29</td>
      <td>56</td>
      <td>30.03</td>
      <td>10</td>
      <td>7.0</td>
      <td>0</td>
      <td>2</td>
      <td>0</td>
      <td>244</td>
    </tr>
    <tr>
      <th>26</th>
      <td>1/27/2016</td>
      <td>41</td>
      <td>22</td>
      <td>45</td>
      <td>30.03</td>
      <td>10</td>
      <td>7.0</td>
      <td>T</td>
      <td>3</td>
      <td>Rain</td>
      <td>311</td>
    </tr>
    <tr>
      <th>27</th>
      <td>1/28/2016</td>
      <td>37</td>
      <td>20</td>
      <td>51</td>
      <td>29.90</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>1</td>
      <td>0</td>
      <td>234</td>
    </tr>
    <tr>
      <th>28</th>
      <td>1/29/2016</td>
      <td>36</td>
      <td>21</td>
      <td>50</td>
      <td>29.58</td>
      <td>10</td>
      <td>8.0</td>
      <td>0</td>
      <td>4</td>
      <td>0</td>
      <td>298</td>
    </tr>
    <tr>
      <th>29</th>
      <td>1/30/2016</td>
      <td>34</td>
      <td>16</td>
      <td>46</td>
      <td>30.01</td>
      <td>10</td>
      <td>7.0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>257</td>
    </tr>
    <tr>
      <th>30</th>
      <td>1/31/2016</td>
      <td>46</td>
      <td>28</td>
      <td>52</td>
      <td>29.90</td>
      <td>10</td>
      <td>5.0</td>
      <td>0</td>
      <td>0</td>
      <td>0</td>
      <td>241</td>
    </tr>
  </tbody>
</table>
</div>




```python
import io
import requests
url = "https://raw.githubusercontent.com/cs109/2014_data/master/countries.csv"
s = requests.get(url).content
data = pd.read_csv(io.StringIO(s.decode('utf-8')))
data
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
      <th>Country</th>
      <th>Region</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Algeria</td>
      <td>AFRICA</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Angola</td>
      <td>AFRICA</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Benin</td>
      <td>AFRICA</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Botswana</td>
      <td>AFRICA</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Burkina</td>
      <td>AFRICA</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>189</th>
      <td>Paraguay</td>
      <td>SOUTH AMERICA</td>
    </tr>
    <tr>
      <th>190</th>
      <td>Peru</td>
      <td>SOUTH AMERICA</td>
    </tr>
    <tr>
      <th>191</th>
      <td>Suriname</td>
      <td>SOUTH AMERICA</td>
    </tr>
    <tr>
      <th>192</th>
      <td>Uruguay</td>
      <td>SOUTH AMERICA</td>
    </tr>
    <tr>
      <th>193</th>
      <td>Venezuela</td>
      <td>SOUTH AMERICA</td>
    </tr>
  </tbody>
</table>
<p>194 rows × 2 columns</p>
</div>



### the end 


```python

```
