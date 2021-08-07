#Python
Assignments
Lists
Write a Python program which accepts a sequence of comma-separated numbers from user and generate a list and a tuple with those numbers.
values = input("Input some comma seprated numbers : ")
list = values.split(",")
tuple = tuple(list)
print('List : ',list)
print('Tuple : ',tuple)
Input some comma seprated numbers : 3,5,7,23
List :  ['3', '5', '7', '23']
Tuple :  ('3', '5', '7', '23')
color_list = ["Red","Green","White" ,"Black"]
Result_Color = [color_list [0], color_list [-1]]
Result_Color
['Red', 'Black']
Write a Python program to print the even numbers from a given list.
Sample List : [1, 2, 3, 4, 5, 6, 7, 8, 9]
num = [1, 2, 3, 4, 5, 6, 7, 8, 9]
Result = []
for i in num:
     if i % 2 == 0:
            Result.append(i)
Result
[2, 4, 6, 8]
Module
from datetime import date
def differ_days(date1, date2):

    a = date1
    b = date2
    return (a-b).days
print()
print(differ_days((date(2014,7,2)), date(2014,7,11)))
print()
-9

Functions
Write a Python program to get the volume of a sphere with radius 6.
pi = 3.1415926535897931
r= 6.0
V= 4.0/3.0*pi* r**3
print('The volume of the sphere is: ',V)
The volume of the sphere is:  904.7786842338603
Write a Python program to calculate the sum of three given numbers, if the values are equal then return three times of their sum hint: write User defined functions
def a(x, y, z):

     sum = x + y + z
  
     if x == y == z:
      sum = sum * 3
     return sum

print(a(1,2,3))
print(a(3, 3, 3))
6
27
Write a Python program to count the number 4 in a given list.

List = [1,4,6,8,4,9,4]
def list_count_4(nums):
  count = 0  
  for num in nums:
    if num == 4:
      count = count + 1

  return count

print(list_count_4([1, 4, 6, 8, 4, 9, 4]))
3
a Python program to print all even numbers from a given numbers list in the same order and stop the printing if any numbers that come after 237 in the sequence. Write
numbers = [    
    386, 462, 47, 418, 907, 344, 236, 375, 823, 566, 597, 978, 328, 615, 953, 345, 
    399, 162, 758, 219, 918, 237, 412, 566, 826, 248, 866, 950, 626, 949, 687, 217, 
    815, 67, 104, 58, 512, 24, 892, 894, 767, 553, 81, 379, 843, 831, 445, 742, 717, 
    958,743, 527
    ]
for x in numbers:
    if x == 237:
        print(x)
        break;
    elif x % 2 == 0:
        print(x)
386
462
418
344
236
566
978
328
162
758
918
237
Write a Python program to find those numbers which are divisible by 7 and multiple of 5, between 1500 and 2700 (both included)
nl=[]
for x in range(1500, 2701):
    if (x%7==0) and (x%5==0):
        nl.append(str(x))
print (','.join(nl))
1505,1540,1575,1610,1645,1680,1715,1750,1785,1820,1855,1890,1925,1960,1995,2030,2065,2100,2135,2170,2205,2240,2275,2310,2345,2380,2415,2450,2485,2520,2555,2590,2625,2660,2695
Write a Python program that prints all the numbers from 0 to 6 except 3 and 6.
for x in range(6):
    if (x == 3 or x==6):
        continue
    print(x,end=' ')
print("\n")
0 1 2 4 5 

Write a Python program to get the Fibonacci series between 0 to 50.
x,y=0,1

while y<50:
    print(y)
    x,y = y,x+y
1
1
2
3
5
8
13
21
34
def unique_list(l):
  x = []
  for a in l:
    if a not in x:
      x.append(a)
  return x

print(unique_list([1,2,3,3,3,3,4,5]))
[1, 2, 3, 4, 5]
Strings
Write a Python program to concatenate all elements in a list into a string and return it.
def concatenate_list_data(list):
    result= ''
    for element in list:
        result += str(element)
    return result

