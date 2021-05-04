
 # Gathering Data


```python
# Import libraries
```

## 1- Gather data from 'twitter-archive-enhanced.csv':

#read the csv file

#check the imported file

## 2- Gather data from "image_predictions.tsv":

# save HTML to file

#check the file aquired


```python
#create a folder for data
```


```python
#Write data to a file in our folder
```


```python
#Read the file, using the tab sepration
```

#check the file aquired

## 3- Gather data from "Twitter API":


```python
#import Twitter API json file (line by line)
```

#Check imported data

# convert data to dataframe


```python
# save twettr_api data as csv file
```


```python
# save twettr_df_image_predictions as csv file
```


```python
# save df_twetter_archive.csv as csv file
```

# 2- Assessing:

## 1-Assessing df_image_predictions Data

# import the data file

# Show the first 10 rows for visual assessment

Assesssment findings:
Q1- Column Header is undescribtive: img_num	p1, p1_conf, p1_dog, p2, p2_conf, p2_dog, p3, p3_conf, p3_dog.
T1- img_num column contain the data as the same for the jpg_url column.
T2- the first column to be removed as it the same as index.


```python
# Show the last 10 rows for visual assessment
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
      <th>Unnamed: 0</th>
      <th>tweet_id</th>
      <th>jpg_url</th>
      <th>img_num</th>
      <th>p1</th>
      <th>p1_conf</th>
      <th>p1_dog</th>
      <th>p2</th>
      <th>p2_conf</th>
      <th>p2_dog</th>
      <th>p3</th>
      <th>p3_conf</th>
      <th>p3_dog</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2065</th>
      <td>2065</td>
      <td>890240255349198849</td>
      <td>https://pbs.twimg.com/media/DFrEyVuW0AAO3t9.jpg</td>
      <td>1</td>
      <td>Pembroke</td>
      <td>0.511319</td>
      <td>True</td>
      <td>Cardigan</td>
      <td>0.451038</td>
      <td>True</td>
      <td>Chihuahua</td>
      <td>0.029248</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2066</th>
      <td>2066</td>
      <td>890609185150312448</td>
      <td>https://pbs.twimg.com/media/DFwUU__XcAEpyXI.jpg</td>
      <td>1</td>
      <td>Irish_terrier</td>
      <td>0.487574</td>
      <td>True</td>
      <td>Irish_setter</td>
      <td>0.193054</td>
      <td>True</td>
      <td>Chesapeake_Bay_retriever</td>
      <td>0.118184</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2067</th>
      <td>2067</td>
      <td>890729181411237888</td>
      <td>https://pbs.twimg.com/media/DFyBahAVwAAhUTd.jpg</td>
      <td>2</td>
      <td>Pomeranian</td>
      <td>0.566142</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.178406</td>
      <td>True</td>
      <td>Pembroke</td>
      <td>0.076507</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2068</th>
      <td>2068</td>
      <td>890971913173991426</td>
      <td>https://pbs.twimg.com/media/DF1eOmZXUAALUcq.jpg</td>
      <td>1</td>
      <td>Appenzeller</td>
      <td>0.341703</td>
      <td>True</td>
      <td>Border_collie</td>
      <td>0.199287</td>
      <td>True</td>
      <td>ice_lolly</td>
      <td>0.193548</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2069</th>
      <td>2069</td>
      <td>891087950875897856</td>
      <td>https://pbs.twimg.com/media/DF3HwyEWsAABqE6.jpg</td>
      <td>1</td>
      <td>Chesapeake_Bay_retriever</td>
      <td>0.425595</td>
      <td>True</td>
      <td>Irish_terrier</td>
      <td>0.116317</td>
      <td>True</td>
      <td>Indian_elephant</td>
      <td>0.076902</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2070</th>
      <td>2070</td>
      <td>891327558926688256</td>
      <td>https://pbs.twimg.com/media/DF6hr6BUMAAzZgT.jpg</td>
      <td>2</td>
      <td>basset</td>
      <td>0.555712</td>
      <td>True</td>
      <td>English_springer</td>
      <td>0.225770</td>
      <td>True</td>
      <td>German_short-haired_pointer</td>
      <td>0.175219</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2071</th>
      <td>2071</td>
      <td>891689557279858688</td>
      <td>https://pbs.twimg.com/media/DF_q7IAWsAEuuN8.jpg</td>
      <td>1</td>
      <td>paper_towel</td>
      <td>0.170278</td>
      <td>False</td>
      <td>Labrador_retriever</td>
      <td>0.168086</td>
      <td>True</td>
      <td>spatula</td>
      <td>0.040836</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2072</th>
      <td>2072</td>
      <td>891815181378084864</td>
      <td>https://pbs.twimg.com/media/DGBdLU1WsAANxJ9.jpg</td>
      <td>1</td>
      <td>Chihuahua</td>
      <td>0.716012</td>
      <td>True</td>
      <td>malamute</td>
      <td>0.078253</td>
      <td>True</td>
      <td>kelpie</td>
      <td>0.031379</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2073</th>
      <td>2073</td>
      <td>892177421306343426</td>
      <td>https://pbs.twimg.com/media/DGGmoV4XsAAUL6n.jpg</td>
      <td>1</td>
      <td>Chihuahua</td>
      <td>0.323581</td>
      <td>True</td>
      <td>Pekinese</td>
      <td>0.090647</td>
      <td>True</td>
      <td>papillon</td>
      <td>0.068957</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2074</th>
      <td>2074</td>
      <td>892420643555336193</td>
      <td>https://pbs.twimg.com/media/DGKD1-bXoAAIAUK.jpg</td>
      <td>1</td>
      <td>orange</td>
      <td>0.097049</td>
      <td>False</td>
      <td>bagel</td>
      <td>0.085851</td>
      <td>False</td>
      <td>banana</td>
      <td>0.076110</td>
      <td>False</td>
    </tr>
  </tbody>
</table>
</div>




```python

```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 2075 entries, 0 to 2074
    Data columns (total 13 columns):
    Unnamed: 0    2075 non-null int64
    tweet_id      2075 non-null int64
    jpg_url       2075 non-null object
    img_num       2075 non-null int64
    p1            2075 non-null object
    p1_conf       2075 non-null float64
    p1_dog        2075 non-null bool
    p2            2075 non-null object
    p2_conf       2075 non-null float64
    p2_dog        2075 non-null bool
    p3            2075 non-null object
    p3_conf       2075 non-null float64
    p3_dog        2075 non-null bool
    dtypes: bool(3), float64(3), int64(3), object(4)
    memory usage: 168.3+ KB



```python
# Show the random sample of 10 rows for visual assessment
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
      <th>Unnamed: 0</th>
      <th>tweet_id</th>
      <th>jpg_url</th>
      <th>img_num</th>
      <th>p1</th>
      <th>p1_conf</th>
      <th>p1_dog</th>
      <th>p2</th>
      <th>p2_conf</th>
      <th>p2_dog</th>
      <th>p3</th>
      <th>p3_conf</th>
      <th>p3_dog</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>503</th>
      <td>503</td>
      <td>675878199931371520</td>
      <td>https://pbs.twimg.com/media/CWEzo19WoAEiOCj.jpg</td>
      <td>1</td>
      <td>wood_rabbit</td>
      <td>0.785756</td>
      <td>False</td>
      <td>hare</td>
      <td>0.118181</td>
      <td>False</td>
      <td>Cardigan</td>
      <td>0.043627</td>
      <td>True</td>
    </tr>
    <tr>
      <th>447</th>
      <td>447</td>
      <td>674670581682434048</td>
      <td>https://pbs.twimg.com/media/CVzpUGUWUAAo7Vn.jpg</td>
      <td>1</td>
      <td>malamute</td>
      <td>0.180079</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.178033</td>
      <td>True</td>
      <td>Siberian_husky</td>
      <td>0.077966</td>
      <td>True</td>
    </tr>
    <tr>
      <th>1561</th>
      <td>1561</td>
      <td>793286476301799424</td>
      <td>https://pbs.twimg.com/media/CwJR1okWIAA6XMp.jpg</td>
      <td>1</td>
      <td>Afghan_hound</td>
      <td>0.274637</td>
      <td>True</td>
      <td>borzoi</td>
      <td>0.142204</td>
      <td>True</td>
      <td>doormat</td>
      <td>0.109677</td>
      <td>False</td>
    </tr>
    <tr>
      <th>284</th>
      <td>284</td>
      <td>671141549288370177</td>
      <td>https://pbs.twimg.com/media/CVBfrU9WUAApDeV.jpg</td>
      <td>1</td>
      <td>guinea_pig</td>
      <td>0.387728</td>
      <td>False</td>
      <td>wood_rabbit</td>
      <td>0.171681</td>
      <td>False</td>
      <td>borzoi</td>
      <td>0.075358</td>
      <td>True</td>
    </tr>
    <tr>
      <th>1002</th>
      <td>1002</td>
      <td>708810915978854401</td>
      <td>https://pbs.twimg.com/media/CdYzwuYUIAAHPkB.jpg</td>
      <td>2</td>
      <td>golden_retriever</td>
      <td>0.976139</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.016301</td>
      <td>True</td>
      <td>Norfolk_terrier</td>
      <td>0.001871</td>
      <td>True</td>
    </tr>
    <tr>
      <th>881</th>
      <td>881</td>
      <td>698703483621523456</td>
      <td>https://pbs.twimg.com/media/CbJLG0HWwAAV-ug.jpg</td>
      <td>1</td>
      <td>Brittany_spaniel</td>
      <td>0.931963</td>
      <td>True</td>
      <td>Welsh_springer_spaniel</td>
      <td>0.030695</td>
      <td>True</td>
      <td>beagle</td>
      <td>0.012896</td>
      <td>True</td>
    </tr>
    <tr>
      <th>1419</th>
      <td>1419</td>
      <td>771500966810099713</td>
      <td>https://pbs.twimg.com/media/CrTsCPHWYAANdzC.jpg</td>
      <td>1</td>
      <td>Labrador_retriever</td>
      <td>0.833952</td>
      <td>True</td>
      <td>golden_retriever</td>
      <td>0.103223</td>
      <td>True</td>
      <td>soccer_ball</td>
      <td>0.012094</td>
      <td>False</td>
    </tr>
    <tr>
      <th>1027</th>
      <td>1027</td>
      <td>710844581445812225</td>
      <td>https://pbs.twimg.com/media/Cd1tYGmXIAAoW5b.jpg</td>
      <td>1</td>
      <td>dingo</td>
      <td>0.536593</td>
      <td>False</td>
      <td>Pembroke</td>
      <td>0.200407</td>
      <td>True</td>
      <td>basenji</td>
      <td>0.060735</td>
      <td>True</td>
    </tr>
    <tr>
      <th>860</th>
      <td>860</td>
      <td>696900204696625153</td>
      <td>https://pbs.twimg.com/media/CavjCdJW0AIB5Oz.jpg</td>
      <td>1</td>
      <td>Chihuahua</td>
      <td>0.297735</td>
      <td>True</td>
      <td>Pembroke</td>
      <td>0.266953</td>
      <td>True</td>
      <td>basenji</td>
      <td>0.136814</td>
      <td>True</td>
    </tr>
    <tr>
      <th>421</th>
      <td>421</td>
      <td>674045139690631169</td>
      <td>https://pbs.twimg.com/media/CVqwedgXIAEAT6A.jpg</td>
      <td>1</td>
      <td>robin</td>
      <td>0.369661</td>
      <td>False</td>
      <td>rhinoceros_beetle</td>
      <td>0.110607</td>
      <td>False</td>
      <td>European_fire_salamander</td>
      <td>0.043178</td>
      <td>False</td>
    </tr>
  </tbody>
</table>
</div>




```python
# check the count of values in p1 column
```




    golden_retriever             150
    Labrador_retriever           100
    Pembroke                      89
    Chihuahua                     83
    pug                           57
    chow                          44
    Samoyed                       43
    toy_poodle                    39
    Pomeranian                    38
    cocker_spaniel                30
    malamute                      30
    French_bulldog                26
    Chesapeake_Bay_retriever      23
    miniature_pinscher            23
    seat_belt                     22
    Siberian_husky                20
    German_shepherd               20
    Staffordshire_bullterrier     20
    Cardigan                      19
    web_site                      19
    teddy                         18
    Eskimo_dog                    18
    Maltese_dog                   18
    beagle                        18
    Shetland_sheepdog             18
    Lakeland_terrier              17
    Rottweiler                    17
    Shih-Tzu                      17
    kuvasz                        16
    Italian_greyhound             16
                                ... 
    binoculars                     1
    teapot                         1
    bow                            1
    boathouse                      1
    cougar                         1
    pillow                         1
    panpipe                        1
    hotdog                         1
    padlock                        1
    peacock                        1
    bee_eater                      1
    jersey                         1
    mortarboard                    1
    African_crocodile              1
    coffee_mug                     1
    bannister                      1
    lion                           1
    carousel                       1
    orange                         1
    ping-pong_ball                 1
    guenon                         1
    clog                           1
    grey_fox                       1
    piggy_bank                     1
    microphone                     1
    park_bench                     1
    African_hunting_dog            1
    wooden_spoon                   1
    standard_schnauzer             1
    leaf_beetle                    1
    Name: p1, Length: 378, dtype: int64




```python
# check the count of values in p2 column
```




    Labrador_retriever                104
    golden_retriever                   92
    Cardigan                           73
    Chihuahua                          44
    Pomeranian                         42
    Chesapeake_Bay_retriever           41
    French_bulldog                     41
    toy_poodle                         37
    cocker_spaniel                     34
    miniature_poodle                   33
    Siberian_husky                     33
    beagle                             28
    collie                             27
    Pembroke                           27
    Eskimo_dog                         27
    kuvasz                             26
    Italian_greyhound                  22
    Pekinese                           21
    American_Staffordshire_terrier     21
    malinois                           20
    miniature_pinscher                 20
    toy_terrier                        20
    Samoyed                            20
    chow                               20
    Norwegian_elkhound                 19
    Boston_bull                        19
    Staffordshire_bullterrier          18
    pug                                17
    Irish_terrier                      17
    kelpie                             16
                                     ... 
    toucan                              1
    barracouta                          1
    coral_reef                          1
    desk                                1
    bucket                              1
    web_site                            1
    shower_curtain                      1
    rain_barrel                         1
    cougar                              1
    breastplate                         1
    turnstile                           1
    laptop                              1
    paper_towel                         1
    cowboy_hat                          1
    waffle_iron                         1
    standard_schnauzer                  1
    grey_whale                          1
    snorkel                             1
    dining_table                        1
    sock                                1
    cannon                              1
    cornet                              1
    Bernese_mountain_dog                1
    maillot                             1
    wombat                              1
    moped                               1
    torch                               1
    streetcar                           1
    breakwater                          1
    European_gallinule                  1
    Name: p2, Length: 405, dtype: int64




```python
# check the count of values in p3 column
```




    Labrador_retriever                79
    Chihuahua                         58
    golden_retriever                  48
    Eskimo_dog                        38
    kelpie                            35
    kuvasz                            34
    chow                              32
    Staffordshire_bullterrier         32
    cocker_spaniel                    31
    beagle                            31
    Pomeranian                        29
    Pekinese                          29
    toy_poodle                        29
    Chesapeake_Bay_retriever          27
    Pembroke                          27
    Great_Pyrenees                    27
    malamute                          26
    French_bulldog                    26
    American_Staffordshire_terrier    24
    pug                               23
    Cardigan                          23
    basenji                           21
    bull_mastiff                      20
    toy_terrier                       20
    Siberian_husky                    19
    Boston_bull                       17
    Shetland_sheepdog                 17
    Lakeland_terrier                  16
    doormat                           16
    boxer                             16
                                      ..
    rhinoceros_beetle                  1
    coffeepot                          1
    assault_rifle                      1
    zebra                              1
    jaguar                             1
    chime                              1
    ballplayer                         1
    panpipe                            1
    great_grey_owl                     1
    croquet_ball                       1
    pool_table                         1
    African_chameleon                  1
    meerkat                            1
    park_bench                         1
    jeep                               1
    coral_reef                         1
    pajama                             1
    kimono                             1
    rifle                              1
    triceratops                        1
    desktop_computer                   1
    hammerhead                         1
    wombat                             1
    moped                              1
    spatula                            1
    cheetah                            1
    wok                                1
    bib                                1
    parachute                          1
    sunglass                           1
    Name: p3, Length: 408, dtype: int64



Assessment findings:
Q2- some of the dogs types are incorrect, such in p1 column: car_mirror in raw 371, snorkel in row 655, killer_whale in column 337, mousetrap in row 889


```python
# check the missing values
```




    Unnamed: 0    0
    tweet_id      0
    jpg_url       0
    img_num       0
    p1            0
    p1_conf       0
    p1_dog        0
    p2            0
    p2_conf       0
    p2_dog        0
    p3            0
    p3_conf       0
    p3_dog        0
    dtype: int64




```python
# check the sorted values in p1 column
```




    1561                      Afghan_hound
    1855                      Afghan_hound
    1458                      Afghan_hound
    1804                      Afghan_hound
    446                  African_crocodile
    1371                      African_grey
    289                African_hunting_dog
    1883                          Airedale
    678                           Airedale
    425                           Airedale
    1319                          Airedale
    1646                          Airedale
    378                           Airedale
    49                            Airedale
    603                           Airedale
    952                           Airedale
    189                           Airedale
    582                           Airedale
    1465                          Airedale
    139     American_Staffordshire_terrier
    269     American_Staffordshire_terrier
    1837    American_Staffordshire_terrier
    550     American_Staffordshire_terrier
    909     American_Staffordshire_terrier
    1582    American_Staffordshire_terrier
    758     American_Staffordshire_terrier
    767     American_Staffordshire_terrier
    1146    American_Staffordshire_terrier
    1586    American_Staffordshire_terrier
    1776    American_Staffordshire_terrier
                         ...              
    213                           web_site
    524                            whippet
    228                            whippet
    2059                           whippet
    661                            whippet
    1968                           whippet
    1306                           whippet
    1802                           whippet
    1047                           whippet
    987                            whippet
    1881                        white_wolf
    914                         white_wolf
    714                         white_wolf
    974                          wild_boar
    1134                      window_shade
    938                       window_shade
    237                       window_shade
    1557           wire-haired_fox_terrier
    1265           wire-haired_fox_terrier
    660                             wombat
    372                             wombat
    1197                            wombat
    395                             wombat
    743                        wood_rabbit
    503                        wood_rabbit
    253                        wood_rabbit
    1831                      wooden_spoon
    932                               wool
    246                               wool
    297                              zebra
    Name: p1, Length: 2075, dtype: object




```python
# check the sorted values in p2 column
```




    2024                      Afghan_hound
    1701                      Afghan_hound
    26                        Afghan_hound
    460                       Afghan_hound
    1290                      Afghan_hound
    53                 African_hunting_dog
    983                           Airedale
    340                           Airedale
    548                           Airedale
    1730                          Airedale
    1493                          Airedale
    716                           Airedale
    1950                          Airedale
    1632    American_Staffordshire_terrier
    1406    American_Staffordshire_terrier
    1849    American_Staffordshire_terrier
    1824    American_Staffordshire_terrier
    1218    American_Staffordshire_terrier
    1654    American_Staffordshire_terrier
    689     American_Staffordshire_terrier
    768     American_Staffordshire_terrier
    1903    American_Staffordshire_terrier
    1881    American_Staffordshire_terrier
    875     American_Staffordshire_terrier
    992     American_Staffordshire_terrier
    2039    American_Staffordshire_terrier
    1768    American_Staffordshire_terrier
    401     American_Staffordshire_terrier
    963     American_Staffordshire_terrier
    1785    American_Staffordshire_terrier
                         ...              
    1665                          web_site
    2010                           whippet
    505                            whippet
    867                            whippet
    1326                           whippet
    292                            whippet
    1255                           whippet
    1041                           whippet
    1427                           whippet
    1380                           whippet
    676                            whippet
    633                            whippet
    1673                           whippet
    776                            whippet
    1820                           whippet
    737                            whippet
    1829                        white_wolf
    1192                               wig
    311                                wig
    938                      window_screen
    580                      window_screen
    1774                     window_screen
    2012                     window_screen
    1093                      window_shade
    304            wire-haired_fox_terrier
    1261           wire-haired_fox_terrier
    1022           wire-haired_fox_terrier
    1007           wire-haired_fox_terrier
    929                             wombat
    284                        wood_rabbit
    Name: p2, Length: 2075, dtype: object




