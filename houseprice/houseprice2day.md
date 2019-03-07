# 住宅価格予想コンペティションの日記

## 2日目取り組んだこと、気づき、学び
- １日目の続きを主にやっていた。データの欠損値の扱いなどをfillnaメソッドなどを用いて行なっていた。
- pandasのDataFrameではlocとilocは列だけの指定はできない。
- 以下のやつはiloc,locどちらでも良い
- できるやつdata.iloc[row], data.iloc[row, col], data.iloc[[row1, row2]], data.iloc[[row1, row2], [col1, col2]]、etc..
- できないやつdata.iloc[col], data.iloc[[col1, col2]]
- groupbyメソッドを理解するのに時間がかかった。あとtransdormメソッドも...
- df[カラム] = df.groupby(グループ化できそうなカラム)
- example: df['col'] のvalueが['a', 'a', 'b', 'c', 'b']こんな感じのやつを上のグループ化できそうなカラムに指定したら良い

## 感想
今日はあまり進捗があまり出なかった。しかし今まで名前だけは知っていたメソッドをより深く知ることができたので良しとする。
