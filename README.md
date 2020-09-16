
# 1.缩进
4个空格的缩进（编辑器都可以完成此功能），不要使用Tap，更不能混合使用Tap和空格。

# 2.变量命名
变量名只能包含字母、数字和下划线。

变量名不能包含空格。

变量名应既简短又具有描述性。

切勿将字符“ l”，“ O”或“ I”用作单个字符变量名称。

# 3.每行最多字符数

每行最大长度120，换行可以使用反斜杠，最好使用圆括号。换行点要在操作符的后边敲回车。

# 4.函数最大行数

一个函数最多为50行。

# 5.函数、类命名
## 总体原则，新编代码必须按下面命名风格进行，现有库的编码尽量保持风格

1.函数命名使用全部小写的方式，可以使用下划线。

2.类的属性（方法和变量）命名使用全部小写的方式，可以使用下划线。

3.类的属性有3种作用域public、non-public和subclass API，可以理解成C++中的public、private、protected，non-public属性前，前缀一条下划线。

4.类的属性若与关键字名字冲突，后缀一下划线，尽量不要使用缩略等其他方式。

5.为避免与子类属性命名冲突，在类的一些属性前，前缀两条下划线。比如：类Foo中声明__a,访问时，只能通过Foo._Foo__a，避免歧义。如果子类也叫Foo，那就无能为力了。

# 6.常量
常量通常在模块级别定义，并以所有大写字母书写，并用下划线分隔单词。示例包括 MAX_OVERFLOW和TOTAL。

# 7.空行规则
1.类和top-level函数定义之间空两行；类中的方法定义之间空一行；函数内逻辑无关段落之间空一行；其他地方尽量不要再空行。

2.不要将多句语句写在同一行，尽管使用‘；’允许。

3.if/for/while语句中，即使执行语句只有一句，也必须另起一行。

# 8.注释规则
## 总体原则，错误的注释不如没有注释。所以当一段代码发生变化时，第一件事就是要修改注释！
注释必须使用英文，最好是完整的句子，首字母大写，句后要有结束符，结束符后跟两个空格，开始下一句。如果是短语，可以省略结束符。

1.块注释，在一段代码前增加的注释。在‘#’后加一空格。段落之间以只有‘#’的行间隔。

2.行注释，在一句代码后加注释。比如：x = x + 1 # Increment x

3.避免无谓的注释。

# 9.操作符前后空格
## 总体原则，避免不必要的空格。
1 各种右括号前不要加空格。

2 逗号、冒号、分号前不要加空格。

3 函数的左括号前不要加空格。

4 序列的左括号前不要加空格。

5 操作符左右各加一个空格，不要为了对齐增加空格。

6 函数默认参数使用的赋值符左右省略空格。

# 10.其他规则

1. 为所有的共有模块、函数、类、方法写docstrings；非共有的没有必要，但是可以写注释（在def的下一行）。

2. 应该以不损害Python其他实现（PyPy，Jython，IronPython，Cython，Psyco等）的方式编写代码

3.与单例（如None）的比较应该始终使用 is或not进行，永远不要使用相等运算符进行

4.使用不是运算符，而不是...不是。虽然两个表达式在功能上都相同，但前者更易读和首选