```python
# check the sorted values in p3 column
```




    134                       Afghan_hound
    850                       Afghan_hound
    590                       Afghan_hound
    355                       Afghan_hound
    107                  African_chameleon
    100                       African_grey
    766                           Airedale
    635                           Airedale
    1624                          Airedale
    583                           Airedale
    368                           Airedale
    1754                          Airedale
    344                           Airedale
    1554                          Airedale
    800                           Airedale
    657                           Airedale
    1435                          Airedale
    507     American_Staffordshire_terrier
    1338    American_Staffordshire_terrier
    1427    American_Staffordshire_terrier
    1643    American_Staffordshire_terrier
    624     American_Staffordshire_terrier
    549     American_Staffordshire_terrier
    562     American_Staffordshire_terrier
    873     American_Staffordshire_terrier
    1687    American_Staffordshire_terrier
    2011    American_Staffordshire_terrier
    1380    American_Staffordshire_terrier
    250     American_Staffordshire_terrier
    1968    American_Staffordshire_terrier
                         ...              
    118                         white_wolf
    812                         white_wolf
    1095                        white_wolf
    1346                        white_wolf
    1876                        white_wolf
    196                         white_wolf
    851                         white_wolf
    314                         white_wolf
    816                         white_wolf
    1222                        white_wolf
    51                                 wig
    233                                wig
    683                          wild_boar
    237                      window_screen
    205                               wing
    373            wire-haired_fox_terrier
    1660           wire-haired_fox_terrier
    1298           wire-haired_fox_terrier
    1229                               wok
    272                        wolf_spider
    1429                            wombat
    117                        wood_rabbit
    948                        wood_rabbit
    254                        wood_rabbit
    311                               wool
    457                               wool
    1329                              wool
    1956                             wreck
    453                              wreck
    597                              zebra
    Name: p3, Length: 2075, dtype: object




```python
# check the duplicated rows
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
      <th>Unnamed: 0</th>
      <th>tweet_id</th>
      <th>jpg_url</th>
      <th>img_num</th>
      <th>p1</th>
      <th>p1_conf</th>
      <th>p1_dog</th>
      <th>p2</th>
      <th>p2_conf</th>
      <th>p2_dog</th>
      <th>p3</th>
      <th>p3_conf</th>
      <th>p3_dog</th>
    </tr>
  </thead>
  <tbody>
  </tbody>
</table>
</div>



## 2- Assessing twitter_archive:


```python
# import the data file

# view the first 10 rows
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
      <th>Unnamed: 0</th>
      <th>tweet_id</th>
      <th>in_reply_to_status_id</th>
      <th>in_reply_to_user_id</th>
      <th>timestamp</th>
      <th>source</th>
      <th>text</th>
      <th>retweeted_status_id</th>
      <th>retweeted_status_user_id</th>
      <th>retweeted_status_timestamp</th>
      <th>expanded_urls</th>
      <th>rating_numerator</th>
      <th>rating_denominator</th>
      <th>name</th>
      <th>doggo</th>
      <th>floofer</th>
      <th>pupper</th>
      <th>puppo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>892420643555336193</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2017-08-01 16:23:56 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Phineas. He's a mystical boy. Only eve...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/892420643...</td>
      <td>13</td>
      <td>10</td>
      <td>Phineas</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>892177421306343426</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2017-08-01 00:17:27 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Tilly. She's just checking pup on you....</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/892177421...</td>
      <td>13</td>
      <td>10</td>
      <td>Tilly</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>891815181378084864</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2017-07-31 00:18:03 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Archie. He is a rare Norwegian Pouncin...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/891815181...</td>
      <td>12</td>
      <td>10</td>
      <td>Archie</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>891689557279858688</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2017-07-30 15:58:51 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Darla. She commenced a snooze mid meal...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/891689557...</td>
      <td>13</td>
      <td>10</td>
      <td>Darla</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>891327558926688256</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2017-07-29 16:00:24 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Franklin. He would like you to stop ca...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/891327558...</td>
      <td>12</td>
      <td>10</td>
      <td>Franklin</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>5</th>
      <td>5</td>
      <td>891087950875897856</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2017-07-29 00:08:17 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>Here we have a majestic great white breaching ...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/891087950...</td>
      <td>13</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>6</th>
      <td>6</td>
      <td>890971913173991426</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2017-07-28 16:27:12 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>Meet Jax. He enjoys ice cream so much he gets ...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://gofundme.com/ydvmve-surgery-for-jax,ht...</td>
      <td>13</td>
      <td>10</td>
      <td>Jax</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>7</th>
      <td>7</td>
      <td>890729181411237888</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2017-07-28 00:22:40 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>When you watch your owner call another dog a g...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/890729181...</td>
      <td>13</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>8</th>
      <td>8</td>
      <td>890609185150312448</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2017-07-27 16:25:51 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Zoey. She doesn't want to be one of th...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/890609185...</td>
      <td>13</td>
      <td>10</td>
      <td>Zoey</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>9</th>
      <td>9</td>
      <td>890240255349198849</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2017-07-26 15:59:51 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Cassie. She is a college pup. Studying...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/890240255...</td>
      <td>14</td>
      <td>10</td>
      <td>Cassie</td>
      <td>doggo</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
  </tbody>
</table>
</div>




```python
# view the last 10 rows
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
      <th>Unnamed: 0</th>
      <th>tweet_id</th>
      <th>in_reply_to_status_id</th>
      <th>in_reply_to_user_id</th>
      <th>timestamp</th>
      <th>source</th>
      <th>text</th>
      <th>retweeted_status_id</th>
      <th>retweeted_status_user_id</th>
      <th>retweeted_status_timestamp</th>
      <th>expanded_urls</th>
      <th>rating_numerator</th>
      <th>rating_denominator</th>
      <th>name</th>
      <th>doggo</th>
      <th>floofer</th>
      <th>pupper</th>
      <th>puppo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2346</th>
      <td>2346</td>
      <td>666058600524156928</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-11-16 01:01:59 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>Here is the Rand Paul of retrievers folks! He'...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/666058600...</td>
      <td>8</td>
      <td>10</td>
      <td>the</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>2347</th>
      <td>2347</td>
      <td>666057090499244032</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-11-16 00:55:59 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>My oh my. This is a rare blond Canadian terrie...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/666057090...</td>
      <td>9</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>2348</th>
      <td>2348</td>
      <td>666055525042405380</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-11-16 00:49:46 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>Here is a Siberian heavily armored polar bear ...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/666055525...</td>
      <td>10</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>2349</th>
      <td>2349</td>
      <td>666051853826850816</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-11-16 00:35:11 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is an odd dog. Hard on the outside but lo...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/666051853...</td>
      <td>2</td>
      <td>10</td>
      <td>an</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>2350</th>
      <td>2350</td>
      <td>666050758794694657</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-11-16 00:30:50 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is a truly beautiful English Wilson Staff...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/666050758...</td>
      <td>10</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>2351</th>
      <td>2351</td>
      <td>666049248165822465</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-11-16 00:24:50 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>Here we have a 1949 1st generation vulpix. Enj...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/666049248...</td>
      <td>5</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>2352</th>
      <td>2352</td>
      <td>666044226329800704</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-11-16 00:04:52 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is a purebred Piers Morgan. Loves to Netf...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/666044226...</td>
      <td>6</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>2353</th>
      <td>2353</td>
      <td>666033412701032449</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-11-15 23:21:54 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>Here is a very happy pup. Big fan of well-main...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/666033412...</td>
      <td>9</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>2354</th>
      <td>2354</td>
      <td>666029285002620928</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-11-15 23:05:30 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is a western brown Mitsubishi terrier. Up...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/666029285...</td>
      <td>7</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>2355</th>
      <td>2355</td>
      <td>666020888022790149</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-11-15 22:32:08 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>Here we have a Japanese Irish Setter. Lost eye...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/666020888...</td>
      <td>8</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
  </tbody>
</table>
</div>




```python
# view the random sample of 10 rows
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
      <th>Unnamed: 0</th>
      <th>tweet_id</th>
      <th>in_reply_to_status_id</th>
      <th>in_reply_to_user_id</th>
      <th>timestamp</th>
      <th>source</th>
      <th>text</th>
      <th>retweeted_status_id</th>
      <th>retweeted_status_user_id</th>
      <th>retweeted_status_timestamp</th>
      <th>expanded_urls</th>
      <th>rating_numerator</th>
      <th>rating_denominator</th>
      <th>name</th>
      <th>doggo</th>
      <th>floofer</th>
      <th>pupper</th>
      <th>puppo</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1544</th>
      <td>1544</td>
      <td>689517482558820352</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2016-01-19 18:39:13 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Carl. He just wants to make sure you'r...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/689517482...</td>
      <td>12</td>
      <td>10</td>
      <td>Carl</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>879</th>
      <td>879</td>
      <td>760641137271070720</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2016-08-03 00:59:13 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Theo. He can walk on water. Still comi...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/760641137...</td>
      <td>12</td>
      <td>10</td>
      <td>Theo</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>1085</th>
      <td>1085</td>
      <td>738184450748633089</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2016-06-02 01:44:22 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>For the last time, we only rate dogs. Pls stop...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/738184450...</td>
      <td>9</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>1135</th>
      <td>1135</td>
      <td>728409960103686147</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2016-05-06 02:24:02 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Wallace. He's a skater pup. He said se...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/728409960...</td>
      <td>10</td>
      <td>10</td>
      <td>Wallace</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>1121</th>
      <td>1121</td>
      <td>730924654643314689</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2016-05-13 00:56:32 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>We only rate dogs. Pls stop sending non-canine...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/730924654...</td>
      <td>9</td>
      <td>10</td>
      <td>unacceptable</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>1810</th>
      <td>1810</td>
      <td>676821958043033607</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-12-15 17:51:44 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>Finally some constructive political change in ...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/676821958...</td>
      <td>11</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>1042</th>
      <td>1042</td>
      <td>743895849529389061</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2016-06-17 19:59:26 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>When you're given AUX cord privileges from the...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/743895849...</td>
      <td>10</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>1754</th>
      <td>1754</td>
      <td>678798276842360832</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2015-12-21 04:44:55 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Linda. She fucking hates trees. 7/10 h...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/678798276...</td>
      <td>7</td>
      <td>10</td>
      <td>Linda</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>255</th>
      <td>255</td>
      <td>844223788422217728</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2017-03-21 16:26:50 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Margo. She just dug pup a massive hole...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/844223788...</td>
      <td>12</td>
      <td>10</td>
      <td>Margo</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
    <tr>
      <th>894</th>
      <td>894</td>
      <td>759197388317847553</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2016-07-30 01:22:17 +0000</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>This is Luna. She's just heckin precious af I ...</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>https://twitter.com/dog_rates/status/759197388...</td>
      <td>12</td>
      <td>10</td>
      <td>Luna</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
      <td>None</td>
    </tr>
  </tbody>
</table>
</div>



Assessment Findings:
T3- the first column to be removed as it the same as index.
Q3- Column Header is undescribtive: in_reply_to_status_id, in_reply_to_user_idname, doggo, floofer, pupper, puppo.


```python
# check for duplicated columns
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
      <th>Unnamed: 0</th>
      <th>tweet_id</th>
      <th>in_reply_to_status_id</th>
      <th>in_reply_to_user_id</th>
      <th>timestamp</th>
      <th>source</th>
      <th>text</th>
      <th>retweeted_status_id</th>
      <th>retweeted_status_user_id</th>
      <th>retweeted_status_timestamp</th>
      <th>expanded_urls</th>
      <th>rating_numerator</th>
      <th>rating_denominator</th>
      <th>name</th>
      <th>doggo</th>
      <th>floofer</th>
      <th>pupper</th>
      <th>puppo</th>
    </tr>
  </thead>
  <tbody>
  </tbody>
</table>
</div>




```python

```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 2356 entries, 0 to 2355
    Data columns (total 18 columns):
    Unnamed: 0                    2356 non-null int64
    tweet_id                      2356 non-null int64
    in_reply_to_status_id         78 non-null float64
    in_reply_to_user_id           78 non-null float64
    timestamp                     2356 non-null object
    source                        2356 non-null object
    text                          2356 non-null object
    retweeted_status_id           181 non-null float64
    retweeted_status_user_id      181 non-null float64
    retweeted_status_timestamp    181 non-null object
    expanded_urls                 2297 non-null object
    rating_numerator              2356 non-null int64
    rating_denominator            2356 non-null int64
    name                          2356 non-null object
    doggo                         2356 non-null object
    floofer                       2356 non-null object
    pupper                        2356 non-null object
    puppo                         2356 non-null object
    dtypes: float64(4), int64(4), object(10)
    memory usage: 331.4+ KB


Q4- For the data in column  in_reply_to_status_id: wrong data type (to be object insteade of float). 
Q5- For the data in column  in_reply_to_user_id: wrong data type (to be object insteade of float). 
Q6- For the data in column  retweeted_status_timestamp: wrong data type (to be date insteade of object). 
Q7- For the data in column  in_timestamp: wrong data type (to be date insteade of object). 
Q8- For the data in column  retweeted_status_id: wrong data type (to be object insteade of float). 
Q9- For the data in column  retweeted_status_user_id: wrong data type (to be object insteade of float). 
Q10- For the data in column  retweeted_status_timestamp: wrong data type (to be date insteade of object).
Q11- There are many empty arrays in the data frame.
Q12- In the columns doggo, floofer, pupper, puppo: there are data entered as none.
T3- the first column to be removed as it the same as index.


```python
# Check sorted data in the column doggo
```




    0        None
    1567     None
    1568     None
    1569     None
    1570     None
    1571     None
    1572     None
    1566     None
    1573     None
    1575     None
    1576     None
    1577     None
    1578     None
    1579     None
    1580     None
    1574     None
    1581     None
    1565     None
    1563     None
    1549     None
    1550     None
    1551     None
    1552     None
    1553     None
    1554     None
    1564     None
    1555     None
    1557     None
    1558     None
    1559     None
            ...  
    944     doggo
    362     doggo
    389     doggo
    1039    doggo
    835     doggo
    778     doggo
    429     doggo
    977     doggo
    956     doggo
    780     doggo
    211     doggo
    1113    doggo
    372     doggo
    1030    doggo
    914     doggo
    727     doggo
    426     doggo
    733     doggo
    919     doggo
    822     doggo
    1103    doggo
    423     doggo
    731     doggo
    782     doggo
    924     doggo
    818     doggo
    384     doggo
    385     doggo
    425     doggo
    447     doggo
    Name: doggo, Length: 2356, dtype: object




```python
# Check sorted data count in the column doggo
```




    None     2259
    doggo      97
    Name: doggo, dtype: int64




```python
# Check sorted data count in the column floofer
```




    None       2346
    floofer      10
    Name: floofer, dtype: int64




```python
# Check sorted data count in the column pupper
```




    None      2099
    pupper     257
    Name: pupper, dtype: int64




```python
# Check sorted data count in the column puppo
```




    None     2326
    puppo      30
    Name: puppo, dtype: int64



## 3- Assessing twitter_api data:


```python
# import the data file

