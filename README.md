# PandasLearning-Nullvalues
learn pandas nullvalues
pandas 中缺失值 处理
一、（丢弃缺失值）
dropna四种参数：
1、axis ：参数用于控制行或列，跟其他不一样的是，axis=0 （默认）表示操作行，axis=1 表示操作列。
2、subset ：参数表示删除时只考虑的索引或列名
3、how ：参数可选的值为 any（默认） 或者 all。any 表示一行/列有任意元素为空时即丢弃，all 一行/列所有值都为空时才丢弃。
4、thresh :如thresh=3，会在一行/列中至少有三个非空值时将其保留

二、（填充缺失值）
fillna
1、
2、标量填充：fillna(0)

3、前后值填充
前值：fillna(method="ffill")
后值：fillna(method="bfill")or(method="backfill")
线性差值：interpolate
