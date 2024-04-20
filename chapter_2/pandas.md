## pandas の良さ

表データを扱える。<br>
DataFrame で計算すると、それぞれのカラムごとに計算されるため、カラム同士の特性の比較がしやすい。

```python
# numeric_dataはDataFrameオブジェクト
numeric_data = student_data_math.select_dtypes(include=[np.number])
numeric_data.std(ddof=0) / numeric_data.mean()

age           0.076330
Medu          0.397673
Fedu          0.431019
traveltime    0.481058
studytime     0.411791
...
dtype: float64
```
