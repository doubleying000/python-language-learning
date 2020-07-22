## 1.变量、运算符与数据类型
### Q1. python中代码的基本注释
#### 单行注释：# ``` 位于注释行的行首```
#### 多行注释： ''' ''' 或 """ """ ```引号间的所有内容被注释```
```python
【例子】
print("Hello World")
# Hello World
print('This is Python')

""" 
Hello World 
Hello China
Hello Python
"""
```




### Q2. python中的运算符及其优先级
#### 运算符类型：算术运算符、比较运算符、逻辑运算符、位运算符、其他运算符
#### 运算符的优先级
##### 一级运算符优于二级运算符
##### 先算术运算，后移位运算，最后位运算
##### 逻辑运算最后结合




### Q3. python中``` is, is not ``` 与 ``` ==，!= ```的区别
#### 名称不同
操作符类型 | 操作符 | 名称 | 示例
:---:|:---:|:---:|:---:
比较运算符|`is`|是| `"hello" is "hello"`
比较运算符|`is not`|不是|`"hello" is not "hello"`
其他运算符|`==`|等于| `3==3`
其他运算符|`！=`|不等于|`3！=5`

#### 对比变量不同
操作符 | 对比变量 | 示例
:---:|:---:|:---:
`is``is not`|变量的内存地址
`==``！=`|变量的值

注：
- 当比较的两个变量，指向的都是地址不可变的类型（str等），那么is，is not 和 ==，！= 是完全等价的。
- 对比的两个变量，指向的是地址可变的类型（list，dict等），则两者是有区别的。
```python
【例子】比较的两个变量均指向不可变类型。
a = "hello"
b = "hello"
print(a is b, a == b)  # True True
print(a is not b, a != b)  # False False

【例子】比较的两个变量均指向可变类型。
a = ["hello"]
b = ["hello"]
print(a is b, a == b)  # False True
print(a is not b, a != b)  # True False
```




### Q4. python中包含的数据类型及其转换

数据类型 | 名称 | 示例
:---:|:---:|:---:
int | 整型 `<class 'int'>`| `25, 8`
float | 浮点型`<class 'float'>`| `0.52, 3.23`
bool | 布尔型`<class 'bool'>` | `True, False`

数据类型间的转换

- 转换为整型 `int(x, base=10)`
- 转换为字符串 `str(object='')`
- 转换为浮点型 `float(x)`





