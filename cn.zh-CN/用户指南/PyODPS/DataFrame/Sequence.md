# Sequence {#concept_ddr_lv4_cfb .concept}

[SequenceExpr](intl.zh-CN/用户指南/PyODPS/API Reference/API概述.md#)代表了二维数据集中的一列。您不需要手动创建SequenceExpr，而是从一个Collection中获取。

## 获取列 {#section_gvy_ks4_cfb .section}

您可以使用collection.column\_name取出一列，例如

```
iris.sepallength.head(5)
   sepallength
0          5.1
1          4.9
2          4.7
3          4.6
4          5.0
```

如果列名存储在一个字符串变量中，除了使用getattr\(df, ‘column\_name’\)达到相同的效果外，也可以使用 df\[column\_name\]的形式，例如

```
iris['sepallength'].head(5)
   sepallength
0          5.1
1          4.9
2          4.7
3          4.6
4          5.0
```

## 列类型 {#section_avk_4s4_cfb .section}

DataFrame包括自己的类型系统，在使用Table初始化的时候，ODPS的类型会被进行转换。这样做的好处是，能支持更多的计算后端。 目前，DataFrame的执行后端支持ODPS SQL、pandas以及数据库（MySQL和Postgres）。

PyODPS DataFrame包括以下类型：

`int8`，`int16`，`int32`，`int64`，`float32`，`float64`，`boolean`，`string`，`decimal`，`datetime`，`list`，`dict`

ODPS的字段和DataFrame的类型映射关系如下：

|ODPS类型|DataFrame类型|
|:-----|:----------|
|bigint|int64|
|double|float64|
|string|string|
|datetime|datetime|
|boolean|boolean|
|decimal|decimal|
|array<value\_type\>|list<value\_type\>|
|map<key\_type, value\_type\>|dict<key\_type, value\_type\>|

list和dict必须填写其包含值的类型，否则会报错。目前DataFrame暂不支持MaxCompute 2.0中新增的Timestamp及Struct 类型，未来的版本会支持。

在Sequence中可以通过sequence.dtype获取数据类型：

```
iris.sepallength.dtype
float64
```

如果要修改一列的类型，可以使用astype方法。该方法输入一个类型，并返回类型转换后的Sequence。例如，

```
iris.sepallength.astype('int')
   sepallength
0            5
1            4
2            4
3            4
4            5
```

## 列名 {#section_qzd_5s4_cfb .section}

在DataFrame的计算过程中，一个Sequence必须要有列名。在很多情况下，DataFrame会起一个名字。比如：

```
iris.groupby('name').sepalwidth.max()
   sepalwidth_max
0             4.4
1             3.4
2             3.8
```

可以看到，`sepalwidth`取最大值后被命名为`sepalwidth_max`。还有一些操作，比如一个Sequence做加法，加上一个Scalar，这时，会被命名为这个Sequence的名字。其它情况下，需要用户去自己命名。

Sequence提供rename方法对一列进行重命名，用法示例如下：

```
iris.sepalwidth.rename('sepal_width').head(5)
   sepal_width
0          3.5
1          3.0
2          3.2
3          3.1
4          3.6
```

## 简单的列变换 {#section_uzf_xs4_cfb .section}

您可以对一个Sequence进行运算，返回一个新的Sequence，正如对简单的Python变量进行运算一样。对数值列， Sequence支持四则运算，而对字符串则支持字符串相加等操作。例如，

```
(iris.sepallength + 5).head(5)
   sepallength
0         10.1
1          9.9
2          9.7
3          9.6
4         10.0
```

而

```
(iris.sepallength + iris.sepalwidth).rename('sum_sepal').head(5)
   sum_sepal
0        8.6
1        7.9
2        7.9
3        7.7
4        8.6
```

注意到两列参与运算，因而PyODPS无法确定最终显示的列名，需要手动指定。详细的列变换说明，请参见[列运算](intl.zh-CN/用户指南/PyODPS/DataFrame/列运算.md#)。