print(concatenate_list_data([1, 5, 8, 9, 15]))
158915
Dictionary
Write a Python script to concatenate following dictionaries to create a new one.
dic1={1:10, 2:20}
dic2={3:30, 4:40}
dic3={5:50,6:60}
dic4={}
for d in (dic1, dic2, dic3): dic4.update(d)
print(dic4)
{1: 10, 2: 20, 3: 30, 4: 40, 5: 50, 6: 60}
Series
Write a Python program to add, subtract, multiple and divide two Pandas Series.
import pandas as pd
ds1 = pd.Series([2, 4, 6, 8, 10])
ds2 = pd.Series([1, 3, 5, 7, 9])
ds = ds1 + ds2
print("Addition:")
print(ds)
print("Subtraction:")
ds = ds1 - ds2
print(ds)
print("Multiplication:")
ds = ds1 * ds2
print(ds)
print("Division:")
ds = ds1 / ds2
print(ds)
Addition:
0     3
1     7
2    11
3    15
4    19
dtype: int64
Subtraction:
0    1
1    1
2    1
3    1
4    1
dtype: int64
Multiplication:
0     2
1    12
2    30
3    56
4    90
dtype: int64
Division:
0    2.000000
1    1.333333
2    1.200000
3    1.142857
4    1.111111
dtype: float64
Dataframes
Write a Pandas program to select the specified columns and rows from a given data frame. Go to the editorSample Python dictionary data and list labels:
import pandas as pd
import numpy as np

exam_data  = {'name': ['Anastasia', 'Dima', 'Katherine', 'James', 'Emily', 'Michael', 'Matthew', 'Laura', 'Kevin', 'Jonas'],
        'score': [12.5, 9, 16.5, np.nan, 9, 20, 14.5, np.nan, 8, 19],
        'attempts': [1, 3, 2, 3, 2, 3, 1, 1, 2, 1],
        'qualify': ['yes', 'no', 'yes', 'no', 'no', 'yes', 'yes', 'no', 'no', 'yes']}
labels = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j']

df = pd.DataFrame(exam_data , index=labels)
print("Select specific columns and rows:")
print(df.iloc[[1, 3, 5, 6], [0, 1]])
Select specific columns and rows:
      name  score