# view the first 10 rows
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
      <th>Unnamed: 0</th>
      <th>contributors</th>
      <th>coordinates</th>
      <th>created_at</th>
      <th>display_text_range</th>
      <th>entities</th>
      <th>extended_entities</th>
      <th>favorite_count</th>
      <th>favorited</th>
      <th>full_text</th>
      <th>...</th>
      <th>possibly_sensitive_appealable</th>
      <th>quoted_status</th>
      <th>quoted_status_id</th>
      <th>quoted_status_id_str</th>
      <th>retweet_count</th>
      <th>retweeted</th>
      <th>retweeted_status</th>
      <th>source</th>
      <th>truncated</th>
      <th>user</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Tue Aug 01 16:23:56 +0000 2017</td>
      <td>[0, 85]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 892420639486877696, 'id_str'...</td>
      <td>39467</td>
      <td>False</td>
      <td>This is Phineas. He's a mystical boy. Only eve...</td>
      <td>...</td>
      <td>False</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>8853</td>
      <td>False</td>
      <td>NaN</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>False</td>
      <td>{'id': 4196983835, 'id_str': '4196983835', 'na...</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Tue Aug 01 00:17:27 +0000 2017</td>
      <td>[0, 138]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 892177413194625024, 'id_str'...</td>
      <td>33819</td>
      <td>False</td>
      <td>This is Tilly. She's just checking pup on you....</td>
      <td>...</td>
      <td>False</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>6514</td>
      <td>False</td>
      <td>NaN</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>False</td>
      <td>{'id': 4196983835, 'id_str': '4196983835', 'na...</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Mon Jul 31 00:18:03 +0000 2017</td>
      <td>[0, 121]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 891815175371796480, 'id_str'...</td>
      <td>25461</td>
      <td>False</td>
      <td>This is Archie. He is a rare Norwegian Pouncin...</td>
      <td>...</td>
      <td>False</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>4328</td>
      <td>False</td>
      <td>NaN</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>False</td>
      <td>{'id': 4196983835, 'id_str': '4196983835', 'na...</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Sun Jul 30 15:58:51 +0000 2017</td>
      <td>[0, 79]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 891689552724799489, 'id_str'...</td>
      <td>42908</td>
      <td>False</td>
      <td>This is Darla. She commenced a snooze mid meal...</td>
      <td>...</td>
      <td>False</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>8964</td>
      <td>False</td>
      <td>NaN</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>False</td>
      <td>{'id': 4196983835, 'id_str': '4196983835', 'na...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Sat Jul 29 16:00:24 +0000 2017</td>
      <td>[0, 138]</td>
      <td>{'hashtags': [{'text': 'BarkWeek', 'indices': ...</td>
      <td>{'media': [{'id': 891327551943041024, 'id_str'...</td>
      <td>41048</td>
      <td>False</td>
      <td>This is Franklin. He would like you to stop ca...</td>
      <td>...</td>
      <td>False</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>9774</td>
      <td>False</td>
      <td>NaN</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>False</td>
      <td>{'id': 4196983835, 'id_str': '4196983835', 'na...</td>
    </tr>
    <tr>
      <th>5</th>
      <td>5</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Sat Jul 29 00:08:17 +0000 2017</td>
      <td>[0, 138]</td>
      <td>{'hashtags': [{'text': 'BarkWeek', 'indices': ...</td>
      <td>{'media': [{'id': 891087942176911360, 'id_str'...</td>
      <td>20562</td>
      <td>False</td>
      <td>Here we have a majestic great white breaching ...</td>
      <td>...</td>
      <td>False</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>3261</td>
      <td>False</td>
      <td>NaN</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>False</td>
      <td>{'id': 4196983835, 'id_str': '4196983835', 'na...</td>
    </tr>
    <tr>
      <th>6</th>
      <td>6</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Fri Jul 28 16:27:12 +0000 2017</td>
      <td>[0, 140]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 890971906207338496, 'id_str'...</td>
      <td>12041</td>
      <td>False</td>
      <td>Meet Jax. He enjoys ice cream so much he gets ...</td>
      <td>...</td>
      <td>False</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>2158</td>
      <td>False</td>
      <td>NaN</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>False</td>
      <td>{'id': 4196983835, 'id_str': '4196983835', 'na...</td>
    </tr>
    <tr>
      <th>7</th>
      <td>7</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Fri Jul 28 00:22:40 +0000 2017</td>
      <td>[0, 118]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 890729118844600320, 'id_str'...</td>
      <td>56848</td>
      <td>False</td>
      <td>When you watch your owner call another dog a g...</td>
      <td>...</td>
      <td>False</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>16716</td>
      <td>False</td>
      <td>NaN</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>False</td>
      <td>{'id': 4196983835, 'id_str': '4196983835', 'na...</td>
    </tr>
    <tr>
      <th>8</th>
      <td>8</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Thu Jul 27 16:25:51 +0000 2017</td>
      <td>[0, 122]</td>
      <td>{'hashtags': [{'text': 'BarkWeek', 'indices': ...</td>
      <td>{'media': [{'id': 890609177319665665, 'id_str'...</td>
      <td>28226</td>
      <td>False</td>
      <td>This is Zoey. She doesn't want to be one of th...</td>
      <td>...</td>
      <td>False</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>4429</td>
      <td>False</td>
      <td>NaN</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>False</td>
      <td>{'id': 4196983835, 'id_str': '4196983835', 'na...</td>
    </tr>
    <tr>
      <th>9</th>
      <td>9</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>Wed Jul 26 15:59:51 +0000 2017</td>
      <td>[0, 133]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 890240245463175168, 'id_str'...</td>
      <td>32467</td>
      <td>False</td>
      <td>This is Cassie. She is a college pup. Studying...</td>
      <td>...</td>
      <td>False</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>7711</td>
      <td>False</td>
      <td>NaN</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>False</td>
      <td>{'id': 4196983835, 'id_str': '4196983835', 'na...</td>
    </tr>
  </tbody>
</table>
<p>10 rows × 32 columns</p>
</div>




```python
# view the last 10 rows
```


```python
# view the random sample of 10 rows
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
      <th>Unnamed: 0</th>
      <th>created_at</th>
      <th>id</th>
      <th>id_str</th>
      <th>full_text</th>
      <th>truncated</th>
      <th>display_text_range</th>
      <th>entities</th>
      <th>extended_entities</th>
      <th>source</th>
      <th>...</th>
      <th>favorite_count</th>
      <th>favorited</th>
      <th>retweeted</th>
      <th>possibly_sensitive</th>
      <th>possibly_sensitive_appealable</th>
      <th>lang</th>
      <th>retweeted_status</th>
      <th>quoted_status_id</th>
      <th>quoted_status_id_str</th>
      <th>quoted_status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>290</th>
      <td>290</td>
      <td>Sat Mar 04 17:56:49 +0000 2017</td>
      <td>838085839343206401</td>
      <td>838085839343206401</td>
      <td>@bragg6of8 @Andy_Pace_ we are still looking fo...</td>
      <td>False</td>
      <td>[23, 63]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>NaN</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>...</td>
      <td>150</td>
      <td>False</td>
      <td>False</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>en</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>315</th>
      <td>315</td>
      <td>Fri Feb 24 01:03:08 +0000 2017</td>
      <td>834931633769889797</td>
      <td>834931633769889797</td>
      <td>This is Tucker. He decided it was time to part...</td>
      <td>False</td>
      <td>[0, 127]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 834931620566208513, 'id_str'...</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>...</td>
      <td>11838</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>en</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1517</th>
      <td>1517</td>
      <td>Sat Jan 23 03:20:44 +0000 2016</td>
      <td>690735892932222976</td>
      <td>690735892932222976</td>
      <td>Say hello to Peaches. She's a Dingleberry Zand...</td>
      <td>False</td>
      <td>[0, 102]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 690735878365315073, 'id_str'...</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>...</td>
      <td>4134</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>en</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>406</th>
      <td>406</td>
      <td>Tue Jan 24 01:08:40 +0000 2017</td>
      <td>823699002998870016</td>
      <td>823699002998870016</td>
      <td>This is Winston. The goggles make him a superh...</td>
      <td>False</td>
      <td>[0, 135]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 823698991951056896, 'id_str'...</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>...</td>
      <td>13826</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>en</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2320</th>
      <td>2320</td>
      <td>Tue Nov 17 01:40:41 +0000 2015</td>
      <td>666430724426358785</td>
      <td>666430724426358785</td>
      <td>Oh boy what a pup! Sunglasses take this one to...</td>
      <td>False</td>
      <td>[0, 129]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 666430720227860480, 'id_str'...</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>...</td>
      <td>330</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>en</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>85</th>
      <td>85</td>
      <td>Fri Jun 16 16:11:53 +0000 2017</td>
      <td>875747767867523072</td>
      <td>875747767867523072</td>
      <td>This is Goose. He's a womanizer. Cheeky as h*c...</td>
      <td>False</td>
      <td>[0, 125]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 875747755280318464, 'id_str'...</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>...</td>
      <td>25773</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>en</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>281</th>
      <td>281</td>
      <td>Tue Mar 07 22:22:32 +0000 2017</td>
      <td>839239871831150596</td>
      <td>839239871831150596</td>
      <td>This is Odie. He's big. 13/10 would attempt to...</td>
      <td>False</td>
      <td>[0, 51]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 839239862192648194, 'id_str'...</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>...</td>
      <td>29684</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>en</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2079</th>
      <td>2079</td>
      <td>Sun Nov 29 04:32:51 +0000 2015</td>
      <td>670822709593571328</td>
      <td>670822709593571328</td>
      <td>Can't do better than this lol. 10/10 for the o...</td>
      <td>False</td>
      <td>[0, 74]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 670822703281086466, 'id_str'...</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>...</td>
      <td>647</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>en</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>152</th>
      <td>152</td>
      <td>Thu May 11 00:01:27 +0000 2017</td>
      <td>862457590147678208</td>
      <td>862457590147678208</td>
      <td>This is Jersey. He likes to watch movies, but ...</td>
      <td>False</td>
      <td>[0, 133]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 862457580722860032, 'id_str'...</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>...</td>
      <td>21492</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>en</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2288</th>
      <td>2288</td>
      <td>Thu Nov 19 02:43:18 +0000 2015</td>
      <td>667171260800061440</td>
      <td>667171260800061440</td>
      <td>Say hello to Kenneth. He likes Reese's Puffs. ...</td>
      <td>False</td>
      <td>[0, 75]</td>
      <td>{'hashtags': [], 'symbols': [], 'user_mentions...</td>
      <td>{'media': [{'id': 667171256467398656, 'id_str'...</td>
      <td>&lt;a href="http://twitter.com/download/iphone" r...</td>
      <td>...</td>
      <td>235</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>False</td>
      <td>en</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
<p>10 rows × 32 columns</p>
</div>




```python
# view the information
```

Assessment findings:
T4- Columns id, id_str contain the same data.
T5- the first column to be removed as it the same as index.
Q13- Column Header is undescribtive: extended_entities, sourc, lang
Q14- There are many missing data.
Q15- For the data in column  created_at: wrong data type (to be date insteade of object). 
Q16- For the data in column  in_reply_to_status_id: wrong data type (to be object insteade of float64).
Q17- For the data in column  in_reply_to_status_id_str: wrong data type (to be object insteade of float64).
Q18- For the data in column  in_reply_to_status_id_str: wrong data type (to be object insteade of float64).


```python
# check for duplicated rows
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
      <th>Unnamed: 0</th>
      <th>contributors</th>
      <th>coordinates</th>
      <th>created_at</th>
      <th>display_text_range</th>
      <th>entities</th>
      <th>extended_entities</th>
      <th>favorite_count</th>
      <th>favorited</th>
      <th>full_text</th>
      <th>...</th>
      <th>possibly_sensitive_appealable</th>
      <th>quoted_status</th>
      <th>quoted_status_id</th>
      <th>quoted_status_id_str</th>
      <th>retweet_count</th>
      <th>retweeted</th>
      <th>retweeted_status</th>
      <th>source</th>
      <th>truncated</th>
      <th>user</th>
    </tr>
  </thead>
  <tbody>
  </tbody>
</table>
<p>0 rows × 32 columns</p>
</div>




```python

```




    False    2346
    True        8
    Name: favorited, dtype: int64




```python

```




    13               Unnamed: 0
    45               Unnamed: 0
    46                 tweet_id
    47    in_reply_to_status_id
    48      in_reply_to_user_id
    50                   source
    dtype: object



Assessment Final Findings:

A) image_predictions:

Quality issues:
Q1- Column Header is undescribtive: img_num	p1, p1_conf, p1_dog, p2, p2_conf, p2_dog, p3, p3_conf, p3_dog.
Q2- some of the dogs types are incorrect, such in p1 column: car_mirror in raw 371, snorkel in row 655, killer_whale in column 337, mousetrap in row 889

Tiddiness issues:
T1- img_num column contain the data as the same for the jpg_url column.
T2- the first column to be removed as it the same as index.


B) twetter_archive:

Quality issues:
Q4- For the data in column  in_reply_to_status_id: wrong data type (to be object insteade of float). 
Q5- For the data in column  in_reply_to_user_id: wrong data type (to be object insteade of float). 
Q6- For the data in column  retweeted_status_timestamp: wrong data type (to be date insteade of object). 
Q7- For the data in column  in_timestamp: wrong data type (to be date insteade of object). 
Q8- For the data in column  retweeted_status_id: wrong data type (to be object insteade of float). 
Q9- For the data in column  retweeted_status_user_id: wrong data type (to be object insteade of float). 
Q10- For the data in column  retweeted_status_timestamp: wrong data type (to be date insteade of object).
Q11- There are many empty arrays in the data frame.


Tiddiness issues:
T3- the first column to be removed as it the same as index.
T4- In the columns doggo, floofer, pupper, puppo: need to be melted in one column.

C) twettr_api:

Quality issues:
Q12- Column Header is undescribtive: extended_entities, sourc, lang
Q13- There are many missing data.
Q14- For the data in column  created_at: wrong data type (to be date insteade of object). 
Q15- For the data in column  in_reply_to_status_id: wrong data type (to be object insteade of float64).
Q16- For the data in column  in_reply_to_status_id_str: wrong data type (to be object insteade of float64).
Q17- For the data in column  in_reply_to_status_id_str: wrong data type (to be object insteade of float64).

Tiddiness issues:
T5- Columns id, id_str contain the same data.
T6- the first column to be removed as it the same as index.

D) All the 3 data frame:
T7- All the 3 data frame can be merged in one dataframe, using the tweet id as index, and the follwing columns are replicated between them:in_reply_to_status_id, in_reply_to_user_id, source

# 3- Cleaning:


```python
# make a copy of data files, to prevent loss of original data

```

## 3.1- Clean clean_twettr_api:

#### Define:

Clean the unneeded columns in the clean_twettr_api Dataframe:
Delete all columns except:  tweet ID, retweet count, and favorite count
https://cmdlinetips.com/2018/04/how-to-drop-one-or-more-columns-in-pandas-dataframe/

#### Code:


```python
# list all the columns of the dataframe

```




    Index(['Unnamed: 0', 'contributors', 'coordinates', 'created_at',
           'display_text_range', 'entities', 'extended_entities', 'favorite_count',
           'favorited', 'full_text', 'geo', 'id', 'id_str',
           'in_reply_to_screen_name', 'in_reply_to_status_id',
           'in_reply_to_status_id_str', 'in_reply_to_user_id',
           'in_reply_to_user_id_str', 'is_quote_status', 'lang', 'place',
           'possibly_sensitive', 'possibly_sensitive_appealable', 'quoted_status',
           'quoted_status_id', 'quoted_status_id_str', 'retweet_count',
           'retweeted', 'retweeted_status', 'source', 'truncated', 'user'],
          dtype='object')




```python
# delete all columns, except tweet ID, retweet count, and favorite count
```

#### Test:


```python
# Check the remaining columns 
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 2354 entries, 0 to 2353
    Data columns (total 3 columns):
    favorite_count    2354 non-null int64
    id                2354 non-null int64
    retweet_count     2354 non-null int64
    dtypes: int64(3)
    memory usage: 55.2 KB


#### Define:

Rename the column of clean_twettr_api_1 id column to tweet_id to merge them
https://www.datacamp.com/community/tutorials/python-rename-column?utm_source=adwords_ppc&utm_campaignid=1455363063&utm_adgroupid=65083631748&utm_device=c&utm_keyword=&utm_matchtype=b&utm_network=g&utm_adpostion=&utm_creative=332602034361&utm_targetid=dsa-429603003980&utm_loc_interest_ms=&utm_loc_physical_ms=1005386&gclid=CjwKCAiA17P9BRB2EiwAMvwNyH3bB3luhVIX_22iCIfPZwCoJjjtqPUT2w-3lNkwFKdfitIMfwL1ABoCCRgQAvD_BwE

#### Code:


```python
# Rename ID column
```

#### Test Code:


```python

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
      <th>favorite_count</th>
      <th>tweet_id</th>
      <th>retweet_count</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>39467</td>
      <td>892420643555336193</td>
      <td>8853</td>
    </tr>
    <tr>
      <th>1</th>
      <td>33819</td>
      <td>892177421306343426</td>
      <td>6514</td>
    </tr>
    <tr>
      <th>2</th>
      <td>25461</td>
      <td>891815181378084864</td>
      <td>4328</td>
    </tr>
    <tr>
      <th>3</th>
      <td>42908</td>
      <td>891689557279858688</td>
      <td>8964</td>
    </tr>
    <tr>
      <th>4</th>
      <td>41048</td>
      <td>891327558926688256</td>
      <td>9774</td>
    </tr>
  </tbody>
</table>
</div>



## 3.2- Clean clean_twetter_archive:

#### Define:

Melt the columns doggo, floofer, pupper, puppo to dog_type

#### Code:


```python
# check the doggo column values
```




    None     2259
    doggo      97
    Name: doggo, dtype: int64




```python
# check the floofer column values
```




    None       2346
    floofer      10
    Name: floofer, dtype: int64




```python
# check the floofer column values
```




    None      2099
    pupper     257
    Name: pupper, dtype: int64




```python
# check the puppo column values
```




    None     2326
    puppo      30
    Name: puppo, dtype: int64




```python
# list the columns in clean_twetter_archive
```




    Index(['Unnamed: 0', 'tweet_id', 'in_reply_to_status_id',
           'in_reply_to_user_id', 'timestamp', 'source', 'text',
           'retweeted_status_id', 'retweeted_status_user_id',
           'retweeted_status_timestamp', 'expanded_urls', 'rating_numerator',
           'rating_denominator', 'name', 'doggo', 'floofer', 'pupper', 'puppo'],
          dtype='object')




```python
# melt the 4 columns into new dog_type column
```


```python
# Check columns after melting
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 9424 entries, 0 to 9423
    Data columns (total 16 columns):
    Unnamed: 0                    9424 non-null int64
    tweet_id                      9424 non-null int64
    in_reply_to_status_id         312 non-null float64
    in_reply_to_user_id           312 non-null float64
    timestamp                     9424 non-null object
    source                        9424 non-null object
    text                          9424 non-null object
    retweeted_status_id           724 non-null float64
    retweeted_status_user_id      724 non-null float64
    retweeted_status_timestamp    724 non-null object
    expanded_urls                 9188 non-null object
    rating_numerator              9424 non-null int64
    rating_denominator            9424 non-null int64
    name                          9424 non-null object
    types                         9424 non-null object
    dog_type                      9424 non-null object
    dtypes: float64(4), int64(4), object(8)
    memory usage: 1.2+ MB



```python
#Check the count of each of the dog types
```




    None       9030
    pupper      257
    doggo        97
    puppo        30
    floofer      10
    Name: dog_type, dtype: int64




```python
# remove thd duplicates of the data frame after melting
```

#### Test:


```python
#Check the count of each of the dog types
```




    None       1976
    pupper      257
    doggo        83
    puppo        30
    floofer      10
    Name: dog_type, dtype: int64




```python

```

    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 2356 entries, 2259 to 7236
    Data columns (total 16 columns):
    Unnamed: 0                    2356 non-null int64
    tweet_id                      2356 non-null int64
    in_reply_to_status_id         78 non-null float64
    in_reply_to_user_id           78 non-null float64
    timestamp                     2356 non-null object
    source                        2356 non-null object
    text                          2356 non-null object
    retweeted_status_id           181 non-null float64
    retweeted_status_user_id      181 non-null float64
    retweeted_status_timestamp    181 non-null object
    expanded_urls                 2297 non-null object
    rating_numerator              2356 non-null int64
    rating_denominator            2356 non-null int64
    name                          2356 non-null object
    types                         2356 non-null object
    dog_type                      2356 non-null object
    dtypes: float64(4), int64(4), object(8)
    memory usage: 312.9+ KB


#### Define:

Remove the unnessary data columns

#### Code:


```python
# List all the columns
```




    Index(['Unnamed: 0', 'tweet_id', 'in_reply_to_status_id',
           'in_reply_to_user_id', 'timestamp', 'source', 'text',
           'retweeted_status_id', 'retweeted_status_user_id',
           'retweeted_status_timestamp', 'expanded_urls', 'rating_numerator',
           'rating_denominator', 'name', 'types', 'dog_type'],
          dtype='object')




```python
# Remove the columns:
```


```python
# Remove more
```

#### Test:


```python

```




    Index(['tweet_id', 'retweeted_status_id', 'retweeted_status_user_id',
           'expanded_urls', 'rating_numerator', 'name', 'dog_type'],
          dtype='object')




```python

```

    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 2356 entries, 2259 to 7236
    Data columns (total 7 columns):
    tweet_id                    2356 non-null int64
    retweeted_status_id         181 non-null float64
    retweeted_status_user_id    181 non-null float64
    expanded_urls               2297 non-null object
    rating_numerator            2356 non-null int64
    name                        2356 non-null object
    dog_type                    2356 non-null object
    dtypes: float64(2), int64(2), object(3)
    memory usage: 147.2+ KB


#### Define:

Rename the undescriptive colums names

#### Code:


```python
# rename the columns
```

#### Test:


```python

```




    Index(['tweet_id', 'retweeted_status_id', 'retweeted_status_user_id',
           'expanded_urls', 'rating_numerator', 'dog_name', 'dog_type'],
          dtype='object')




```python

```

    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 2356 entries, 2259 to 7236
    Data columns (total 7 columns):
    tweet_id                    2356 non-null int64
    retweeted_status_id         181 non-null float64
    retweeted_status_user_id    181 non-null float64
    expanded_urls               2297 non-null object
    rating_numerator            2356 non-null int64
    dog_name                    2356 non-null object
    dog_type                    2356 non-null object
    dtypes: float64(2), int64(2), object(3)
    memory usage: 147.2+ KB


#### Define:

Change the columns data types to the correct types (float to object):
    retweeted_status_id
    retweeted_status_user_id

#### Code:


```python
# Change retweeted_status_id: wrong data type (to be object insteade of float).
```


```python
# Change retweeted_status_user_id: wrong data type (to be object insteade of float).
```

#### Test:


```python
# check the columns data types
```

    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 2356 entries, 2259 to 7236
    Data columns (total 7 columns):
    tweet_id                    2356 non-null int64
    retweeted_status_id         2356 non-null object
    retweeted_status_user_id    2356 non-null object
    expanded_urls               2297 non-null object
    rating_numerator            2356 non-null int64
    dog_name                    2356 non-null object
    dog_type                    2356 non-null object
    dtypes: int64(2), object(5)
    memory usage: 147.2+ KB


## 3.3- Clean clean_image_predictions:

#### Define:

Remove the unusable columns

#### Code:


```python
# list the columns
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
      <th>Unnamed: 0</th>
      <th>tweet_id</th>
      <th>jpg_url</th>
      <th>img_num</th>
      <th>p1</th>
      <th>p1_conf</th>
      <th>p1_dog</th>
      <th>p2</th>
      <th>p2_conf</th>
      <th>p2_dog</th>
      <th>p3</th>
      <th>p3_conf</th>
      <th>p3_dog</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>666020888022790149</td>
      <td>https://pbs.twimg.com/media/CT4udn0WwAA0aMy.jpg</td>
      <td>1</td>
      <td>Welsh_springer_spaniel</td>
      <td>0.465074</td>
      <td>True</td>
      <td>collie</td>
      <td>0.156665</td>
      <td>True</td>
      <td>Shetland_sheepdog</td>
      <td>0.061428</td>
      <td>True</td>
    </tr>
    <tr>
      <th>1</th>
      <td>1</td>
      <td>666029285002620928</td>
      <td>https://pbs.twimg.com/media/CT42GRgUYAA5iDo.jpg</td>
      <td>1</td>
      <td>redbone</td>
      <td>0.506826</td>
      <td>True</td>
      <td>miniature_pinscher</td>
      <td>0.074192</td>
      <td>True</td>
      <td>Rhodesian_ridgeback</td>
      <td>0.072010</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2</td>
      <td>666033412701032449</td>
      <td>https://pbs.twimg.com/media/CT4521TWwAEvMyu.jpg</td>
      <td>1</td>
      <td>German_shepherd</td>
      <td>0.596461</td>
      <td>True</td>
      <td>malinois</td>
      <td>0.138584</td>
      <td>True</td>
      <td>bloodhound</td>
      <td>0.116197</td>
      <td>True</td>
    </tr>
    <tr>
      <th>3</th>
      <td>3</td>
      <td>666044226329800704</td>
      <td>https://pbs.twimg.com/media/CT5Dr8HUEAA-lEu.jpg</td>
      <td>1</td>
      <td>Rhodesian_ridgeback</td>
      <td>0.408143</td>
      <td>True</td>
      <td>redbone</td>
      <td>0.360687</td>
      <td>True</td>
      <td>miniature_pinscher</td>
      <td>0.222752</td>
      <td>True</td>
    </tr>
    <tr>
      <th>4</th>
      <td>4</td>
      <td>666049248165822465</td>
      <td>https://pbs.twimg.com/media/CT5IQmsXIAAKY4A.jpg</td>
      <td>1</td>
      <td>miniature_pinscher</td>
      <td>0.560311</td>
      <td>True</td>
      <td>Rottweiler</td>
      <td>0.243682</td>
      <td>True</td>
      <td>Doberman</td>
      <td>0.154629</td>
      <td>True</td>
    </tr>
  </tbody>
</table>
</div>




```python
# list the columns
```




    Index(['Unnamed: 0', 'tweet_id', 'jpg_url', 'img_num', 'p1', 'p1_conf',
           'p1_dog', 'p2', 'p2_conf', 'p2_dog', 'p3', 'p3_conf', 'p3_dog'],
          dtype='object')




```python
# Remove the columns
```

#### Test:


```python
# list the columns
```




    Index(['tweet_id', 'jpg_url', 'p1', 'p1_conf', 'p1_dog', 'p2', 'p2_conf',
           'p2_dog', 'p3', 'p3_conf', 'p3_dog'],
          dtype='object')




```python
# list the columns
```

    <class 'pandas.core.frame.DataFrame'>
    RangeIndex: 2075 entries, 0 to 2074
    Data columns (total 11 columns):
    tweet_id    2075 non-null int64
    jpg_url     2075 non-null object
    p1          2075 non-null object
    p1_conf     2075 non-null float64
    p1_dog      2075 non-null bool
    p2          2075 non-null object
    p2_conf     2075 non-null float64
    p2_dog      2075 non-null bool
    p3          2075 non-null object
    p3_conf     2075 non-null float64
    p3_dog      2075 non-null bool
    dtypes: bool(3), float64(3), int64(1), object(4)
    memory usage: 135.8+ KB


## 3.4- Merge the data:

#### Define:

Merge the three data fram into one using the tweet id column as index

https://www.datacamp.com/community/tutorials/joining-dataframes-pandas?utm_source=adwords_ppc&utm_campaignid=1455363063&utm_adgroupid=65083631748&utm_device=c&utm_keyword=&utm_matchtype=b&utm_network=g&utm_adpostion=&utm_creative=278443377086&utm_targetid=dsa-429603003980&utm_loc_interest_ms=&utm_loc_physical_ms=9048953&gclid=CjwKCAiAkan9BRAqEiwAP9X6Uesd4feZ9gwzZt3XVSY8ro9Wquw0q2v0kGjKo2V5t5qxrXHRuQDOZhoCeHQQAvD_BwE

#### Code:


```python
# merge data

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
      <th>favorite_count</th>
      <th>tweet_id</th>
      <th>retweet_count</th>
      <th>retweeted_status_id</th>
      <th>retweeted_status_user_id</th>
      <th>expanded_urls</th>
      <th>rating_numerator</th>
      <th>dog_name</th>
      <th>dog_type</th>
      <th>jpg_url</th>
      <th>p1</th>
      <th>p1_conf</th>
      <th>p1_dog</th>
      <th>p2</th>
      <th>p2_conf</th>
      <th>p2_dog</th>
      <th>p3</th>
      <th>p3_conf</th>
      <th>p3_dog</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>39467</td>
      <td>892420643555336193</td>
      <td>8853</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/892420643...</td>
      <td>13</td>
      <td>Phineas</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DGKD1-bXoAAIAUK.jpg</td>
      <td>orange</td>
      <td>0.097049</td>
      <td>False</td>
      <td>bagel</td>
      <td>0.085851</td>
      <td>False</td>
      <td>banana</td>
      <td>0.076110</td>
      <td>False</td>
    </tr>
    <tr>
      <th>1</th>
      <td>33819</td>
      <td>892177421306343426</td>
      <td>6514</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/892177421...</td>
      <td>13</td>
      <td>Tilly</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DGGmoV4XsAAUL6n.jpg</td>
      <td>Chihuahua</td>
      <td>0.323581</td>
      <td>True</td>
      <td>Pekinese</td>
      <td>0.090647</td>
      <td>True</td>
      <td>papillon</td>
      <td>0.068957</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2</th>
      <td>25461</td>
      <td>891815181378084864</td>
      <td>4328</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/891815181...</td>
      <td>12</td>
      <td>Archie</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DGBdLU1WsAANxJ9.jpg</td>
      <td>Chihuahua</td>
      <td>0.716012</td>
      <td>True</td>
      <td>malamute</td>
      <td>0.078253</td>
      <td>True</td>
      <td>kelpie</td>
      <td>0.031379</td>
      <td>True</td>
    </tr>
    <tr>
      <th>3</th>
      <td>42908</td>
      <td>891689557279858688</td>
      <td>8964</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/891689557...</td>
      <td>13</td>
      <td>Darla</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF_q7IAWsAEuuN8.jpg</td>
      <td>paper_towel</td>
      <td>0.170278</td>
      <td>False</td>
      <td>Labrador_retriever</td>
      <td>0.168086</td>
      <td>True</td>
      <td>spatula</td>
      <td>0.040836</td>
      <td>False</td>
    </tr>
    <tr>
      <th>4</th>
      <td>41048</td>
      <td>891327558926688256</td>
      <td>9774</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/891327558...</td>
      <td>12</td>
      <td>Franklin</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF6hr6BUMAAzZgT.jpg</td>
      <td>basset</td>
      <td>0.555712</td>
      <td>True</td>
      <td>English_springer</td>
      <td>0.225770</td>
      <td>True</td>
      <td>German_short-haired_pointer</td>
      <td>0.175219</td>
      <td>True</td>
    </tr>
    <tr>
      <th>5</th>
      <td>20562</td>
      <td>891087950875897856</td>
      <td>3261</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/891087950...</td>
      <td>13</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF3HwyEWsAABqE6.jpg</td>
      <td>Chesapeake_Bay_retriever</td>
      <td>0.425595</td>
      <td>True</td>
      <td>Irish_terrier</td>
      <td>0.116317</td>
      <td>True</td>
      <td>Indian_elephant</td>
      <td>0.076902</td>
      <td>False</td>
    </tr>
    <tr>
      <th>6</th>
      <td>12041</td>
      <td>890971913173991426</td>
      <td>2158</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://gofundme.com/ydvmve-surgery-for-jax,ht...</td>
      <td>13</td>
      <td>Jax</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF1eOmZXUAALUcq.jpg</td>
      <td>Appenzeller</td>
      <td>0.341703</td>
      <td>True</td>
      <td>Border_collie</td>
      <td>0.199287</td>
      <td>True</td>
      <td>ice_lolly</td>
      <td>0.193548</td>
      <td>False</td>
    </tr>
    <tr>
      <th>7</th>
      <td>56848</td>
      <td>890729181411237888</td>
      <td>16716</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/890729181...</td>
      <td>13</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFyBahAVwAAhUTd.jpg</td>
      <td>Pomeranian</td>
      <td>0.566142</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.178406</td>
      <td>True</td>
      <td>Pembroke</td>
      <td>0.076507</td>
      <td>True</td>
    </tr>
    <tr>
      <th>8</th>
      <td>28226</td>
      <td>890609185150312448</td>
      <td>4429</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/890609185...</td>
      <td>13</td>
      <td>Zoey</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFwUU__XcAEpyXI.jpg</td>
      <td>Irish_terrier</td>
      <td>0.487574</td>
      <td>True</td>
      <td>Irish_setter</td>
      <td>0.193054</td>
      <td>True</td>
      <td>Chesapeake_Bay_retriever</td>
      <td>0.118184</td>
      <td>True</td>
    </tr>
    <tr>
      <th>9</th>
      <td>32467</td>
      <td>890240255349198849</td>
      <td>7711</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/890240255...</td>
      <td>14</td>
      <td>Cassie</td>
      <td>doggo</td>
      <td>https://pbs.twimg.com/media/DFrEyVuW0AAO3t9.jpg</td>
      <td>Pembroke</td>
      <td>0.511319</td>
      <td>True</td>
      <td>Cardigan</td>
      <td>0.451038</td>
      <td>True</td>
      <td>Chihuahua</td>
      <td>0.029248</td>
      <td>True</td>
    </tr>
    <tr>
      <th>10</th>
      <td>31166</td>
      <td>890006608113172480</td>
      <td>7624</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/890006608...</td>
      <td>13</td>
      <td>Koda</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFnwSY4WAAAMliS.jpg</td>
      <td>Samoyed</td>
      <td>0.957979</td>
      <td>True</td>
      <td>Pomeranian</td>
      <td>0.013884</td>
      <td>True</td>
      <td>chow</td>
      <td>0.008167</td>
      <td>True</td>
    </tr>
    <tr>
      <th>11</th>
      <td>28268</td>
      <td>889880896479866881</td>
      <td>5156</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/889880896...</td>
      <td>13</td>
      <td>Bruno</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFl99B1WsAITKsg.jpg</td>
      <td>French_bulldog</td>
      <td>0.377417</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.151317</td>
      <td>True</td>
      <td>muzzle</td>
      <td>0.082981</td>
      <td>False</td>
    </tr>
    <tr>
      <th>12</th>
      <td>38818</td>
      <td>889665388333682689</td>
      <td>8538</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/889665388...</td>
      <td>13</td>
      <td>None</td>
      <td>puppo</td>
      <td>https://pbs.twimg.com/media/DFi579UWsAAatzw.jpg</td>
      <td>Pembroke</td>
      <td>0.966327</td>
      <td>True</td>
      <td>Cardigan</td>
      <td>0.027356</td>
      <td>True</td>
      <td>basenji</td>
      <td>0.004633</td>
      <td>True</td>
    </tr>
    <tr>
      <th>13</th>
      <td>27672</td>
      <td>889638837579907072</td>
      <td>4735</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/889638837...</td>
      <td>12</td>
      <td>Ted</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFihzFfXsAYGDPR.jpg</td>
      <td>French_bulldog</td>
      <td>0.991650</td>
      <td>True</td>
      <td>boxer</td>
      <td>0.002129</td>
      <td>True</td>
      <td>Staffordshire_bullterrier</td>
      <td>0.001498</td>
      <td>True</td>
    </tr>
    <tr>
      <th>14</th>
      <td>15359</td>
      <td>889531135344209921</td>
      <td>2321</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/889531135...</td>
      <td>13</td>
      <td>Stuart</td>
      <td>puppo</td>
      <td>https://pbs.twimg.com/media/DFg_2PVW0AEHN3p.jpg</td>
      <td>golden_retriever</td>
      <td>0.953442</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.013834</td>
      <td>True</td>
      <td>redbone</td>
      <td>0.007958</td>
      <td>True</td>
    </tr>
    <tr>
      <th>15</th>
      <td>25652</td>
      <td>889278841981685760</td>
      <td>5637</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/889278841...</td>
      <td>13</td>
      <td>Oliver</td>
      <td>None</td>
      <td>https://pbs.twimg.com/ext_tw_video_thumb/88927...</td>
      <td>whippet</td>
      <td>0.626152</td>
      <td>True</td>
      <td>borzoi</td>
      <td>0.194742</td>
      <td>True</td>
      <td>Saluki</td>
      <td>0.027351</td>
      <td>True</td>
    </tr>
    <tr>
      <th>16</th>
      <td>29611</td>
      <td>888917238123831296</td>
      <td>4709</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/888917238...</td>
      <td>12</td>
      <td>Jim</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFYRgsOUQAARGhO.jpg</td>
      <td>golden_retriever</td>
      <td>0.714719</td>
      <td>True</td>
      <td>Tibetan_mastiff</td>
      <td>0.120184</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.105506</td>
      <td>True</td>
    </tr>
    <tr>
      <th>17</th>
      <td>26080</td>
      <td>888804989199671297</td>
      <td>4559</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/888804989...</td>
      <td>13</td>
      <td>Zeke</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFWra-3VYAA2piG.jpg</td>
      <td>golden_retriever</td>
      <td>0.469760</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.184172</td>
      <td>True</td>
      <td>English_setter</td>
      <td>0.073482</td>
      <td>True</td>
    </tr>
    <tr>
      <th>18</th>
      <td>20290</td>
      <td>888554962724278272</td>
      <td>3732</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/888554962...</td>
      <td>13</td>
      <td>Ralphus</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFTH_O-UQAACu20.jpg</td>
      <td>Siberian_husky</td>
      <td>0.700377</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.166511</td>
      <td>True</td>
      <td>malamute</td>
      <td>0.111411</td>
      <td>True</td>
    </tr>
    <tr>
      <th>19</th>
      <td>22201</td>
      <td>888078434458587136</td>
      <td>3653</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/888078434...</td>
      <td>12</td>
      <td>Gerald</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFMWn56WsAAkA7B.jpg</td>
      <td>French_bulldog</td>
      <td>0.995026</td>
      <td>True</td>
      <td>pug</td>
      <td>0.000932</td>
      <td>True</td>
      <td>bull_mastiff</td>
      <td>0.000903</td>
      <td>True</td>
    </tr>
    <tr>
      <th>20</th>
      <td>30779</td>
      <td>887705289381826560</td>
      <td>5609</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/887705289...</td>
      <td>13</td>
      <td>Jeffrey</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFHDQBbXgAEqY7t.jpg</td>
      <td>basset</td>
      <td>0.821664</td>
      <td>True</td>
      <td>redbone</td>
      <td>0.087582</td>
      <td>True</td>
      <td>Weimaraner</td>
      <td>0.026236</td>
      <td>True</td>
    </tr>
    <tr>
      <th>21</th>
      <td>46959</td>
      <td>887517139158093824</td>
      <td>12082</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/887517139...</td>
      <td>14</td>
      <td>such</td>
      <td>None</td>
      <td>https://pbs.twimg.com/ext_tw_video_thumb/88751...</td>
      <td>limousine</td>
      <td>0.130432</td>
      <td>False</td>
      <td>tow_truck</td>
      <td>0.029175</td>
      <td>False</td>
      <td>shopping_cart</td>
      <td>0.026321</td>
      <td>False</td>
    </tr>
    <tr>
      <th>22</th>
      <td>69871</td>
      <td>887473957103951883</td>
      <td>18781</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/887473957...</td>
      <td>13</td>
      <td>Canela</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFDw2tyUQAAAFke.jpg</td>
      <td>Pembroke</td>
      <td>0.809197</td>
      <td>True</td>
      <td>Rhodesian_ridgeback</td>
      <td>0.054950</td>
      <td>True</td>
      <td>beagle</td>
      <td>0.038915</td>
      <td>True</td>
    </tr>
    <tr>
      <th>23</th>
      <td>34222</td>
      <td>887343217045368832</td>
      <td>10737</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/887343217...</td>
      <td>13</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/ext_tw_video_thumb/88734...</td>
      <td>Mexican_hairless</td>
      <td>0.330741</td>
      <td>True</td>
      <td>sea_lion</td>
      <td>0.275645</td>
      <td>False</td>
      <td>Weimaraner</td>
      <td>0.134203</td>
      <td>True</td>
    </tr>
    <tr>
      <th>24</th>
      <td>31061</td>
      <td>887101392804085760</td>
      <td>6167</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/887101392...</td>
      <td>12</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE-eAq6UwAA-jaE.jpg</td>
      <td>Samoyed</td>
      <td>0.733942</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.035029</td>
      <td>True</td>
      <td>Staffordshire_bullterrier</td>
      <td>0.029705</td>
      <td>True</td>
    </tr>
    <tr>
      <th>25</th>
      <td>35859</td>
      <td>886983233522544640</td>
      <td>8084</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/886983233...</td>
      <td>13</td>
      <td>Maya</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE8yicJW0AAAvBJ.jpg</td>
      <td>Chihuahua</td>
      <td>0.793469</td>
      <td>True</td>
      <td>toy_terrier</td>
      <td>0.143528</td>
      <td>True</td>
      <td>can_opener</td>
      <td>0.032253</td>
      <td>False</td>
    </tr>
    <tr>
      <th>26</th>
      <td>12306</td>
      <td>886736880519319552</td>
      <td>3443</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://www.gofundme.com/mingusneedsus,https:/...</td>
      <td>13</td>
      <td>Mingus</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE5Se8FXcAAJFx4.jpg</td>
      <td>kuvasz</td>
      <td>0.309706</td>
      <td>True</td>
      <td>Great_Pyrenees</td>
      <td>0.186136</td>
      <td>True</td>
      <td>Dandie_Dinmont</td>
      <td>0.086346</td>
      <td>True</td>
    </tr>
    <tr>
      <th>27</th>
      <td>22798</td>
      <td>886680336477933568</td>
      <td>4610</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/886680336...</td>
      <td>13</td>
      <td>Derek</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE4fEDzWAAAyHMM.jpg</td>
      <td>convertible</td>
      <td>0.738995</td>
      <td>False</td>
      <td>sports_car</td>
      <td>0.139952</td>
      <td>False</td>
      <td>car_wheel</td>
      <td>0.044173</td>
      <td>False</td>
    </tr>
    <tr>
      <th>28</th>
      <td>21524</td>
      <td>886366144734445568</td>
      <td>3316</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/886366144...</td>
      <td>12</td>
      <td>Roscoe</td>
      <td>pupper</td>
      <td>https://pbs.twimg.com/media/DE0BTnQUwAApKEH.jpg</td>
      <td>French_bulldog</td>
      <td>0.999201</td>
      <td>True</td>
      <td>Chihuahua</td>
      <td>0.000361</td>
      <td>True</td>
      <td>Boston_bull</td>
      <td>0.000076</td>
      <td>True</td>
    </tr>
    <tr>
      <th>29</th>
      <td>28469</td>
      <td>886258384151887873</td>
      <td>6523</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/886258384...</td>
      <td>13</td>
      <td>Waffles</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DEyfTG4UMAE4aE9.jpg</td>
      <td>pug</td>
      <td>0.943575</td>
      <td>True</td>
      <td>shower_cap</td>
      <td>0.025286</td>
      <td>False</td>
      <td>Siamese_cat</td>
      <td>0.002849</td>
      <td>False</td>
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
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2043</th>
      <td>459</td>
      <td>666411507551481857</td>
      <td>339</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666411507...</td>
      <td>2</td>
      <td>quite</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT-RugiWIAELEaq.jpg</td>
      <td>coho</td>
      <td>0.404640</td>
      <td>False</td>
      <td>barracouta</td>
      <td>0.271485</td>
      <td>False</td>
      <td>gar</td>
      <td>0.189945</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2044</th>
      <td>113</td>
      <td>666407126856765440</td>
      <td>44</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666407126...</td>
      <td>7</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT-NvwmW4AAugGZ.jpg</td>
      <td>black-and-tan_coonhound</td>
      <td>0.529139</td>
      <td>True</td>
      <td>bloodhound</td>
      <td>0.244220</td>
      <td>True</td>
      <td>flat-coated_retriever</td>
      <td>0.173810</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2045</th>
      <td>172</td>
      <td>666396247373291520</td>
      <td>92</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666396247...</td>
      <td>9</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT-D2ZHWIAA3gK1.jpg</td>
      <td>Chihuahua</td>
      <td>0.978108</td>
      <td>True</td>
      <td>toy_terrier</td>
      <td>0.009397</td>
      <td>True</td>
      <td>papillon</td>
      <td>0.004577</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2046</th>
      <td>194</td>
      <td>666373753744588802</td>
      <td>100</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666373753...</td>
      <td>11</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9vZEYWUAAlZ05.jpg</td>
      <td>soft-coated_wheaten_terrier</td>
      <td>0.326467</td>
      <td>True</td>
      <td>Afghan_hound</td>
      <td>0.259551</td>
      <td>True</td>
      <td>briard</td>
      <td>0.206803</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2047</th>
      <td>804</td>
      <td>666362758909284353</td>
      <td>595</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666362758...</td>
      <td>6</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9lXGsUcAAyUFt.jpg</td>
      <td>guinea_pig</td>
      <td>0.996496</td>
      <td>False</td>
      <td>skunk</td>
      <td>0.002402</td>
      <td>False</td>
      <td>hamster</td>
      <td>0.000461</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2048</th>
      <td>229</td>
      <td>666353288456101888</td>
      <td>77</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666353288...</td>
      <td>8</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9cx0tUEAAhNN_.jpg</td>
      <td>malamute</td>
      <td>0.336874</td>
      <td>True</td>
      <td>Siberian_husky</td>
      <td>0.147655</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.093412</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2049</th>
      <td>307</td>
      <td>666345417576210432</td>
      <td>146</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666345417...</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9Vn7PWoAA_ZCM.jpg</td>
      <td>golden_retriever</td>
      <td>0.858744</td>
      <td>True</td>
      <td>Chesapeake_Bay_retriever</td>
      <td>0.054787</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.014241</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2050</th>
      <td>204</td>
      <td>666337882303524864</td>
      <td>96</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666337882...</td>
      <td>9</td>
      <td>an</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9OwFIWEAMuRje.jpg</td>
      <td>ox</td>
      <td>0.416669</td>
      <td>False</td>
      <td>Newfoundland</td>
      <td>0.278407</td>
      <td>True</td>
      <td>groenendael</td>
      <td>0.102643</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2051</th>
      <td>522</td>
      <td>666293911632134144</td>
      <td>368</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666293911...</td>
      <td>3</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8mx7KW4AEQu8N.jpg</td>
      <td>three-toed_sloth</td>
      <td>0.914671</td>
      <td>False</td>
      <td>otter</td>
      <td>0.015250</td>
      <td>False</td>
      <td>great_grey_owl</td>
      <td>0.013207</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2052</th>
      <td>152</td>
      <td>666287406224695296</td>
      <td>71</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666287406...</td>
      <td>1</td>
      <td>an</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8g3BpUEAAuFjg.jpg</td>
      <td>Maltese_dog</td>
      <td>0.857531</td>
      <td>True</td>
      <td>toy_poodle</td>
      <td>0.063064</td>
      <td>True</td>
      <td>miniature_poodle</td>
      <td>0.025581</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2053</th>
      <td>184</td>
      <td>666273097616637952</td>
      <td>82</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666273097...</td>
      <td>11</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8T1mtUwAA3aqm.jpg</td>
      <td>Italian_greyhound</td>
      <td>0.176053</td>
      <td>True</td>
      <td>toy_terrier</td>
      <td>0.111884</td>
      <td>True</td>
      <td>basenji</td>
      <td>0.111152</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2054</th>
      <td>108</td>
      <td>666268910803644416</td>
      <td>37</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666268910...</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8QCd1WEAADXws.jpg</td>
      <td>desktop_computer</td>
      <td>0.086502</td>
      <td>False</td>
      <td>desk</td>
      <td>0.085547</td>
      <td>False</td>
      <td>bookcase</td>
      <td>0.079480</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2055</th>
      <td>14765</td>
      <td>666104133288665088</td>
      <td>6871</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666104133...</td>
      <td>1</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT56LSZWoAAlJj2.jpg</td>
      <td>hen</td>
      <td>0.965932</td>
      <td>False</td>
      <td>cock</td>
      <td>0.033919</td>
      <td>False</td>
      <td>partridge</td>
      <td>0.000052</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2056</th>
      <td>81</td>
      <td>666102155909144576</td>
      <td>16</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666102155...</td>
      <td>11</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT54YGiWUAEZnoK.jpg</td>
      <td>English_setter</td>
      <td>0.298617</td>
      <td>True</td>
      <td>Newfoundland</td>
      <td>0.149842</td>
      <td>True</td>
      <td>borzoi</td>
      <td>0.133649</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2057</th>
      <td>164</td>
      <td>666099513787052032</td>
      <td>73</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666099513...</td>
      <td>8</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT51-JJUEAA6hV8.jpg</td>
      <td>Lhasa</td>
      <td>0.582330</td>
      <td>True</td>
      <td>Shih-Tzu</td>
      <td>0.166192</td>
      <td>True</td>
      <td>Dandie_Dinmont</td>
      <td>0.089688</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2058</th>
      <td>169</td>
      <td>666094000022159362</td>
      <td>79</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666094000...</td>
      <td>9</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5w9gUW4AAsBNN.jpg</td>
      <td>bloodhound</td>
      <td>0.195217</td>
      <td>True</td>
      <td>German_shepherd</td>
      <td>0.078260</td>
      <td>True</td>
      <td>malinois</td>
      <td>0.075628</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2059</th>
      <td>121</td>
      <td>666082916733198337</td>
      <td>47</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666082916...</td>
      <td>6</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5m4VGWEAAtKc8.jpg</td>
      <td>pug</td>
      <td>0.489814</td>
      <td>True</td>
      <td>bull_mastiff</td>
      <td>0.404722</td>
      <td>True</td>
      <td>French_bulldog</td>
      <td>0.048960</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2060</th>
      <td>335</td>
      <td>666073100786774016</td>
      <td>174</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666073100...</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5d9DZXAAALcwe.jpg</td>
      <td>Walker_hound</td>
      <td>0.260857</td>
      <td>True</td>
      <td>English_foxhound</td>
      <td>0.175382</td>
      <td>True</td>
      <td>Ibizan_hound</td>
      <td>0.097471</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2061</th>
      <td>154</td>
      <td>666071193221509120</td>
      <td>67</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666071193...</td>
      <td>9</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5cN_3WEAAlOoZ.jpg</td>
      <td>Gordon_setter</td>
      <td>0.503672</td>
      <td>True</td>
      <td>Yorkshire_terrier</td>
      <td>0.174201</td>
      <td>True</td>
      <td>Pekinese</td>
      <td>0.109454</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2062</th>
      <td>496</td>
      <td>666063827256086533</td>
      <td>232</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666063827...</td>
      <td>10</td>
      <td>the</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Vg_wXIAAXfnj.jpg</td>
      <td>golden_retriever</td>
      <td>0.775930</td>
      <td>True</td>
      <td>Tibetan_mastiff</td>
      <td>0.093718</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.072427</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2063</th>
      <td>115</td>
      <td>666058600524156928</td>
      <td>61</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666058600...</td>
      <td>8</td>
      <td>the</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Qw94XAAA_2dP.jpg</td>
      <td>miniature_poodle</td>
      <td>0.201493</td>
      <td>True</td>
      <td>komondor</td>
      <td>0.192305</td>
      <td>True</td>
      <td>soft-coated_wheaten_terrier</td>
      <td>0.082086</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2064</th>
      <td>304</td>
      <td>666057090499244032</td>
      <td>146</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666057090...</td>
      <td>9</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5PY90WoAAQGLo.jpg</td>
      <td>shopping_cart</td>
      <td>0.962465</td>
      <td>False</td>
      <td>shopping_basket</td>
      <td>0.014594</td>
      <td>False</td>
      <td>golden_retriever</td>
      <td>0.007959</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2065</th>
      <td>448</td>
      <td>666055525042405380</td>
      <td>261</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666055525...</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5N9tpXIAAifs1.jpg</td>
      <td>chow</td>
      <td>0.692517</td>
      <td>True</td>
      <td>Tibetan_mastiff</td>
      <td>0.058279</td>
      <td>True</td>
      <td>fur_coat</td>
      <td>0.054449</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2066</th>
      <td>1253</td>
      <td>666051853826850816</td>
      <td>879</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666051853...</td>
      <td>2</td>
      <td>an</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5KoJ1WoAAJash.jpg</td>
      <td>box_turtle</td>
      <td>0.933012</td>
      <td>False</td>
      <td>mud_turtle</td>
      <td>0.045885</td>
      <td>False</td>
      <td>terrapin</td>
      <td>0.017885</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2067</th>
      <td>136</td>
      <td>666050758794694657</td>
      <td>60</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666050758...</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Jof1WUAEuVxN.jpg</td>
      <td>Bernese_mountain_dog</td>
      <td>0.651137</td>
      <td>True</td>
      <td>English_springer</td>
      <td>0.263788</td>
      <td>True</td>
      <td>Greater_Swiss_Mountain_dog</td>
      <td>0.016199</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2068</th>
      <td>111</td>
      <td>666049248165822465</td>
      <td>41</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666049248...</td>
      <td>5</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5IQmsXIAAKY4A.jpg</td>
      <td>miniature_pinscher</td>
      <td>0.560311</td>
      <td>True</td>
      <td>Rottweiler</td>
      <td>0.243682</td>
      <td>True</td>
      <td>Doberman</td>
      <td>0.154629</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2069</th>
      <td>311</td>
      <td>666044226329800704</td>
      <td>147</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666044226...</td>
      <td>6</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Dr8HUEAA-lEu.jpg</td>
      <td>Rhodesian_ridgeback</td>
      <td>0.408143</td>
      <td>True</td>
      <td>redbone</td>
      <td>0.360687</td>
      <td>True</td>
      <td>miniature_pinscher</td>
      <td>0.222752</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2070</th>
      <td>128</td>
      <td>666033412701032449</td>
      <td>47</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666033412...</td>
      <td>9</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT4521TWwAEvMyu.jpg</td>
      <td>German_shepherd</td>
      <td>0.596461</td>
      <td>True</td>
      <td>malinois</td>
      <td>0.138584</td>
      <td>True</td>
      <td>bloodhound</td>
      <td>0.116197</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2071</th>
      <td>132</td>
      <td>666029285002620928</td>
      <td>48</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666029285...</td>
      <td>7</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT42GRgUYAA5iDo.jpg</td>
      <td>redbone</td>
      <td>0.506826</td>
      <td>True</td>
      <td>miniature_pinscher</td>
      <td>0.074192</td>
      <td>True</td>
      <td>Rhodesian_ridgeback</td>
      <td>0.072010</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2072</th>
      <td>2535</td>
      <td>666020888022790149</td>
      <td>532</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666020888...</td>
      <td>8</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT4udn0WwAA0aMy.jpg</td>
      <td>Welsh_springer_spaniel</td>
      <td>0.465074</td>
      <td>True</td>
      <td>collie</td>
      <td>0.156665</td>
      <td>True</td>
      <td>Shetland_sheepdog</td>
      <td>0.061428</td>
      <td>True</td>
    </tr>
  </tbody>
</table>
<p>2073 rows × 19 columns</p>
</div>



#### Test:


```python
# Check the new dataframe
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
      <th>favorite_count</th>
      <th>tweet_id</th>
      <th>retweet_count</th>
      <th>retweeted_status_id</th>
      <th>retweeted_status_user_id</th>
      <th>expanded_urls</th>
      <th>rating_numerator</th>
      <th>dog_name</th>
      <th>dog_type</th>
      <th>jpg_url</th>
      <th>p1</th>
      <th>p1_conf</th>
      <th>p1_dog</th>
      <th>p2</th>
      <th>p2_conf</th>
      <th>p2_dog</th>
      <th>p3</th>
      <th>p3_conf</th>
      <th>p3_dog</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>39467</td>
      <td>892420643555336193</td>
      <td>8853</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/892420643...</td>
      <td>13</td>
      <td>Phineas</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DGKD1-bXoAAIAUK.jpg</td>
      <td>orange</td>
      <td>0.097049</td>
      <td>False</td>
      <td>bagel</td>
      <td>0.085851</td>
      <td>False</td>
      <td>banana</td>
      <td>0.076110</td>
      <td>False</td>
    </tr>
    <tr>
      <th>1</th>
      <td>33819</td>
      <td>892177421306343426</td>
      <td>6514</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/892177421...</td>
      <td>13</td>
      <td>Tilly</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DGGmoV4XsAAUL6n.jpg</td>
      <td>Chihuahua</td>
      <td>0.323581</td>
      <td>True</td>
      <td>Pekinese</td>
      <td>0.090647</td>
      <td>True</td>
      <td>papillon</td>
      <td>0.068957</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2</th>
      <td>25461</td>
      <td>891815181378084864</td>
      <td>4328</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/891815181...</td>
      <td>12</td>
      <td>Archie</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DGBdLU1WsAANxJ9.jpg</td>
      <td>Chihuahua</td>
      <td>0.716012</td>
      <td>True</td>
      <td>malamute</td>
      <td>0.078253</td>
      <td>True</td>
      <td>kelpie</td>
      <td>0.031379</td>
      <td>True</td>
    </tr>
    <tr>
      <th>3</th>
      <td>42908</td>
      <td>891689557279858688</td>
      <td>8964</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/891689557...</td>
      <td>13</td>
      <td>Darla</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF_q7IAWsAEuuN8.jpg</td>
      <td>paper_towel</td>
      <td>0.170278</td>
      <td>False</td>
      <td>Labrador_retriever</td>
      <td>0.168086</td>
      <td>True</td>
      <td>spatula</td>
      <td>0.040836</td>
      <td>False</td>
    </tr>
    <tr>
      <th>4</th>
      <td>41048</td>
      <td>891327558926688256</td>
      <td>9774</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/891327558...</td>
      <td>12</td>
      <td>Franklin</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF6hr6BUMAAzZgT.jpg</td>
      <td>basset</td>
      <td>0.555712</td>
      <td>True</td>
      <td>English_springer</td>
      <td>0.225770</td>
      <td>True</td>
      <td>German_short-haired_pointer</td>
      <td>0.175219</td>
      <td>True</td>
    </tr>
    <tr>
      <th>5</th>
      <td>20562</td>
      <td>891087950875897856</td>
      <td>3261</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/891087950...</td>
      <td>13</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF3HwyEWsAABqE6.jpg</td>
      <td>Chesapeake_Bay_retriever</td>
      <td>0.425595</td>
      <td>True</td>
      <td>Irish_terrier</td>
      <td>0.116317</td>
      <td>True</td>
      <td>Indian_elephant</td>
      <td>0.076902</td>
      <td>False</td>
    </tr>
    <tr>
      <th>6</th>
      <td>12041</td>
      <td>890971913173991426</td>
      <td>2158</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://gofundme.com/ydvmve-surgery-for-jax,ht...</td>
      <td>13</td>
      <td>Jax</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF1eOmZXUAALUcq.jpg</td>
      <td>Appenzeller</td>
      <td>0.341703</td>
      <td>True</td>
      <td>Border_collie</td>
      <td>0.199287</td>
      <td>True</td>
      <td>ice_lolly</td>
      <td>0.193548</td>
      <td>False</td>
    </tr>
    <tr>
      <th>7</th>
      <td>56848</td>
      <td>890729181411237888</td>
      <td>16716</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/890729181...</td>
      <td>13</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFyBahAVwAAhUTd.jpg</td>
      <td>Pomeranian</td>
      <td>0.566142</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.178406</td>
      <td>True</td>
      <td>Pembroke</td>
      <td>0.076507</td>
      <td>True</td>
    </tr>
    <tr>
      <th>8</th>
      <td>28226</td>
      <td>890609185150312448</td>
      <td>4429</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/890609185...</td>
      <td>13</td>
      <td>Zoey</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFwUU__XcAEpyXI.jpg</td>
      <td>Irish_terrier</td>
      <td>0.487574</td>
      <td>True</td>
      <td>Irish_setter</td>
      <td>0.193054</td>
      <td>True</td>
      <td>Chesapeake_Bay_retriever</td>
      <td>0.118184</td>
      <td>True</td>
    </tr>
    <tr>
      <th>9</th>
      <td>32467</td>
      <td>890240255349198849</td>
      <td>7711</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/890240255...</td>
      <td>14</td>
      <td>Cassie</td>
      <td>doggo</td>
      <td>https://pbs.twimg.com/media/DFrEyVuW0AAO3t9.jpg</td>
      <td>Pembroke</td>
      <td>0.511319</td>
      <td>True</td>
      <td>Cardigan</td>
      <td>0.451038</td>
      <td>True</td>
      <td>Chihuahua</td>
      <td>0.029248</td>
      <td>True</td>
    </tr>
    <tr>
      <th>10</th>
      <td>31166</td>
      <td>890006608113172480</td>
      <td>7624</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/890006608...</td>
      <td>13</td>
      <td>Koda</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFnwSY4WAAAMliS.jpg</td>
      <td>Samoyed</td>
      <td>0.957979</td>
      <td>True</td>
      <td>Pomeranian</td>
      <td>0.013884</td>
      <td>True</td>
      <td>chow</td>
      <td>0.008167</td>
      <td>True</td>
    </tr>
    <tr>
      <th>11</th>
      <td>28268</td>
      <td>889880896479866881</td>
      <td>5156</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/889880896...</td>
      <td>13</td>
      <td>Bruno</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFl99B1WsAITKsg.jpg</td>
      <td>French_bulldog</td>
      <td>0.377417</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.151317</td>
      <td>True</td>
      <td>muzzle</td>
      <td>0.082981</td>
      <td>False</td>
    </tr>
    <tr>
      <th>12</th>
      <td>38818</td>
      <td>889665388333682689</td>
      <td>8538</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/889665388...</td>
      <td>13</td>
      <td>None</td>
      <td>puppo</td>
      <td>https://pbs.twimg.com/media/DFi579UWsAAatzw.jpg</td>
      <td>Pembroke</td>
      <td>0.966327</td>
      <td>True</td>
      <td>Cardigan</td>
      <td>0.027356</td>
      <td>True</td>
      <td>basenji</td>
      <td>0.004633</td>
      <td>True</td>
    </tr>
    <tr>
      <th>13</th>
      <td>27672</td>
      <td>889638837579907072</td>
      <td>4735</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/889638837...</td>
      <td>12</td>
      <td>Ted</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFihzFfXsAYGDPR.jpg</td>
      <td>French_bulldog</td>
      <td>0.991650</td>
      <td>True</td>
      <td>boxer</td>
      <td>0.002129</td>
      <td>True</td>
      <td>Staffordshire_bullterrier</td>
      <td>0.001498</td>
      <td>True</td>
    </tr>
    <tr>
      <th>14</th>
      <td>15359</td>
      <td>889531135344209921</td>
      <td>2321</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/889531135...</td>
      <td>13</td>
      <td>Stuart</td>
      <td>puppo</td>
      <td>https://pbs.twimg.com/media/DFg_2PVW0AEHN3p.jpg</td>
      <td>golden_retriever</td>
      <td>0.953442</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.013834</td>
      <td>True</td>
      <td>redbone</td>
      <td>0.007958</td>
      <td>True</td>
    </tr>
    <tr>
      <th>15</th>
      <td>25652</td>
      <td>889278841981685760</td>
      <td>5637</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/889278841...</td>
      <td>13</td>
      <td>Oliver</td>
      <td>None</td>
      <td>https://pbs.twimg.com/ext_tw_video_thumb/88927...</td>
      <td>whippet</td>
      <td>0.626152</td>
      <td>True</td>
      <td>borzoi</td>
      <td>0.194742</td>
      <td>True</td>
      <td>Saluki</td>
      <td>0.027351</td>
      <td>True</td>
    </tr>
    <tr>
      <th>16</th>
      <td>29611</td>
      <td>888917238123831296</td>
      <td>4709</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/888917238...</td>
      <td>12</td>
      <td>Jim</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFYRgsOUQAARGhO.jpg</td>
      <td>golden_retriever</td>
      <td>0.714719</td>
      <td>True</td>
      <td>Tibetan_mastiff</td>
      <td>0.120184</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.105506</td>
      <td>True</td>
    </tr>
    <tr>
      <th>17</th>
      <td>26080</td>
      <td>888804989199671297</td>
      <td>4559</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/888804989...</td>
      <td>13</td>
      <td>Zeke</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFWra-3VYAA2piG.jpg</td>
      <td>golden_retriever</td>
      <td>0.469760</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.184172</td>
      <td>True</td>
      <td>English_setter</td>
      <td>0.073482</td>
      <td>True</td>
    </tr>
    <tr>
      <th>18</th>
      <td>20290</td>
      <td>888554962724278272</td>
      <td>3732</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/888554962...</td>
      <td>13</td>
      <td>Ralphus</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFTH_O-UQAACu20.jpg</td>
      <td>Siberian_husky</td>
      <td>0.700377</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.166511</td>
      <td>True</td>
      <td>malamute</td>
      <td>0.111411</td>
      <td>True</td>
    </tr>
    <tr>
      <th>19</th>
      <td>22201</td>
      <td>888078434458587136</td>
      <td>3653</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/888078434...</td>
      <td>12</td>
      <td>Gerald</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFMWn56WsAAkA7B.jpg</td>
      <td>French_bulldog</td>
      <td>0.995026</td>
      <td>True</td>
      <td>pug</td>
      <td>0.000932</td>
      <td>True</td>
      <td>bull_mastiff</td>
      <td>0.000903</td>
      <td>True</td>
    </tr>
    <tr>
      <th>20</th>
      <td>30779</td>
      <td>887705289381826560</td>
      <td>5609</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/887705289...</td>
      <td>13</td>
      <td>Jeffrey</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFHDQBbXgAEqY7t.jpg</td>
      <td>basset</td>
      <td>0.821664</td>
      <td>True</td>
      <td>redbone</td>
      <td>0.087582</td>
      <td>True</td>
      <td>Weimaraner</td>
      <td>0.026236</td>
      <td>True</td>
    </tr>
    <tr>
      <th>21</th>
      <td>46959</td>
      <td>887517139158093824</td>
      <td>12082</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/887517139...</td>
      <td>14</td>
      <td>such</td>
      <td>None</td>
      <td>https://pbs.twimg.com/ext_tw_video_thumb/88751...</td>
      <td>limousine</td>
      <td>0.130432</td>
      <td>False</td>
      <td>tow_truck</td>
      <td>0.029175</td>
      <td>False</td>
      <td>shopping_cart</td>
      <td>0.026321</td>
      <td>False</td>
    </tr>
    <tr>
      <th>22</th>
      <td>69871</td>
      <td>887473957103951883</td>
      <td>18781</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/887473957...</td>
      <td>13</td>
      <td>Canela</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFDw2tyUQAAAFke.jpg</td>
      <td>Pembroke</td>
      <td>0.809197</td>
      <td>True</td>
      <td>Rhodesian_ridgeback</td>
      <td>0.054950</td>
      <td>True</td>
      <td>beagle</td>
      <td>0.038915</td>
      <td>True</td>
    </tr>
    <tr>
      <th>23</th>
      <td>34222</td>
      <td>887343217045368832</td>
      <td>10737</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/887343217...</td>
      <td>13</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/ext_tw_video_thumb/88734...</td>
      <td>Mexican_hairless</td>
      <td>0.330741</td>
      <td>True</td>
      <td>sea_lion</td>
      <td>0.275645</td>
      <td>False</td>
      <td>Weimaraner</td>
      <td>0.134203</td>
      <td>True</td>
    </tr>
    <tr>
      <th>24</th>
      <td>31061</td>
      <td>887101392804085760</td>
      <td>6167</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/887101392...</td>
      <td>12</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE-eAq6UwAA-jaE.jpg</td>
      <td>Samoyed</td>
      <td>0.733942</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.035029</td>
      <td>True</td>
      <td>Staffordshire_bullterrier</td>
      <td>0.029705</td>
      <td>True</td>
    </tr>
    <tr>
      <th>25</th>
      <td>35859</td>
      <td>886983233522544640</td>
      <td>8084</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/886983233...</td>
      <td>13</td>
      <td>Maya</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE8yicJW0AAAvBJ.jpg</td>
      <td>Chihuahua</td>
      <td>0.793469</td>
      <td>True</td>
      <td>toy_terrier</td>
      <td>0.143528</td>
      <td>True</td>
      <td>can_opener</td>
      <td>0.032253</td>
      <td>False</td>
    </tr>
    <tr>
      <th>26</th>
      <td>12306</td>
      <td>886736880519319552</td>
      <td>3443</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://www.gofundme.com/mingusneedsus,https:/...</td>
      <td>13</td>
      <td>Mingus</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE5Se8FXcAAJFx4.jpg</td>
      <td>kuvasz</td>
      <td>0.309706</td>
      <td>True</td>
      <td>Great_Pyrenees</td>
      <td>0.186136</td>
      <td>True</td>
      <td>Dandie_Dinmont</td>
      <td>0.086346</td>
      <td>True</td>
    </tr>
    <tr>
      <th>27</th>
      <td>22798</td>
      <td>886680336477933568</td>
      <td>4610</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/886680336...</td>
      <td>13</td>
      <td>Derek</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE4fEDzWAAAyHMM.jpg</td>
      <td>convertible</td>
      <td>0.738995</td>
      <td>False</td>
      <td>sports_car</td>
      <td>0.139952</td>
      <td>False</td>
      <td>car_wheel</td>
      <td>0.044173</td>
      <td>False</td>
    </tr>
    <tr>
      <th>28</th>
      <td>21524</td>
      <td>886366144734445568</td>
      <td>3316</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/886366144...</td>
      <td>12</td>
      <td>Roscoe</td>
      <td>pupper</td>
      <td>https://pbs.twimg.com/media/DE0BTnQUwAApKEH.jpg</td>
      <td>French_bulldog</td>
      <td>0.999201</td>
      <td>True</td>
      <td>Chihuahua</td>
      <td>0.000361</td>
      <td>True</td>
      <td>Boston_bull</td>
      <td>0.000076</td>
      <td>True</td>
    </tr>
    <tr>
      <th>29</th>
      <td>28469</td>
      <td>886258384151887873</td>
      <td>6523</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/886258384...</td>
      <td>13</td>
      <td>Waffles</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DEyfTG4UMAE4aE9.jpg</td>
      <td>pug</td>
      <td>0.943575</td>
      <td>True</td>
      <td>shower_cap</td>
      <td>0.025286</td>
      <td>False</td>
      <td>Siamese_cat</td>
      <td>0.002849</td>
      <td>False</td>
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
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2043</th>
      <td>459</td>
      <td>666411507551481857</td>
      <td>339</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666411507...</td>
      <td>2</td>
      <td>quite</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT-RugiWIAELEaq.jpg</td>
      <td>coho</td>
      <td>0.404640</td>
      <td>False</td>
      <td>barracouta</td>
      <td>0.271485</td>
      <td>False</td>
      <td>gar</td>
      <td>0.189945</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2044</th>
      <td>113</td>
      <td>666407126856765440</td>
      <td>44</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666407126...</td>
      <td>7</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT-NvwmW4AAugGZ.jpg</td>
      <td>black-and-tan_coonhound</td>
      <td>0.529139</td>
      <td>True</td>
      <td>bloodhound</td>
      <td>0.244220</td>
      <td>True</td>
      <td>flat-coated_retriever</td>
      <td>0.173810</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2045</th>
      <td>172</td>
      <td>666396247373291520</td>
      <td>92</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666396247...</td>
      <td>9</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT-D2ZHWIAA3gK1.jpg</td>
      <td>Chihuahua</td>
      <td>0.978108</td>
      <td>True</td>
      <td>toy_terrier</td>
      <td>0.009397</td>
      <td>True</td>
      <td>papillon</td>
      <td>0.004577</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2046</th>
      <td>194</td>
      <td>666373753744588802</td>
      <td>100</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666373753...</td>
      <td>11</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9vZEYWUAAlZ05.jpg</td>
      <td>soft-coated_wheaten_terrier</td>
      <td>0.326467</td>
      <td>True</td>
      <td>Afghan_hound</td>
      <td>0.259551</td>
      <td>True</td>
      <td>briard</td>
      <td>0.206803</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2047</th>
      <td>804</td>
      <td>666362758909284353</td>
      <td>595</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666362758...</td>
      <td>6</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9lXGsUcAAyUFt.jpg</td>
      <td>guinea_pig</td>
      <td>0.996496</td>
      <td>False</td>
      <td>skunk</td>
      <td>0.002402</td>
      <td>False</td>
      <td>hamster</td>
      <td>0.000461</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2048</th>
      <td>229</td>
      <td>666353288456101888</td>
      <td>77</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666353288...</td>
      <td>8</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9cx0tUEAAhNN_.jpg</td>
      <td>malamute</td>
      <td>0.336874</td>
      <td>True</td>
      <td>Siberian_husky</td>
      <td>0.147655</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.093412</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2049</th>
      <td>307</td>
      <td>666345417576210432</td>
      <td>146</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666345417...</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9Vn7PWoAA_ZCM.jpg</td>
      <td>golden_retriever</td>
      <td>0.858744</td>
      <td>True</td>
      <td>Chesapeake_Bay_retriever</td>
      <td>0.054787</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.014241</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2050</th>
      <td>204</td>
      <td>666337882303524864</td>
      <td>96</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666337882...</td>
      <td>9</td>
      <td>an</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9OwFIWEAMuRje.jpg</td>
      <td>ox</td>
      <td>0.416669</td>
      <td>False</td>
      <td>Newfoundland</td>
      <td>0.278407</td>
      <td>True</td>
      <td>groenendael</td>
      <td>0.102643</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2051</th>
      <td>522</td>
      <td>666293911632134144</td>
      <td>368</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666293911...</td>
      <td>3</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8mx7KW4AEQu8N.jpg</td>
      <td>three-toed_sloth</td>
      <td>0.914671</td>
      <td>False</td>
      <td>otter</td>
      <td>0.015250</td>
      <td>False</td>
      <td>great_grey_owl</td>
      <td>0.013207</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2052</th>
      <td>152</td>
      <td>666287406224695296</td>
      <td>71</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666287406...</td>
      <td>1</td>
      <td>an</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8g3BpUEAAuFjg.jpg</td>
      <td>Maltese_dog</td>
      <td>0.857531</td>
      <td>True</td>
      <td>toy_poodle</td>
      <td>0.063064</td>
      <td>True</td>
      <td>miniature_poodle</td>
      <td>0.025581</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2053</th>
      <td>184</td>
      <td>666273097616637952</td>
      <td>82</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666273097...</td>
      <td>11</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8T1mtUwAA3aqm.jpg</td>
      <td>Italian_greyhound</td>
      <td>0.176053</td>
      <td>True</td>
      <td>toy_terrier</td>
      <td>0.111884</td>
      <td>True</td>
      <td>basenji</td>
      <td>0.111152</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2054</th>
      <td>108</td>
      <td>666268910803644416</td>
      <td>37</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666268910...</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8QCd1WEAADXws.jpg</td>
      <td>desktop_computer</td>
      <td>0.086502</td>
      <td>False</td>
      <td>desk</td>
      <td>0.085547</td>
      <td>False</td>
      <td>bookcase</td>
      <td>0.079480</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2055</th>
      <td>14765</td>
      <td>666104133288665088</td>
      <td>6871</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666104133...</td>
      <td>1</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT56LSZWoAAlJj2.jpg</td>
      <td>hen</td>
      <td>0.965932</td>
      <td>False</td>
      <td>cock</td>
      <td>0.033919</td>
      <td>False</td>
      <td>partridge</td>
      <td>0.000052</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2056</th>
      <td>81</td>
      <td>666102155909144576</td>
      <td>16</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666102155...</td>
      <td>11</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT54YGiWUAEZnoK.jpg</td>
      <td>English_setter</td>
      <td>0.298617</td>
      <td>True</td>
      <td>Newfoundland</td>
      <td>0.149842</td>
      <td>True</td>
      <td>borzoi</td>
      <td>0.133649</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2057</th>
      <td>164</td>
      <td>666099513787052032</td>
      <td>73</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666099513...</td>
      <td>8</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT51-JJUEAA6hV8.jpg</td>
      <td>Lhasa</td>
      <td>0.582330</td>
      <td>True</td>
      <td>Shih-Tzu</td>
      <td>0.166192</td>
      <td>True</td>
      <td>Dandie_Dinmont</td>
      <td>0.089688</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2058</th>
      <td>169</td>
      <td>666094000022159362</td>
      <td>79</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666094000...</td>
      <td>9</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5w9gUW4AAsBNN.jpg</td>
      <td>bloodhound</td>
      <td>0.195217</td>
      <td>True</td>
      <td>German_shepherd</td>
      <td>0.078260</td>
      <td>True</td>
      <td>malinois</td>
      <td>0.075628</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2059</th>
      <td>121</td>
      <td>666082916733198337</td>
      <td>47</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666082916...</td>
      <td>6</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5m4VGWEAAtKc8.jpg</td>
      <td>pug</td>
      <td>0.489814</td>
      <td>True</td>
      <td>bull_mastiff</td>
      <td>0.404722</td>
      <td>True</td>
      <td>French_bulldog</td>
      <td>0.048960</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2060</th>
      <td>335</td>
      <td>666073100786774016</td>
      <td>174</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666073100...</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5d9DZXAAALcwe.jpg</td>
      <td>Walker_hound</td>
      <td>0.260857</td>
      <td>True</td>
      <td>English_foxhound</td>
      <td>0.175382</td>
      <td>True</td>
      <td>Ibizan_hound</td>
      <td>0.097471</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2061</th>
      <td>154</td>
      <td>666071193221509120</td>
      <td>67</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666071193...</td>
      <td>9</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5cN_3WEAAlOoZ.jpg</td>
      <td>Gordon_setter</td>
      <td>0.503672</td>
      <td>True</td>
      <td>Yorkshire_terrier</td>
      <td>0.174201</td>
      <td>True</td>
      <td>Pekinese</td>
      <td>0.109454</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2062</th>
      <td>496</td>
      <td>666063827256086533</td>
      <td>232</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666063827...</td>
      <td>10</td>
      <td>the</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Vg_wXIAAXfnj.jpg</td>
      <td>golden_retriever</td>
      <td>0.775930</td>
      <td>True</td>
      <td>Tibetan_mastiff</td>
      <td>0.093718</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.072427</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2063</th>
      <td>115</td>
      <td>666058600524156928</td>
      <td>61</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666058600...</td>
      <td>8</td>
      <td>the</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Qw94XAAA_2dP.jpg</td>
      <td>miniature_poodle</td>
      <td>0.201493</td>
      <td>True</td>
      <td>komondor</td>
      <td>0.192305</td>
      <td>True</td>
      <td>soft-coated_wheaten_terrier</td>
      <td>0.082086</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2064</th>
      <td>304</td>
      <td>666057090499244032</td>
      <td>146</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666057090...</td>
      <td>9</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5PY90WoAAQGLo.jpg</td>
      <td>shopping_cart</td>
      <td>0.962465</td>
      <td>False</td>
      <td>shopping_basket</td>
      <td>0.014594</td>
      <td>False</td>
      <td>golden_retriever</td>
      <td>0.007959</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2065</th>
      <td>448</td>
      <td>666055525042405380</td>
      <td>261</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666055525...</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5N9tpXIAAifs1.jpg</td>
      <td>chow</td>
      <td>0.692517</td>
      <td>True</td>
      <td>Tibetan_mastiff</td>
      <td>0.058279</td>
      <td>True</td>
      <td>fur_coat</td>
      <td>0.054449</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2066</th>
      <td>1253</td>
      <td>666051853826850816</td>
      <td>879</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666051853...</td>
      <td>2</td>
      <td>an</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5KoJ1WoAAJash.jpg</td>
      <td>box_turtle</td>
      <td>0.933012</td>
      <td>False</td>
      <td>mud_turtle</td>
      <td>0.045885</td>
      <td>False</td>
      <td>terrapin</td>
      <td>0.017885</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2067</th>
      <td>136</td>
      <td>666050758794694657</td>
      <td>60</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666050758...</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Jof1WUAEuVxN.jpg</td>
      <td>Bernese_mountain_dog</td>
      <td>0.651137</td>
      <td>True</td>
      <td>English_springer</td>
      <td>0.263788</td>
      <td>True</td>
      <td>Greater_Swiss_Mountain_dog</td>
      <td>0.016199</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2068</th>
      <td>111</td>
      <td>666049248165822465</td>
      <td>41</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666049248...</td>
      <td>5</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5IQmsXIAAKY4A.jpg</td>
      <td>miniature_pinscher</td>
      <td>0.560311</td>
      <td>True</td>
      <td>Rottweiler</td>
      <td>0.243682</td>
      <td>True</td>
      <td>Doberman</td>
      <td>0.154629</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2069</th>
      <td>311</td>
      <td>666044226329800704</td>
      <td>147</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666044226...</td>
      <td>6</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Dr8HUEAA-lEu.jpg</td>
      <td>Rhodesian_ridgeback</td>
      <td>0.408143</td>
      <td>True</td>
      <td>redbone</td>
      <td>0.360687</td>
      <td>True</td>
      <td>miniature_pinscher</td>
      <td>0.222752</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2070</th>
      <td>128</td>
      <td>666033412701032449</td>
      <td>47</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666033412...</td>
      <td>9</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT4521TWwAEvMyu.jpg</td>
      <td>German_shepherd</td>
      <td>0.596461</td>
      <td>True</td>
      <td>malinois</td>
      <td>0.138584</td>
      <td>True</td>
      <td>bloodhound</td>
      <td>0.116197</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2071</th>
      <td>132</td>
      <td>666029285002620928</td>
      <td>48</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666029285...</td>
      <td>7</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT42GRgUYAA5iDo.jpg</td>
      <td>redbone</td>
      <td>0.506826</td>
      <td>True</td>
      <td>miniature_pinscher</td>
      <td>0.074192</td>
      <td>True</td>
      <td>Rhodesian_ridgeback</td>
      <td>0.072010</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2072</th>
      <td>2535</td>
      <td>666020888022790149</td>
      <td>532</td>
      <td>nan</td>
      <td>nan</td>
      <td>https://twitter.com/dog_rates/status/666020888...</td>
      <td>8</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT4udn0WwAA0aMy.jpg</td>
      <td>Welsh_springer_spaniel</td>
      <td>0.465074</td>
      <td>True</td>
      <td>collie</td>
      <td>0.156665</td>
      <td>True</td>
      <td>Shetland_sheepdog</td>
      <td>0.061428</td>
      <td>True</td>
    </tr>
  </tbody>
</table>
<p>2073 rows × 19 columns</p>
</div>




```python

```

    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 2073 entries, 0 to 2072
    Data columns (total 19 columns):
    favorite_count              2073 non-null int64
    tweet_id                    2073 non-null int64
    retweet_count               2073 non-null int64
    retweeted_status_id         2073 non-null object
    retweeted_status_user_id    2073 non-null object
    expanded_urls               2073 non-null object
    rating_denominator          2073 non-null int64
    dog_name                    2073 non-null object
    dog_type                    2073 non-null object
    jpg_url                     2073 non-null object
    p1                          2073 non-null object
    p1_conf                     2073 non-null float64
    p1_dog                      2073 non-null bool
    p2                          2073 non-null object
    p2_conf                     2073 non-null float64
    p2_dog                      2073 non-null bool
    p3                          2073 non-null object
    p3_conf                     2073 non-null float64
    p3_dog                      2073 non-null bool
    dtypes: bool(3), float64(3), int64(4), object(9)
    memory usage: 281.4+ KB


## 3.5- More cleaning:

#### Define:

Change the names of undescriptive columns

#### Code:


```python
# list the columns names
```




    Index(['favorite_count', 'tweet_id', 'retweet_count', 'retweeted_status_id',
           'retweeted_status_user_id', 'expanded_urls', 'rating_numerator',
           'dog_name', 'dog_type', 'jpg_url', 'p1', 'p1_conf', 'p1_dog', 'p2',
           'p2_conf', 'p2_dog', 'p3', 'p3_conf', 'p3_dog'],
          dtype='object')




```python
# rename the columns
twitter_archive_master = twitter_archive_master.rename(columns={'p1': 'dog_1_propsed_type', 'p1_conf': 'dog_1_prediction_conformance_percent', 'p1_dog': 'dog_1_prediction_result', 'p2': 'dog_2_propsed_type',
       'p2_conf': 'dog_2_prediction_conformance_percent', 'p2_dog': 'dog_2_prediction_result', 'p3': 'dog_3_propsed_type', 'p3_conf': 'dog_3_prediction_conformance_percent', 'p3_dog': 'dog_3_prediction_result'})
```

#### Test:


```python

```

    <class 'pandas.core.frame.DataFrame'>
    Int64Index: 2073 entries, 0 to 2072
    Data columns (total 19 columns):
    favorite_count                          2073 non-null int64
    tweet_id                                2073 non-null int64
    retweet_count                           2073 non-null int64
    retweeted_status_id                     2073 non-null object
    retweeted_status_user_id                2073 non-null object
    expanded_urls                           2073 non-null object
    rating_numerator                        2073 non-null int64
    dog_name                                2073 non-null object
    dog_type                                2073 non-null object
    jpg_url                                 2073 non-null object
    dog_1_propsed_type                      2073 non-null object
    dog_1_prediction_conformance_percent    2073 non-null float64
    dog_1_prediction_result                 2073 non-null bool
    dog_2_propsed_type                      2073 non-null object
    dog_2_prediction_conformance_percent    2073 non-null float64
    dog_2_prediction_result                 2073 non-null bool
    dog_3_propsed_type                      2073 non-null object
    dog_3_prediction_conformance_percent    2073 non-null float64
    dog_3_prediction_result                 2073 non-null bool
    dtypes: bool(3), float64(3), int64(4), object(9)
    memory usage: 281.4+ KB


#### Define:

make the tweet_id column the first one

https://www.kite.com/python/answers/how-to-reorder-columns-in-a-pandas-dataframe-in-python

#### Code:


```python
# list columns
```




    Index(['favorite_count', 'tweet_id', 'retweet_count', 'retweeted_status_id',
           'retweeted_status_user_id', 'expanded_urls', 'rating_numerator',
           'dog_name', 'dog_type', 'jpg_url', 'dog_1_propsed_type',
           'dog_1_prediction_conformance_percent', 'dog_1_prediction_result',
           'dog_2_propsed_type', 'dog_2_prediction_conformance_percent',
           'dog_2_prediction_result', 'dog_3_propsed_type',
           'dog_3_prediction_conformance_percent', 'dog_3_prediction_result'],
          dtype='object')




```python
# make tweet_id column the first
```

#### Test:


```python

```




    Index(['tweet_id', 'favorite_count', 'retweet_count', 'retweeted_status_id',
           'retweeted_status_user_id', 'expanded_urls', 'rating_numerator',
           'dog_name', 'dog_type', 'jpg_url', 'dog_1_propsed_type',
           'dog_1_prediction_conformance_percent', 'dog_1_prediction_result',
           'dog_2_propsed_type', 'dog_2_prediction_conformance_percent',
           'dog_2_prediction_result', 'dog_3_propsed_type',
           'dog_3_prediction_conformance_percent', 'dog_3_prediction_result'],
          dtype='object')



#### Define:

Check the follwing columns, and remove them if they are with no use:
retweeted_status_id
retweeted_status_user_id

#### Code: 


```python
# Check retweeted_status_id
```




    nan                      1994
    7.902771173469757e+17       1
    8.224890570873897e+17       1
    7.69940425801171e+17        1
    7.804657092979958e+17       1
    7.829691400091075e+17       1
    7.395440793195889e+17       1
    8.001414224018309e+17       1
    7.258422890467492e+17       1
    7.012147008817562e+17       1
    8.071068405092147e+17       1
    8.29374341691347e+17        1
    6.718968093007094e+17       1
    7.119982797733478e+17       1
    8.609144852504699e+17       1
    8.174238601360835e+17       1
    7.575971410995487e+17       1
    6.798284471878574e+17       1
    7.750851326004429e+17       1
    8.392899192982241e+17       1
    7.116947884295537e+17       1
    7.638375655647805e+17       1
    8.159660734094336e+17       1
    7.90946055508652e+17        1
    6.67509364010451e+17        1
    7.961497490868756e+17       1
    8.650134204453683e+17       1
    8.3890598062882e+17         1
    6.75354435921576e+17        1
    7.761133056561889e+17       1
                             ... 
    7.932864763017994e+17       1
    7.128090259859784e+17       1
    7.833346399853896e+17       1
    7.776842335402066e+17       1
    8.305833205850685e+17       1
    7.916723228476375e+17       1
    8.06629075125203e+17        1
    8.688803978194944e+17       1
    7.33109485275861e+17        1
    6.790626142704681e+17       1
    7.93962221541933e+17        1
    7.895308770133934e+17       1
    8.47971000004354e+17        1
    7.950767302853919e+17       1
    7.806013036177326e+17       1
    8.222448165201551e+17       1
    7.848260202937098e+17       1
    7.50429297815552e+17        1
    6.703191306214359e+17       1
    7.652220986336911e+17       1
    6.791583739888763e+17       1
    6.675486956640707e+17       1
    6.67548415174144e+17        1
    7.076109487234785e+17       1
    6.853251128501248e+17       1
    7.887659149929021e+17       1
    7.735475969965711e+17       1
    7.790560957887529e+17       1
    7.424231704734638e+17       1
    7.827225987907256e+17       1
    Name: retweeted_status_id, Length: 80, dtype: int64




```python
# Check retweeted_status_user_id
```




    nan                      1994
    4196983835.0               65
    4296831739.0                2
    341021133.0                 1
    512804507.0                 1
    7.874617784352891e+17       1
    363890752.0                 1
    811740824.0                 1
    487197737.0                 1
    726634734.0                 1
    783214.0                    1
    280479778.0                 1
    1228325660.0                1
    41198418.0                  1
    597064155.0                 1
    Name: retweeted_status_user_id, dtype: int64




```python

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
      <th>tweet_id</th>
      <th>favorite_count</th>
      <th>retweet_count</th>
      <th>expanded_urls</th>
      <th>rating_numerator</th>
      <th>dog_name</th>
      <th>dog_type</th>
      <th>jpg_url</th>
      <th>dog_1_propsed_type</th>
      <th>dog_1_prediction_conformance_percent</th>
      <th>dog_1_prediction_result</th>
      <th>dog_2_propsed_type</th>
      <th>dog_2_prediction_conformance_percent</th>
      <th>dog_2_prediction_result</th>
      <th>dog_3_propsed_type</th>
      <th>dog_3_prediction_conformance_percent</th>
      <th>dog_3_prediction_result</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>892420643555336193</td>
      <td>39467</td>
      <td>8853</td>
      <td>https://twitter.com/dog_rates/status/892420643...</td>
      <td>13</td>
      <td>Phineas</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DGKD1-bXoAAIAUK.jpg</td>
      <td>orange</td>
      <td>0.097049</td>
      <td>False</td>
      <td>bagel</td>
      <td>0.085851</td>
      <td>False</td>
      <td>banana</td>
      <td>0.076110</td>
      <td>False</td>
    </tr>
    <tr>
      <th>1</th>
      <td>892177421306343426</td>
      <td>33819</td>
      <td>6514</td>
      <td>https://twitter.com/dog_rates/status/892177421...</td>
      <td>13</td>
      <td>Tilly</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DGGmoV4XsAAUL6n.jpg</td>
      <td>Chihuahua</td>
      <td>0.323581</td>
      <td>True</td>
      <td>Pekinese</td>
      <td>0.090647</td>
      <td>True</td>
      <td>papillon</td>
      <td>0.068957</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2</th>
      <td>891815181378084864</td>
      <td>25461</td>
      <td>4328</td>
      <td>https://twitter.com/dog_rates/status/891815181...</td>
      <td>12</td>
      <td>Archie</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DGBdLU1WsAANxJ9.jpg</td>
      <td>Chihuahua</td>
      <td>0.716012</td>
      <td>True</td>
      <td>malamute</td>
      <td>0.078253</td>
      <td>True</td>
      <td>kelpie</td>
      <td>0.031379</td>
      <td>True</td>
    </tr>
    <tr>
      <th>3</th>
      <td>891689557279858688</td>
      <td>42908</td>
      <td>8964</td>
      <td>https://twitter.com/dog_rates/status/891689557...</td>
      <td>13</td>
      <td>Darla</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF_q7IAWsAEuuN8.jpg</td>
      <td>paper_towel</td>
      <td>0.170278</td>
      <td>False</td>
      <td>Labrador_retriever</td>
      <td>0.168086</td>
      <td>True</td>
      <td>spatula</td>
      <td>0.040836</td>
      <td>False</td>
    </tr>
    <tr>
      <th>4</th>
      <td>891327558926688256</td>
      <td>41048</td>
      <td>9774</td>
      <td>https://twitter.com/dog_rates/status/891327558...</td>
      <td>12</td>
      <td>Franklin</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF6hr6BUMAAzZgT.jpg</td>
      <td>basset</td>
      <td>0.555712</td>
      <td>True</td>
      <td>English_springer</td>
      <td>0.225770</td>
      <td>True</td>
      <td>German_short-haired_pointer</td>
      <td>0.175219</td>
      <td>True</td>
    </tr>
    <tr>
      <th>5</th>
      <td>891087950875897856</td>
      <td>20562</td>
      <td>3261</td>
      <td>https://twitter.com/dog_rates/status/891087950...</td>
      <td>13</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF3HwyEWsAABqE6.jpg</td>
      <td>Chesapeake_Bay_retriever</td>
      <td>0.425595</td>
      <td>True</td>
      <td>Irish_terrier</td>
      <td>0.116317</td>
      <td>True</td>
      <td>Indian_elephant</td>
      <td>0.076902</td>
      <td>False</td>
    </tr>
    <tr>
      <th>6</th>
      <td>890971913173991426</td>
      <td>12041</td>
      <td>2158</td>
      <td>https://gofundme.com/ydvmve-surgery-for-jax,ht...</td>
      <td>13</td>
      <td>Jax</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DF1eOmZXUAALUcq.jpg</td>
      <td>Appenzeller</td>
      <td>0.341703</td>
      <td>True</td>
      <td>Border_collie</td>
      <td>0.199287</td>
      <td>True</td>
      <td>ice_lolly</td>
      <td>0.193548</td>
      <td>False</td>
    </tr>
    <tr>
      <th>7</th>
      <td>890729181411237888</td>
      <td>56848</td>
      <td>16716</td>
      <td>https://twitter.com/dog_rates/status/890729181...</td>
      <td>13</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFyBahAVwAAhUTd.jpg</td>
      <td>Pomeranian</td>
      <td>0.566142</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.178406</td>
      <td>True</td>
      <td>Pembroke</td>
      <td>0.076507</td>
      <td>True</td>
    </tr>
    <tr>
      <th>8</th>
      <td>890609185150312448</td>
      <td>28226</td>
      <td>4429</td>
      <td>https://twitter.com/dog_rates/status/890609185...</td>
      <td>13</td>
      <td>Zoey</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFwUU__XcAEpyXI.jpg</td>
      <td>Irish_terrier</td>
      <td>0.487574</td>
      <td>True</td>
      <td>Irish_setter</td>
      <td>0.193054</td>
      <td>True</td>
      <td>Chesapeake_Bay_retriever</td>
      <td>0.118184</td>
      <td>True</td>
    </tr>
    <tr>
      <th>9</th>
      <td>890240255349198849</td>
      <td>32467</td>
      <td>7711</td>
      <td>https://twitter.com/dog_rates/status/890240255...</td>
      <td>14</td>
      <td>Cassie</td>
      <td>doggo</td>
      <td>https://pbs.twimg.com/media/DFrEyVuW0AAO3t9.jpg</td>
      <td>Pembroke</td>
      <td>0.511319</td>
      <td>True</td>
      <td>Cardigan</td>
      <td>0.451038</td>
      <td>True</td>
      <td>Chihuahua</td>
      <td>0.029248</td>
      <td>True</td>
    </tr>
    <tr>
      <th>10</th>
      <td>890006608113172480</td>
      <td>31166</td>
      <td>7624</td>
      <td>https://twitter.com/dog_rates/status/890006608...</td>
      <td>13</td>
      <td>Koda</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFnwSY4WAAAMliS.jpg</td>
      <td>Samoyed</td>
      <td>0.957979</td>
      <td>True</td>
      <td>Pomeranian</td>
      <td>0.013884</td>
      <td>True</td>
      <td>chow</td>
      <td>0.008167</td>
      <td>True</td>
    </tr>
    <tr>
      <th>11</th>
      <td>889880896479866881</td>
      <td>28268</td>
      <td>5156</td>
      <td>https://twitter.com/dog_rates/status/889880896...</td>
      <td>13</td>
      <td>Bruno</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFl99B1WsAITKsg.jpg</td>
      <td>French_bulldog</td>
      <td>0.377417</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.151317</td>
      <td>True</td>
      <td>muzzle</td>
      <td>0.082981</td>
      <td>False</td>
    </tr>
    <tr>
      <th>12</th>
      <td>889665388333682689</td>
      <td>38818</td>
      <td>8538</td>
      <td>https://twitter.com/dog_rates/status/889665388...</td>
      <td>13</td>
      <td>None</td>
      <td>puppo</td>
      <td>https://pbs.twimg.com/media/DFi579UWsAAatzw.jpg</td>
      <td>Pembroke</td>
      <td>0.966327</td>
      <td>True</td>
      <td>Cardigan</td>
      <td>0.027356</td>
      <td>True</td>
      <td>basenji</td>
      <td>0.004633</td>
      <td>True</td>
    </tr>
    <tr>
      <th>13</th>
      <td>889638837579907072</td>
      <td>27672</td>
      <td>4735</td>
      <td>https://twitter.com/dog_rates/status/889638837...</td>
      <td>12</td>
      <td>Ted</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFihzFfXsAYGDPR.jpg</td>
      <td>French_bulldog</td>
      <td>0.991650</td>
      <td>True</td>
      <td>boxer</td>
      <td>0.002129</td>
      <td>True</td>
      <td>Staffordshire_bullterrier</td>
      <td>0.001498</td>
      <td>True</td>
    </tr>
    <tr>
      <th>14</th>
      <td>889531135344209921</td>
      <td>15359</td>
      <td>2321</td>
      <td>https://twitter.com/dog_rates/status/889531135...</td>
      <td>13</td>
      <td>Stuart</td>
      <td>puppo</td>
      <td>https://pbs.twimg.com/media/DFg_2PVW0AEHN3p.jpg</td>
      <td>golden_retriever</td>
      <td>0.953442</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.013834</td>
      <td>True</td>
      <td>redbone</td>
      <td>0.007958</td>
      <td>True</td>
    </tr>
    <tr>
      <th>15</th>
      <td>889278841981685760</td>
      <td>25652</td>
      <td>5637</td>
      <td>https://twitter.com/dog_rates/status/889278841...</td>
      <td>13</td>
      <td>Oliver</td>
      <td>None</td>
      <td>https://pbs.twimg.com/ext_tw_video_thumb/88927...</td>
      <td>whippet</td>
      <td>0.626152</td>
      <td>True</td>
      <td>borzoi</td>
      <td>0.194742</td>
      <td>True</td>
      <td>Saluki</td>
      <td>0.027351</td>
      <td>True</td>
    </tr>
    <tr>
      <th>16</th>
      <td>888917238123831296</td>
      <td>29611</td>
      <td>4709</td>
      <td>https://twitter.com/dog_rates/status/888917238...</td>
      <td>12</td>
      <td>Jim</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFYRgsOUQAARGhO.jpg</td>
      <td>golden_retriever</td>
      <td>0.714719</td>
      <td>True</td>
      <td>Tibetan_mastiff</td>
      <td>0.120184</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.105506</td>
      <td>True</td>
    </tr>
    <tr>
      <th>17</th>
      <td>888804989199671297</td>
      <td>26080</td>
      <td>4559</td>
      <td>https://twitter.com/dog_rates/status/888804989...</td>
      <td>13</td>
      <td>Zeke</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFWra-3VYAA2piG.jpg</td>
      <td>golden_retriever</td>
      <td>0.469760</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.184172</td>
      <td>True</td>
      <td>English_setter</td>
      <td>0.073482</td>
      <td>True</td>
    </tr>
    <tr>
      <th>18</th>
      <td>888554962724278272</td>
      <td>20290</td>
      <td>3732</td>
      <td>https://twitter.com/dog_rates/status/888554962...</td>
      <td>13</td>
      <td>Ralphus</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFTH_O-UQAACu20.jpg</td>
      <td>Siberian_husky</td>
      <td>0.700377</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.166511</td>
      <td>True</td>
      <td>malamute</td>
      <td>0.111411</td>
      <td>True</td>
    </tr>
    <tr>
      <th>19</th>
      <td>888078434458587136</td>
      <td>22201</td>
      <td>3653</td>
      <td>https://twitter.com/dog_rates/status/888078434...</td>
      <td>12</td>
      <td>Gerald</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFMWn56WsAAkA7B.jpg</td>
      <td>French_bulldog</td>
      <td>0.995026</td>
      <td>True</td>
      <td>pug</td>
      <td>0.000932</td>
      <td>True</td>
      <td>bull_mastiff</td>
      <td>0.000903</td>
      <td>True</td>
    </tr>
    <tr>
      <th>20</th>
      <td>887705289381826560</td>
      <td>30779</td>
      <td>5609</td>
      <td>https://twitter.com/dog_rates/status/887705289...</td>
      <td>13</td>
      <td>Jeffrey</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFHDQBbXgAEqY7t.jpg</td>
      <td>basset</td>
      <td>0.821664</td>
      <td>True</td>
      <td>redbone</td>
      <td>0.087582</td>
      <td>True</td>
      <td>Weimaraner</td>
      <td>0.026236</td>
      <td>True</td>
    </tr>
    <tr>
      <th>21</th>
      <td>887517139158093824</td>
      <td>46959</td>
      <td>12082</td>
      <td>https://twitter.com/dog_rates/status/887517139...</td>
      <td>14</td>
      <td>such</td>
      <td>None</td>
      <td>https://pbs.twimg.com/ext_tw_video_thumb/88751...</td>
      <td>limousine</td>
      <td>0.130432</td>
      <td>False</td>
      <td>tow_truck</td>
      <td>0.029175</td>
      <td>False</td>
      <td>shopping_cart</td>
      <td>0.026321</td>
      <td>False</td>
    </tr>
    <tr>
      <th>22</th>
      <td>887473957103951883</td>
      <td>69871</td>
      <td>18781</td>
      <td>https://twitter.com/dog_rates/status/887473957...</td>
      <td>13</td>
      <td>Canela</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DFDw2tyUQAAAFke.jpg</td>
      <td>Pembroke</td>
      <td>0.809197</td>
      <td>True</td>
      <td>Rhodesian_ridgeback</td>
      <td>0.054950</td>
      <td>True</td>
      <td>beagle</td>
      <td>0.038915</td>
      <td>True</td>
    </tr>
    <tr>
      <th>23</th>
      <td>887343217045368832</td>
      <td>34222</td>
      <td>10737</td>
      <td>https://twitter.com/dog_rates/status/887343217...</td>
      <td>13</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/ext_tw_video_thumb/88734...</td>
      <td>Mexican_hairless</td>
      <td>0.330741</td>
      <td>True</td>
      <td>sea_lion</td>
      <td>0.275645</td>
      <td>False</td>
      <td>Weimaraner</td>
      <td>0.134203</td>
      <td>True</td>
    </tr>
    <tr>
      <th>24</th>
      <td>887101392804085760</td>
      <td>31061</td>
      <td>6167</td>
      <td>https://twitter.com/dog_rates/status/887101392...</td>
      <td>12</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE-eAq6UwAA-jaE.jpg</td>
      <td>Samoyed</td>
      <td>0.733942</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.035029</td>
      <td>True</td>
      <td>Staffordshire_bullterrier</td>
      <td>0.029705</td>
      <td>True</td>
    </tr>
    <tr>
      <th>25</th>
      <td>886983233522544640</td>
      <td>35859</td>
      <td>8084</td>
      <td>https://twitter.com/dog_rates/status/886983233...</td>
      <td>13</td>
      <td>Maya</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE8yicJW0AAAvBJ.jpg</td>
      <td>Chihuahua</td>
      <td>0.793469</td>
      <td>True</td>
      <td>toy_terrier</td>
      <td>0.143528</td>
      <td>True</td>
      <td>can_opener</td>
      <td>0.032253</td>
      <td>False</td>
    </tr>
    <tr>
      <th>26</th>
      <td>886736880519319552</td>
      <td>12306</td>
      <td>3443</td>
      <td>https://www.gofundme.com/mingusneedsus,https:/...</td>
      <td>13</td>
      <td>Mingus</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE5Se8FXcAAJFx4.jpg</td>
      <td>kuvasz</td>
      <td>0.309706</td>
      <td>True</td>
      <td>Great_Pyrenees</td>
      <td>0.186136</td>
      <td>True</td>
      <td>Dandie_Dinmont</td>
      <td>0.086346</td>
      <td>True</td>
    </tr>
    <tr>
      <th>27</th>
      <td>886680336477933568</td>
      <td>22798</td>
      <td>4610</td>
      <td>https://twitter.com/dog_rates/status/886680336...</td>
      <td>13</td>
      <td>Derek</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DE4fEDzWAAAyHMM.jpg</td>
      <td>convertible</td>
      <td>0.738995</td>
      <td>False</td>
      <td>sports_car</td>
      <td>0.139952</td>
      <td>False</td>
      <td>car_wheel</td>
      <td>0.044173</td>
      <td>False</td>
    </tr>
    <tr>
      <th>28</th>
      <td>886366144734445568</td>
      <td>21524</td>
      <td>3316</td>
      <td>https://twitter.com/dog_rates/status/886366144...</td>
      <td>12</td>
      <td>Roscoe</td>
      <td>pupper</td>
      <td>https://pbs.twimg.com/media/DE0BTnQUwAApKEH.jpg</td>
      <td>French_bulldog</td>
      <td>0.999201</td>
      <td>True</td>
      <td>Chihuahua</td>
      <td>0.000361</td>
      <td>True</td>
      <td>Boston_bull</td>
      <td>0.000076</td>
      <td>True</td>
    </tr>
    <tr>
      <th>29</th>
      <td>886258384151887873</td>
      <td>28469</td>
      <td>6523</td>
      <td>https://twitter.com/dog_rates/status/886258384...</td>
      <td>13</td>
      <td>Waffles</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/DEyfTG4UMAE4aE9.jpg</td>
      <td>pug</td>
      <td>0.943575</td>
      <td>True</td>
      <td>shower_cap</td>
      <td>0.025286</td>
      <td>False</td>
      <td>Siamese_cat</td>
      <td>0.002849</td>
      <td>False</td>
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
      <td>...</td>
    </tr>
    <tr>
      <th>2043</th>
      <td>666411507551481857</td>
      <td>459</td>
      <td>339</td>
      <td>https://twitter.com/dog_rates/status/666411507...</td>
      <td>2</td>
      <td>quite</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT-RugiWIAELEaq.jpg</td>
      <td>coho</td>
      <td>0.404640</td>
      <td>False</td>
      <td>barracouta</td>
      <td>0.271485</td>
      <td>False</td>
      <td>gar</td>
      <td>0.189945</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2044</th>
      <td>666407126856765440</td>
      <td>113</td>
      <td>44</td>
      <td>https://twitter.com/dog_rates/status/666407126...</td>
      <td>7</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT-NvwmW4AAugGZ.jpg</td>
      <td>black-and-tan_coonhound</td>
      <td>0.529139</td>
      <td>True</td>
      <td>bloodhound</td>
      <td>0.244220</td>
      <td>True</td>
      <td>flat-coated_retriever</td>
      <td>0.173810</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2045</th>
      <td>666396247373291520</td>
      <td>172</td>
      <td>92</td>
      <td>https://twitter.com/dog_rates/status/666396247...</td>
      <td>9</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT-D2ZHWIAA3gK1.jpg</td>
      <td>Chihuahua</td>
      <td>0.978108</td>
      <td>True</td>
      <td>toy_terrier</td>
      <td>0.009397</td>
      <td>True</td>
      <td>papillon</td>
      <td>0.004577</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2046</th>
      <td>666373753744588802</td>
      <td>194</td>
      <td>100</td>
      <td>https://twitter.com/dog_rates/status/666373753...</td>
      <td>11</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9vZEYWUAAlZ05.jpg</td>
      <td>soft-coated_wheaten_terrier</td>
      <td>0.326467</td>
      <td>True</td>
      <td>Afghan_hound</td>
      <td>0.259551</td>
      <td>True</td>
      <td>briard</td>
      <td>0.206803</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2047</th>
      <td>666362758909284353</td>
      <td>804</td>
      <td>595</td>
      <td>https://twitter.com/dog_rates/status/666362758...</td>
      <td>6</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9lXGsUcAAyUFt.jpg</td>
      <td>guinea_pig</td>
      <td>0.996496</td>
      <td>False</td>
      <td>skunk</td>
      <td>0.002402</td>
      <td>False</td>
      <td>hamster</td>
      <td>0.000461</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2048</th>
      <td>666353288456101888</td>
      <td>229</td>
      <td>77</td>
      <td>https://twitter.com/dog_rates/status/666353288...</td>
      <td>8</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9cx0tUEAAhNN_.jpg</td>
      <td>malamute</td>
      <td>0.336874</td>
      <td>True</td>
      <td>Siberian_husky</td>
      <td>0.147655</td>
      <td>True</td>
      <td>Eskimo_dog</td>
      <td>0.093412</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2049</th>
      <td>666345417576210432</td>
      <td>307</td>
      <td>146</td>
      <td>https://twitter.com/dog_rates/status/666345417...</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9Vn7PWoAA_ZCM.jpg</td>
      <td>golden_retriever</td>
      <td>0.858744</td>
      <td>True</td>
      <td>Chesapeake_Bay_retriever</td>
      <td>0.054787</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.014241</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2050</th>
      <td>666337882303524864</td>
      <td>204</td>
      <td>96</td>
      <td>https://twitter.com/dog_rates/status/666337882...</td>
      <td>9</td>
      <td>an</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT9OwFIWEAMuRje.jpg</td>
      <td>ox</td>
      <td>0.416669</td>
      <td>False</td>
      <td>Newfoundland</td>
      <td>0.278407</td>
      <td>True</td>
      <td>groenendael</td>
      <td>0.102643</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2051</th>
      <td>666293911632134144</td>
      <td>522</td>
      <td>368</td>
      <td>https://twitter.com/dog_rates/status/666293911...</td>
      <td>3</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8mx7KW4AEQu8N.jpg</td>
      <td>three-toed_sloth</td>
      <td>0.914671</td>
      <td>False</td>
      <td>otter</td>
      <td>0.015250</td>
      <td>False</td>
      <td>great_grey_owl</td>
      <td>0.013207</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2052</th>
      <td>666287406224695296</td>
      <td>152</td>
      <td>71</td>
      <td>https://twitter.com/dog_rates/status/666287406...</td>
      <td>1</td>
      <td>an</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8g3BpUEAAuFjg.jpg</td>
      <td>Maltese_dog</td>
      <td>0.857531</td>
      <td>True</td>
      <td>toy_poodle</td>
      <td>0.063064</td>
      <td>True</td>
      <td>miniature_poodle</td>
      <td>0.025581</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2053</th>
      <td>666273097616637952</td>
      <td>184</td>
      <td>82</td>
      <td>https://twitter.com/dog_rates/status/666273097...</td>
      <td>11</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8T1mtUwAA3aqm.jpg</td>
      <td>Italian_greyhound</td>
      <td>0.176053</td>
      <td>True</td>
      <td>toy_terrier</td>
      <td>0.111884</td>
      <td>True</td>
      <td>basenji</td>
      <td>0.111152</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2054</th>
      <td>666268910803644416</td>
      <td>108</td>
      <td>37</td>
      <td>https://twitter.com/dog_rates/status/666268910...</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT8QCd1WEAADXws.jpg</td>
      <td>desktop_computer</td>
      <td>0.086502</td>
      <td>False</td>
      <td>desk</td>
      <td>0.085547</td>
      <td>False</td>
      <td>bookcase</td>
      <td>0.079480</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2055</th>
      <td>666104133288665088</td>
      <td>14765</td>
      <td>6871</td>
      <td>https://twitter.com/dog_rates/status/666104133...</td>
      <td>1</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT56LSZWoAAlJj2.jpg</td>
      <td>hen</td>
      <td>0.965932</td>
      <td>False</td>
      <td>cock</td>
      <td>0.033919</td>
      <td>False</td>
      <td>partridge</td>
      <td>0.000052</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2056</th>
      <td>666102155909144576</td>
      <td>81</td>
      <td>16</td>
      <td>https://twitter.com/dog_rates/status/666102155...</td>
      <td>11</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT54YGiWUAEZnoK.jpg</td>
      <td>English_setter</td>
      <td>0.298617</td>
      <td>True</td>
      <td>Newfoundland</td>
      <td>0.149842</td>
      <td>True</td>
      <td>borzoi</td>
      <td>0.133649</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2057</th>
      <td>666099513787052032</td>
      <td>164</td>
      <td>73</td>
      <td>https://twitter.com/dog_rates/status/666099513...</td>
      <td>8</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT51-JJUEAA6hV8.jpg</td>
      <td>Lhasa</td>
      <td>0.582330</td>
      <td>True</td>
      <td>Shih-Tzu</td>
      <td>0.166192</td>
      <td>True</td>
      <td>Dandie_Dinmont</td>
      <td>0.089688</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2058</th>
      <td>666094000022159362</td>
      <td>169</td>
      <td>79</td>
      <td>https://twitter.com/dog_rates/status/666094000...</td>
      <td>9</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5w9gUW4AAsBNN.jpg</td>
      <td>bloodhound</td>
      <td>0.195217</td>
      <td>True</td>
      <td>German_shepherd</td>
      <td>0.078260</td>
      <td>True</td>
      <td>malinois</td>
      <td>0.075628</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2059</th>
      <td>666082916733198337</td>
      <td>121</td>
      <td>47</td>
      <td>https://twitter.com/dog_rates/status/666082916...</td>
      <td>6</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5m4VGWEAAtKc8.jpg</td>
      <td>pug</td>
      <td>0.489814</td>
      <td>True</td>
      <td>bull_mastiff</td>
      <td>0.404722</td>
      <td>True</td>
      <td>French_bulldog</td>
      <td>0.048960</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2060</th>
      <td>666073100786774016</td>
      <td>335</td>
      <td>174</td>
      <td>https://twitter.com/dog_rates/status/666073100...</td>
      <td>10</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5d9DZXAAALcwe.jpg</td>
      <td>Walker_hound</td>
      <td>0.260857</td>
      <td>True</td>
      <td>English_foxhound</td>
      <td>0.175382</td>
      <td>True</td>
      <td>Ibizan_hound</td>
      <td>0.097471</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2061</th>
      <td>666071193221509120</td>
      <td>154</td>
      <td>67</td>
      <td>https://twitter.com/dog_rates/status/666071193...</td>
      <td>9</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5cN_3WEAAlOoZ.jpg</td>
      <td>Gordon_setter</td>
      <td>0.503672</td>
      <td>True</td>
      <td>Yorkshire_terrier</td>
      <td>0.174201</td>
      <td>True</td>
      <td>Pekinese</td>
      <td>0.109454</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2062</th>
      <td>666063827256086533</td>
      <td>496</td>
      <td>232</td>
      <td>https://twitter.com/dog_rates/status/666063827...</td>
      <td>10</td>
      <td>the</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Vg_wXIAAXfnj.jpg</td>
      <td>golden_retriever</td>
      <td>0.775930</td>
      <td>True</td>
      <td>Tibetan_mastiff</td>
      <td>0.093718</td>
      <td>True</td>
      <td>Labrador_retriever</td>
      <td>0.072427</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2063</th>
      <td>666058600524156928</td>
      <td>115</td>
      <td>61</td>
      <td>https://twitter.com/dog_rates/status/666058600...</td>
      <td>8</td>
      <td>the</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Qw94XAAA_2dP.jpg</td>
      <td>miniature_poodle</td>
      <td>0.201493</td>
      <td>True</td>
      <td>komondor</td>
      <td>0.192305</td>
      <td>True</td>
      <td>soft-coated_wheaten_terrier</td>
      <td>0.082086</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2064</th>
      <td>666057090499244032</td>
      <td>304</td>
      <td>146</td>
      <td>https://twitter.com/dog_rates/status/666057090...</td>
      <td>9</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5PY90WoAAQGLo.jpg</td>
      <td>shopping_cart</td>
      <td>0.962465</td>
      <td>False</td>
      <td>shopping_basket</td>
      <td>0.014594</td>
      <td>False</td>
      <td>golden_retriever</td>
      <td>0.007959</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2065</th>
      <td>666055525042405380</td>
      <td>448</td>
      <td>261</td>
      <td>https://twitter.com/dog_rates/status/666055525...</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5N9tpXIAAifs1.jpg</td>
      <td>chow</td>
      <td>0.692517</td>
      <td>True</td>
      <td>Tibetan_mastiff</td>
      <td>0.058279</td>
      <td>True</td>
      <td>fur_coat</td>
      <td>0.054449</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2066</th>
      <td>666051853826850816</td>
      <td>1253</td>
      <td>879</td>
      <td>https://twitter.com/dog_rates/status/666051853...</td>
      <td>2</td>
      <td>an</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5KoJ1WoAAJash.jpg</td>
      <td>box_turtle</td>
      <td>0.933012</td>
      <td>False</td>
      <td>mud_turtle</td>
      <td>0.045885</td>
      <td>False</td>
      <td>terrapin</td>
      <td>0.017885</td>
      <td>False</td>
    </tr>
    <tr>
      <th>2067</th>
      <td>666050758794694657</td>
      <td>136</td>
      <td>60</td>
      <td>https://twitter.com/dog_rates/status/666050758...</td>
      <td>10</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Jof1WUAEuVxN.jpg</td>
      <td>Bernese_mountain_dog</td>
      <td>0.651137</td>
      <td>True</td>
      <td>English_springer</td>
      <td>0.263788</td>
      <td>True</td>
      <td>Greater_Swiss_Mountain_dog</td>
      <td>0.016199</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2068</th>
      <td>666049248165822465</td>
      <td>111</td>
      <td>41</td>
      <td>https://twitter.com/dog_rates/status/666049248...</td>
      <td>5</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5IQmsXIAAKY4A.jpg</td>
      <td>miniature_pinscher</td>
      <td>0.560311</td>
      <td>True</td>
      <td>Rottweiler</td>
      <td>0.243682</td>
      <td>True</td>
      <td>Doberman</td>
      <td>0.154629</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2069</th>
      <td>666044226329800704</td>
      <td>311</td>
      <td>147</td>
      <td>https://twitter.com/dog_rates/status/666044226...</td>
      <td>6</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT5Dr8HUEAA-lEu.jpg</td>
      <td>Rhodesian_ridgeback</td>
      <td>0.408143</td>
      <td>True</td>
      <td>redbone</td>
      <td>0.360687</td>
      <td>True</td>
      <td>miniature_pinscher</td>
      <td>0.222752</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2070</th>
      <td>666033412701032449</td>
      <td>128</td>
      <td>47</td>
      <td>https://twitter.com/dog_rates/status/666033412...</td>
      <td>9</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT4521TWwAEvMyu.jpg</td>
      <td>German_shepherd</td>
      <td>0.596461</td>
      <td>True</td>
      <td>malinois</td>
      <td>0.138584</td>
      <td>True</td>
      <td>bloodhound</td>
      <td>0.116197</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2071</th>
      <td>666029285002620928</td>
      <td>132</td>
      <td>48</td>
      <td>https://twitter.com/dog_rates/status/666029285...</td>
      <td>7</td>
      <td>a</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT42GRgUYAA5iDo.jpg</td>
      <td>redbone</td>
      <td>0.506826</td>
      <td>True</td>
      <td>miniature_pinscher</td>
      <td>0.074192</td>
      <td>True</td>
      <td>Rhodesian_ridgeback</td>
      <td>0.072010</td>
      <td>True</td>
    </tr>
    <tr>
      <th>2072</th>
      <td>666020888022790149</td>
      <td>2535</td>
      <td>532</td>
      <td>https://twitter.com/dog_rates/status/666020888...</td>
      <td>8</td>
      <td>None</td>
      <td>None</td>
      <td>https://pbs.twimg.com/media/CT4udn0WwAA0aMy.jpg</td>
      <td>Welsh_springer_spaniel</td>
      <td>0.465074</td>
      <td>True</td>
      <td>collie</td>
      <td>0.156665</td>
      <td>True</td>
      <td>Shetland_sheepdog</td>
      <td>0.061428</td>
      <td>True</td>
    </tr>
  </tbody>
</table>
<p>2073 rows × 17 columns</p>
</div>



#### Define:

Change the none value with NaN (To ease the analysis)
https://www.codegrepper.com/code-examples/delphi/how+to+replace+values+with+nan+in+pandas

#### Code:


```python
#Change the none value with NaN
```

#### Test:


```python

```




    NaN        1753
    pupper      221
    doggo        67
    puppo        24
    floofer       8
    Name: dog_type, dtype: int64




```python

```




    NaN          577
    a             55
    Charlie       11
    Cooper        10
    Penny         10
    Tucker        10
    Lucy          10
    Oliver        10
    Lola           8
    Bo             8
    Sadie          8
    Winston        8
    the            7
    Daisy          7
    an             7
    Toby           7
    Dave           6
    Bella          6
    Scout          6
    Milo           6
    Bailey         6
    Stanley        6
    Koda           6
    Jax            6
    Rusty          6
    Leo            5
    Oscar          5
    Larry          5
    Chester        5
    Alfie          5
                ... 
    Alf            1
    Eugene         1
    Lipton         1
    Danny          1
    Chevy          1
    Erik           1
    Ridley         1
    Tyrus          1
    Al             1
    Molly          1
    Wesley         1
    Carter         1
    Coleman        1
    Buddah         1
    Lolo           1
    Wishes         1
    Kellogg        1
    Zara           1
    Storkson       1
    Poppy          1
    Kody           1
    Augie          1
    Scruffers      1
    O              1
    Milky          1
    Jarvis         1
    Billy          1
    Cheesy         1
    Ebby           1
    Dotsy          1
    Name: dog_name, Length: 936, dtype: int64



## 3.6- Save file "twitter_archive_master.csv":


```python

```

# Analysis of the data

# Import visualization libraries
import matplotlib.pyplot as plt
import seaborn as sns

# 'Magic word' so that your visualizations are plotted
%matplotlib inline

# Set style of plots with seaborn
sns.set(style="darkgrid",font_scale=1.5)

#Load file
twitter_archive_master = pd.read_csv('twitter_archive_master.csv')
twitter_archive_master.head()

## Describe:


```python
# data statistics
twitter_archive_master.describe()
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
      <th>Unnamed: 0</th>
      <th>tweet_id</th>
      <th>favorite_count</th>
      <th>retweet_count</th>
      <th>retweeted_status_id</th>
      <th>retweeted_status_user_id</th>
      <th>rating_numerator</th>
      <th>dog_1_prediction_conformance_percent</th>
      <th>dog_2_prediction_conformance_percent</th>
      <th>dog_3_prediction_conformance_percent</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>2073.000000</td>
      <td>2.073000e+03</td>
      <td>2073.000000</td>
      <td>2073.000000</td>
      <td>7.900000e+01</td>
      <td>7.900000e+01</td>
      <td>2073.000000</td>
      <td>2073.000000</td>
      <td>2.073000e+03</td>
      <td>2.073000e+03</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>1036.000000</td>
      <td>7.383634e+17</td>
      <td>8556.718283</td>
      <td>2976.089243</td>
      <td>7.663364e+17</td>
      <td>9.967874e+15</td>
      <td>12.265798</td>
      <td>0.594532</td>
      <td>1.346665e-01</td>
      <td>6.034005e-02</td>
    </tr>
    <tr>
      <th>std</th>
      <td>598.567874</td>
      <td>6.780118e+16</td>
      <td>12098.640994</td>
      <td>5054.897526</td>
      <td>5.882530e+16</td>
      <td>8.859637e+16</td>
      <td>40.699924</td>
      <td>0.271234</td>
      <td>1.006830e-01</td>
      <td>5.092769e-02</td>
    </tr>
    <tr>
      <th>min</th>
      <td>0.000000</td>
      <td>6.660209e+17</td>
      <td>0.000000</td>
      <td>16.000000</td>
      <td>6.675094e+17</td>
      <td>7.832140e+05</td>
      <td>0.000000</td>
      <td>0.044333</td>
      <td>1.011300e-08</td>
      <td>1.740170e-10</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>518.000000</td>
      <td>6.764706e+17</td>
      <td>1674.000000</td>
      <td>634.000000</td>
      <td>7.124037e+17</td>
      <td>4.196984e+09</td>
      <td>10.000000</td>
      <td>0.364095</td>
      <td>5.390140e-02</td>
      <td>1.619920e-02</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>1036.000000</td>
      <td>7.119681e+17</td>
      <td>3864.000000</td>
      <td>1408.000000</td>
      <td>7.798343e+17</td>
      <td>4.196984e+09</td>
      <td>11.000000</td>
      <td>0.588230</td>
      <td>1.186220e-01</td>
      <td>4.947150e-02</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>1554.000000</td>
      <td>7.931959e+17</td>
      <td>10937.000000</td>
      <td>3443.000000</td>
      <td>8.068680e+17</td>
      <td>4.196984e+09</td>
      <td>12.000000</td>
      <td>0.843911</td>
      <td>1.955730e-01</td>
      <td>9.193000e-02</td>
    </tr>
    <tr>
      <th>max</th>
      <td>2072.000000</td>
      <td>8.924206e+17</td>
      <td>132810.000000</td>
      <td>79515.000000</td>
      <td>8.768508e+17</td>
      <td>7.874618e+17</td>
      <td>1776.000000</td>
      <td>1.000000</td>
      <td>4.880140e-01</td>
      <td>2.734190e-01</td>
    </tr>
  </tbody>
</table>
</div>



## Dogs types vs Tweets:


```python
# dogs types count
twitter_archive_master.dog_type.value_counts()
```




    pupper     221
    doggo       67
    puppo       24
    floofer      8
    Name: dog_type, dtype: int64




```python
fig = plt.figure(figsize=(15,8))
twitter_archive_master.dog_type.value_counts().plot(kind='barh')
plt.title("Comparison between dogs according to the classification",fontsize=20)
plt.ylabel("Dog class")
plt.xlabel("Number of Tweets"); 
```


![png](output_169_0.png)


Conclusion:
    The popper dogs are the most liked dogs

### Dog types vs Rating:


```python
fig = plt.figure(figsize=(15,8))
twitter_archive_master.groupby('dog_type')['rating_numerator'].mean().plot(kind='barh')
plt.title("Comparison between dogs' rating according to the classification",fontsize=20)
plt.ylabel("Dog class")
plt.xlabel("Average Rating"); 
```


![png](output_172_0.png)


Conclosion:
    Dogs classifications puppo, floofer and doggo are the highest average rated dogs, then comes the pupper.

## favorite_count vs retweet_count:


```python
twitter_archive_master.groupby('rating_numerator')[['favorite_count','retweet_count']].corr().describe()
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
      <th>favorite_count</th>
      <th>retweet_count</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>count</th>
      <td>30.000000</td>
      <td>30.000000</td>
    </tr>
    <tr>
      <th>mean</th>
      <td>0.928963</td>
      <td>0.928963</td>
    </tr>
    <tr>
      <th>std</th>
      <td>0.122201</td>
      <td>0.122201</td>
    </tr>
    <tr>
      <th>min</th>
      <td>0.517910</td>
      <td>0.517910</td>
    </tr>
    <tr>
      <th>25%</th>
      <td>0.906694</td>
      <td>0.906694</td>
    </tr>
    <tr>
      <th>50%</th>
      <td>1.000000</td>
      <td>1.000000</td>
    </tr>
    <tr>
      <th>75%</th>
      <td>1.000000</td>
      <td>1.000000</td>
    </tr>
    <tr>
      <th>max</th>
      <td>1.000000</td>
      <td>1.000000</td>
    </tr>
  </tbody>
</table>
</div>




```python
twitter_archive_master.plot(kind='scatter',x='favorite_count',y='retweet_count',color='red')
plt.show()
```


![png](output_176_0.png)


Conclusion:
    There are a strong relationship between the retweet_count and favorite_count.

## Dog types vs favorite_count and retweet_count:


```python
fig = plt.figure(figsize=(15,8))
twitter_archive_master.groupby('dog_type')['favorite_count', 'retweet_count'].mean().plot(kind='barh')
plt.title("Comparison between dogs' favorite_count and retweet_count according to the classification",fontsize=20)
plt.ylabel("Dog class")
plt.xlabel("Average Rating"); 
```


    <matplotlib.figure.Figure at 0x7f07f4b4b3c8>



![png](output_179_1.png)


Conclusion:
    1- The retweet count for the doggo and puppo are the highest, but the lowest for pupper.
    2- the use of favorit count is more senstive than the retweet count.
