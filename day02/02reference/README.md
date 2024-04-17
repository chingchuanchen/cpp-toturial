# 引用

* 引用即别名
```c++
  int a = 10;
  int& b = a;
  int& c = b;
```
* 引用必须初始化
```c++
  int& b; // error
  int& b = a;
  const int& b = 10;
```
* 引用不能为空
* 引用不能更换目标

注意：
变量名如`a`，`b`是高级语言的概念。
代码经过编译后，所有的操作都是通过地址，根本没有所谓的变量名，因此也就没有变量名存哪里的这种说法。
因为通过地址操作更复杂，更重要的编译后根本不知道地址在哪里，所以写代码时就用变量名代替地址操作变量。

* 引用型参数，函数的形参是实参的别名
    * 在函数中修改实参值
    * 避免对象复制开销
* 常应用型参数
    * 接受常量型实参
    * 防止对实参的意外修改