b     Dima    9.0
d    James    NaN
f  Michael   20.0
g  Matthew   14.5
Use Crime dataset from LMS
import pandas as pd
df = pd.read_csv(r'C:\Users\Shubham\Downloads\Data Sets (1)\crime_data.csv')
df
Unnamed: 0	Murder	Assault	UrbanPop	Rape
0	Alabama	13.2	236	58	21.2
1	Alaska	10.0	263	48	44.5
2	Arizona	8.1	294	80	31.0
3	Arkansas	8.8	190	50	19.5
4	California	9.0	276	91	40.6
5	Colorado	7.9	204	78	38.7
6	Connecticut	3.3	110	77	11.1
7	Delaware	5.9	238	72	15.8
8	Florida	15.4	335	80	31.9
9	Georgia	17.4	211	60	25.8
10	Hawaii	5.3	46	83	20.2
11	Idaho	2.6	120	54	14.2
12	Illinois	10.4	249	83	24.0
13	Indiana	7.2	113	65	21.0
14	Iowa	2.2	56	57	11.3
15	Kansas	6.0	115	66	18.0
16	Kentucky	9.7	109	52	16.3
17	Louisiana	15.4	249	66	22.2
18	Maine	2.1	83	51	7.8
19	Maryland	11.3	300	67	27.8
20	Massachusetts	4.4	149	85	16.3
21	Michigan	12.1	255	74	35.1
22	Minnesota	2.7	72	66	14.9
23	Mississippi	16.1	259	44	17.1
24	Missouri	9.0	178	70	28.2
25	Montana	6.0	109	53	16.4
26	Nebraska	4.3	102	62	16.5
27	Nevada	12.2	252	81	46.0
28	New Hampshire	2.1	57	56	9.5
29	New Jersey	7.4	159	89	18.8
30	New Mexico	11.4	285	70	32.1
31	New York	11.1	254	86	26.1
32	North Carolina	13.0	337	45	16.1
33	North Dakota	0.8	45	44	7.3
34	Ohio	7.3	120	75	21.4
35	Oklahoma	6.6	151	68	20.0
36	Oregon	4.9	159	67	29.3
37	Pennsylvania	6.3	106	72	14.9
38	Rhode Island	3.4	174	87	8.3
39	South Carolina	14.4	279	48	22.5
40	South Dakota	3.8	86	45	12.8
41	Tennessee	13.2	188	59	26.9
42	Texas	12.7	201	80	25.5
43	Utah	3.2	120	80	22.9
44	Vermont	2.2	48	32	11.2
45	Virginia	8.5	156	63	20.7
46	Washington	4.0	145	73	26.2
47	West Virginia	5.7	81	39	9.3
48	Wisconsin	2.6	53	66	10.8
49	Wyoming	6.8	161	60	15.6
find the aggregations like all moments of business decisions for all columns,value counts.
df.count()
Unnamed: 0    50
Murder        50
Assault       50
UrbanPop      50
Rape          50
dtype: int64
df.Murder.mean()
7.787999999999999
df.Assault.sum()
8538
df.UrbanPop.max()
91
df.Rape.min()
7.3
import matplotlib.pyplot as plt
df.plot("Unnamed: 0" , "UrbanPop")

plt.show()

df.plot(kind = 'scatter', x = 'Unnamed: 0', y = 'Rape')
<AxesSubplot:xlabel='Unnamed: 0', ylabel='Rape'>

plt.hist(df)
plt.show()

import seaborn as sns
sns.pairplot(df)
<seaborn.axisgrid.PairGrid at 0x2b5ef0b17f0>

sns.heatmap(df.corr(), annot=True)  #plot the correlation coefficients as a heatmap
<AxesSubplot:>

