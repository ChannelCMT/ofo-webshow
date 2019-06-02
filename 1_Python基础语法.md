
## Python基础语法

### 1、Python编程模式
**交互式:**

命令逐条运行

交互式编程不需要创建脚本文件，是通过 Python 解释器的交互模式进来编写代码。


```python
print("hello world")
```

    hello world
    


```python
>>> 1+1
```




    2




```python
>>> a=1
>>> b=1
>>> a+b
```




    2



**脚本式:**

一次性全部运行

通过脚本参数调用解释器开始执行脚本，直到脚本执行完毕。当脚本执行完成后，解释器不再有效。


```python
my_dream='I want to be a quantitative trader.'
print('Hello,world!!! '+my_dream)
print (my_dream + ' What can I do?')
#点击run,显示运行结果:
```

    Hello,world!!! I want to be a quantitative trader.
    I want to be a quantitative trader. What can I do?
    

## 2、 Python标识符

在 Python 里，标识符由字母、数字、下划线组成。

在 Python 中，所有标识符可以包括英文、数字以及下划线_，但不能以数字开头。

Python 中的标识符是区分大小写的。

Python 可以同一行显示多条语句，方法是用分号 ;


```python
1A_ = 1
print(1A_)
```


      File "<ipython-input-8-837b4d511801>", line 1
        1A_ = 1
          ^
    SyntaxError: invalid syntax
    



```python
A1_ = 1
print(A1_)
```

    1
    


```python
a1_ = 2
print(a1_)
```

    2
    


```python
A = 1; a=2
```


```python
print(A,a)
```

    1 2
    

## 3、 Python 保留字符
下面的列表显示了在Python中的保留字。这些保留字不能用作常数或变数，或任何其他标识符名称。

所有 Python 的关键字只包含小写字母。

|||
|:-----:|:-----:|:-----:|
|and|exec|not|
|assert|finally|or|
|break|for|pass|
|class|from|print|
|continue|global|raise|
|def|if|return|
|del|import|try|
|elif|in|while|
|else|is|with|
|except|lambda|yield|

### 4、代码缩进问题:

缩进替代({})

学习Python与其他语言最大的区别就是，Python的代码块不使用大括号（{}）来控制类，函数以及其他逻辑判断。 
python最具特色的就是用缩进来写模块。

### 代码缩进（错误）


```python
price = 1
if price>0:
    print ('True')
        print ('price is greater than 0')
        # 没有严格缩进，在执行时会报错
else:
    print ("False")
```

### 代码缩进（正确）


```python
price = 1
if price>0:
    print ('True')
    print ('price is greater than 0')
else:
    print ("False")
```

### 4、 多行语句处理
Python语句中一般以新行作为语句的结束符。

但是我们可以使用斜杠（ \）将一行的语句分为多行显示，如下所示：


```python
Price = 1+\
        2+\
        3
```


```python
print(Price)
```

    6
    

### 5.Python 引号
Python 可以使用引号( ' )、双引号( " )、三引号( ''' 或 """ ) 来表示字符串，引号的开始与结束必须的相同类型的。

其中三引号可以由多行组成，被当做注释。 


```python
Name = 'Channel'
Career = "Quantitative Trader"
Habit = '''Poppin'''

print(Name+" is "+Career+' who like '+Habit)
```

    Channel is Quantitative Trader who like Poppin
    


```python
def annotation():
    """
    Channel is Quantitative 
    Trader who like Poppin
    """
    annotated = """被注释"""
    return annotated
print(annotation())
```

    被注释
    

### 6、注释代码

单行注释用 # 开头

多行注释用三个引号(''')

代码注释有一个功能在于可以在写代码时跳过不想运行的行


```python
# 宽客你好
# print('hello quant')
```


```python
# 宽客你好
print('hello quant')
```

    hello quant
    


```python
print('hello quant') # 宽客你好
```

    hello quant
    


```python
"""
宽客你好
print('hello quant')
"""

print("OK, Let's code")
```

    OK, Let's code
    