sns.scatterplot(df['Assault'], df['Rape'], hue=df['Unnamed: 0'], palette='Set2')
C:\Users\Shubham\anaconda3\lib\site-packages\seaborn\_decorators.py:36: FutureWarning: Pass the following variables as keyword args: x, y. From version 0.12, the only valid positional argument will be `data`, and passing other arguments without an explicit keyword will result in an error or misinterpretation.
  warnings.warn(
<AxesSubplot:xlabel='Assault', ylabel='Rape'>

use mtcars dataset from LMS
import pandas as pd
df1 = pd.read_csv(r'C:\Users\Shubham\Downloads\Data Sets (1)\mtcars.csv.csv')
df1
mpg	cyl	disp	hp	drat	wt	qsec	vs	am	gear	carb
0	21.0	6	160.0	110	3.90	2.620	16.46	0	1	4	4
1	21.0	6	160.0	110	3.90	2.875	17.02	0	1	4	4
2	22.8	4	108.0	93	3.85	2.320	18.61	1	1	4	1
3	21.4	6	258.0	110	3.08	3.215	19.44	1	0	3	1
4	18.7	8	360.0	175	3.15	3.440	17.02	0	0	3	2
5	18.1	6	225.0	105	2.76	3.460	20.22	1	0	3	1
6	14.3	8	360.0	245	3.21	3.570	15.84	0	0	3	4
7	24.4	4	146.7	62	3.69	3.190	20.00	1	0	4	2
8	22.8	4	140.8	95	3.92	3.150	22.90	1	0	4	2
9	19.2	6	167.6	123	3.92	3.440	18.30	1	0	4	4
10	17.8	6	167.6	123	3.92	3.440	18.90	1	0	4	4
11	16.4	8	275.8	180	3.07	4.070	17.40	0	0	3	3
12	17.3	8	275.8	180	3.07	3.730	17.60	0	0	3	3
13	15.2	8	275.8	180	3.07	3.780	18.00	0	0	3	3
14	10.4	8	472.0	205	2.93	5.250	17.98	0	0	3	4
15	10.4	8	460.0	215	3.00	5.424	17.82	0	0	3	4
16	14.7	8	440.0	230	3.23	5.345	17.42	0	0	3	4
17	32.4	4	78.7	66	4.08	2.200	19.47	1	1	4	1
18	30.4	4	75.7	52	4.93	1.615	18.52	1	1	4	2
19	33.9	4	71.1	65	4.22	1.835	19.90	1	1	4	1
20	21.5	4	120.1	97	3.70	2.465	20.01	1	0	3	1
21	15.5	8	318.0	150	2.76	3.520	16.87	0	0	3	2
22	15.2	8	304.0	150	3.15	3.435	17.30	0	0	3	2
23	13.3	8	350.0	245	3.73	3.840	15.41	0	0	3	4
24	19.2	8	400.0	175	3.08	3.845	17.05	0	0	3	2
25	27.3	4	79.0	66	4.08	1.935	18.90	1	1	4	1
26	26.0	4	120.3	91	4.43	2.140	16.70	0	1	5	2
27	30.4	4	95.1	113	3.77	1.513	16.90	1	1	5	2
28	15.8	8	351.0	264	4.22	3.170	14.50	0	1	5	4
29	19.7	6	145.0	175	3.62	2.770	15.50	0	1	5	6
30	15.0	8	301.0	335	3.54	3.570	14.60	0	1	5	8
31	21.4	4	121.0	109	4.11	2.780	18.60	1	1	4	2
result_df = df1.drop(index=[11, 15])
print(result_df)
     mpg  cyl   disp   hp  drat     wt   qsec  vs  am  gear  carb
0   21.0    6  160.0  110  3.90  2.620  16.46   0   1     4     4
1   21.0    6  160.0  110  3.90  2.875  17.02   0   1     4     4
2   22.8    4  108.0   93  3.85  2.320  18.61   1   1     4     1
3   21.4    6  258.0  110  3.08  3.215  19.44   1   0     3     1
4   18.7    8  360.0  175  3.15  3.440  17.02   0   0     3     2
5   18.1    6  225.0  105  2.76  3.460  20.22   1   0     3     1
6   14.3    8  360.0  245  3.21  3.570  15.84   0   0     3     4
7   24.4    4  146.7   62  3.69  3.190  20.00   1   0     4     2
8   22.8    4  140.8   95  3.92  3.150  22.90   1   0     4     2
9   19.2    6  167.6  123  3.92  3.440  18.30   1   0     4     4
10  17.8    6  167.6  123  3.92  3.440  18.90   1   0     4     4
12  17.3    8  275.8  180  3.07  3.730  17.60   0   0     3     3
13  15.2    8  275.8  180  3.07  3.780  18.00   0   0     3     3
14  10.4    8  472.0  205  2.93  5.250  17.98   0   0     3     4
16  14.7    8  440.0  230  3.23  5.345  17.42   0   0     3     4
17  32.4    4   78.7   66  4.08  2.200  19.47   1   1     4     1
18  30.4    4   75.7   52  4.93  1.615  18.52   1   1     4     2
19  33.9    4   71.1   65  4.22  1.835  19.90   1   1     4     1
20  21.5    4  120.1   97  3.70  2.465  20.01   1   0     3     1
21  15.5    8  318.0  150  2.76  3.520  16.87   0   0     3     2
22  15.2    8  304.0  150  3.15  3.435  17.30   0   0     3     2
23  13.3    8  350.0  245  3.73  3.840  15.41   0   0     3     4
24  19.2    8  400.0  175  3.08  3.845  17.05   0   0     3     2
25  27.3    4   79.0   66  4.08  1.935  18.90   1   1     4     1
26  26.0    4  120.3   91  4.43  2.140  16.70   0   1     5     2
27  30.4    4   95.1  113  3.77  1.513  16.90   1   1     5     2
28  15.8    8  351.0  264  4.22  3.170  14.50   0   1     5     4
29  19.7    6  145.0  175  3.62  2.770  15.50   0   1     5     6
30  15.0    8  301.0  335  3.54  3.570  14.60   0   1     5     8
31  21.4    4  121.0  109  4.11  2.780  18.60   1   1     4     2
voldrop_df1 = result_df.drop("vs", axis=1)
voldrop_df1
mpg	cyl	disp	hp	drat	wt	qsec	am	gear	carb
0	21.0	6	160.0	110	3.90	2.620	16.46	1	4	4
1	21.0	6	160.0	110	3.90	2.875	17.02	1	4	4
2	22.8	4	108.0	93	3.85	2.320	18.61	1	4	1
3	21.4	6	258.0	110	3.08	3.215	19.44	0	3	1
4	18.7	8	360.0	175	3.15	3.440	17.02	0	3	2
5	18.1	6	225.0	105	2.76	3.460	20.22	0	3	1
6	14.3	8	360.0	245	3.21	3.570	15.84	0	3	4
7	24.4	4	146.7	62	3.69	3.190	20.00	0	4	2
8	22.8	4	140.8	95	3.92	3.150	22.90	0	4	2
9	19.2	6	167.6	123	3.92	3.440	18.30	0	4	4
10	17.8	6	167.6	123	3.92	3.440	18.90	0	4	4
12	17.3	8	275.8	180	3.07	3.730	17.60	0	3	3
13	15.2	8	275.8	180	3.07	3.780	18.00	0	3	3
14	10.4	8	472.0	205	2.93	5.250	17.98	0	3	4
16	14.7	8	440.0	230	3.23	5.345	17.42	0	3	4
17	32.4	4	78.7	66	4.08	2.200	19.47	1	4	1
18	30.4	4	75.7	52	4.93	1.615	18.52	1	4	2
19	33.9	4	71.1	65	4.22	1.835	19.90	1	4	1
20	21.5	4	120.1	97	3.70	2.465	20.01	0	3	1
21	15.5	8	318.0	150	2.76	3.520	16.87	0	3	2
22	15.2	8	304.0	150	3.15	3.435	17.30	0	3	2
23	13.3	8	350.0	245	3.73	3.840	15.41	0	3	4
24	19.2	8	400.0	175	3.08	3.845	17.05	0	3	2
25	27.3	4	79.0	66	4.08	1.935	18.90	1	4	1
26	26.0	4	120.3	91	4.43	2.140	16.70	1	5	2
27	30.4	4	95.1	113	3.77	1.513	16.90	1	5	2
28	15.8	8	351.0	264	4.22	3.170	14.50	1	5	4
29	19.7	6	145.0	175	3.62	2.770	15.50	1	5	6
30	15.0	8	301.0	335	3.54	3.570	14.60	1	5	8
31	21.4	4	121.0	109	4.11	2.780	18.60	1	4	2
for col in df1.columns:
        res = df1[col].value_counts()
        print(res)
10.4    2
21.4    2
30.4    2
22.8    2
15.2    2
19.2    2
21.0    2
18.1    1
32.4    1
14.7    1
21.5    1
15.5    1
15.8    1
17.8    1
27.3    1
26.0    1
19.7    1
15.0    1
18.7    1
16.4    1
33.9    1
24.4    1
14.3    1
17.3    1
13.3    1
Name: mpg, dtype: int64
8    14
4    11
6     7
Name: cyl, dtype: int64
275.8    3
160.0    2
167.6    2
360.0    2
400.0    1
108.0    1
258.0    1
225.0    1
472.0    1
460.0    1
440.0    1
318.0    1
304.0    1
350.0    1
78.7     1
79.0     1
120.3    1
145.0    1
301.0    1
121.0    1
75.7     1
95.1     1
140.8    1
146.7    1
71.1     1
120.1    1
351.0    1
Name: disp, dtype: int64
175    3
180    3
110    3
123    2
66     2
150    2
245    2
97     1
65     1
230    1
91     1
264    1
105    1
95     1
205    1
62     1
52     1
113    1
109    1
215    1
93     1
335    1
Name: hp, dtype: int64
3.07    3
3.92    3
2.76    2
3.15    2
3.08    2
4.08    2
4.22    2
3.90    2
4.43    1
3.00    1
3.73    1
3.21    1
4.11    1
3.85    1
3.69    1
3.54    1
4.93    1
3.23    1
3.77    1
3.70    1
3.62    1
2.93    1
Name: drat, dtype: int64
3.440    3
3.570    2
2.780    1
3.520    1
5.250    1
5.345    1
2.140    1
3.845    1
3.780    1
1.835    1
3.435    1
1.935    1
5.424    1
2.465    1
1.615    1
1.513    1
2.200    1
2.620    1
4.070    1
2.320    1
3.215    1
3.460    1
2.770    1
3.150    1
3.190    1
3.730    1
3.170    1
3.840    1
2.875    1
Name: wt, dtype: int64
17.02    2
18.90    2
18.52    1
17.60    1
18.00    1
14.50    1
16.87    1
20.01    1
17.05    1
15.50    1
18.61    1
17.98    1
19.47    1
15.41    1
22.90    1
16.46    1
18.30    1
17.40    1
19.90    1
19.44    1
16.90    1
20.22    1
15.84    1
17.82    1
16.70    1
17.30    1
17.42    1
14.60    1
18.60    1
20.00    1
Name: qsec, dtype: int64
0    18
1    14
Name: vs, dtype: int64
0    19
1    13
Name: am, dtype: int64
3    15
4    12
5     5
Name: gear, dtype: int64
4    10
2    10
1     7
3     3
8     1
6     1
Name: carb, dtype: int64
df5 = pd.read_csv(r'C:\Users\ADMIN\Downloads\bank-full.csv')
data_top = df5.head()
list(df5.columns)
['age;"job";"marital";"education";"default";"balance";"housing";"loan";"contact";"day";"month";"duration";"campaign";"pdays";"previous";"poutcome";"y"']
from sklearn.preprocessing import LabelEncoder   # import label encoder

labelencoder = LabelEncoder()
df_dummies = pd.DataFrame(df5, columns= ['age;"job";"marital";"education";"default";"balance";"housing";"loan";"contact";"day";"month";"duration";"campaign";"pdays";"previous";"poutcome";"y"'])
# df_dummies= pd.get_dummies(df5, prefix='DF', columns= ['age;"job";"marital";"education";"default";"balance";"housing";"loan";"contact";"day";"month";"duration";"campaign";"pdays";"previous";"poutcome";"y"'])
df_dummies['age;"job";"marital";"education";"default";"balance";"housing";"loan";"contact";"day";"month";"duration";"campaign";"pdays";"previous";"poutcome";"y"'] = labelencoder.fit_transform(df_dummies['age;"job";"marital";"education";"default";"balance";"housing";"loan";"contact";"day";"month";"duration";"campaign";"pdays";"previous";"poutcome";"y"']) # returns label encoded variable(s)
print(df5)
df5.columns.tolist()
      age;"job";"marital";"education";"default";"balance";"housing";"loan";"contact";"day";"month";"duration";"campaign";"pdays";"previous";"poutcome";"y"
0      58;"management";"married";"tertiary";"no";2143...                                                                                                  
1      44;"technician";"single";"secondary";"no";29;"...                                                                                                  
2      33;"entrepreneur";"married";"secondary";"no";2...                                                                                                  
3      47;"blue-collar";"married";"unknown";"no";1506...                                                                                                  
4      33;"unknown";"single";"unknown";"no";1;"no";"n...                                                                                                  
...                                                  ...                                                                                                  
45206  51;"technician";"married";"tertiary";"no";825;...                                                                                                  
45207  71;"retired";"divorced";"primary";"no";1729;"n...                                                                                                  
45208  72;"retired";"married";"secondary";"no";5715;"...                                                                                                  
45209  57;"blue-collar";"married";"secondary";"no";66...                                                                                                  
45210  37;"entrepreneur";"married";"secondary";"no";2...                                                                                                  

[45211 rows x 1 columns]
['age;"job";"marital";"education";"default";"balance";"housing";"loan";"contact";"day";"month";"duration";"campaign";"pdays";"previous";"poutcome";"y"']
Basic Programs
#Write Python Programs to use various operators in Python

#Arithmetic operators in Python
x = 15
y = 4

# Output: x + y = 19
print('x + y =',x+y)

# Output: x - y = 11
print('x - y =',x-y)

# Output: x * y = 60
print('x * y =',x*y)

# Output: x / y = 3.75
print('x / y =',x/y)

# Output: x // y = 3
print('x // y =',x//y)

# Output: x ** y = 50625
print('x ** y =',x**y)
#Comparison operators
x = 10
y = 12

# Output: x > y is False
print('x > y is',x>y)

# Output: x < y is True
print('x < y is',x<y)

# Output: x == y is False
print('x == y is',x==y)

# Output: x != y is True
print('x != y is',x!=y)

# Output: x >= y is False
print('x >= y is',x>=y)

# Output: x <= y is True
print('x <= y is',x<=y)
#Logical Operators
x = True
y = False

print('x and y is',x and y)

print('x or y is',x or y)

print('not x is',not x)
#Assignment operators
#a = 5 is a simple assignment operator that assigns the value 5 on the right to the variable a on the left.
#Identity operators in Python
x1 = 5
y1 = 5
x2 = 'Hello'
y2 = 'Hello'
x3 = [1,2,3]
y3 = [1,2,3]

# Output: False
print(x1 is not y1)

# Output: True
print(x2 is y2)

# Output: False
print(x3 is y3)
#Membership operators 
x = 'Hello world'
y = {1:'a',2:'b'}

# Output: True
print('H' in x)

# Output: True
print('hello' not in x)

# Output: True
print(1 in y)

# Output: False
print('a' in y)
#Create list of elements and slice and dice it
a = ("a", "b", "c", "d", "e", "f", "g", "h")
x = slice(2)
print(a[x])
#Using while loop accept numbers until sum of numbers is less than 100
total_sum = 0
a = int(input())
while a != 0:
    total_sum += a
    if total_sum >= 21:
        print('Total sum is', total_sum)
        break
    a = int(input())
else:
    print('Total sum is less than 21 and is equal to', total_sum, '.')
#Write a python program Read & write Excel files 
import openpyxl
my_wb = openpyxl.Workbook()
my_sheet = my_wb.active
c1 = my_sheet.cell(row = 1, column = 1)
c1.value = "Aadrika"
c2 = my_sheet.cell(row= 1 , column = 2)
c2.value = "Adwaita"
c3 = my_sheet['A2']
c3.value = "Satyajit"
# B2 = column = 2 & row = 2.
c4 = my_sheet['B2']
c4.value = "Bivas"
my_wb.save("C:\Users\TP\Desktop\Book1.xlsx")
#Create a 3x3 matrix with values ranging from 2 to 10 using numpy

xr =  np.arange(2, 11).reshape(3,3)
print(x)
#Write a Python program to convert a list of numeric value into a one-dimensional NumPy array
l = [12.23, 13.32, 100, 36.32]
print("Original List:",l)
a = np.array(l)
print("One-dimensional NumPy array: ",a)
#Write a Python program to create a null vector of size 10 and update sixth value to 11.
x = np.zeros(10)
print(x)
print("Update sixth value to 11")
x[6] = 11
print(x)
