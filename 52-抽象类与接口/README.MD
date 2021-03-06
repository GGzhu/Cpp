什么是抽象类：
.面向对象中的抽象概念
  在进行面向对象分析时，会发现一些抽象的概念！
  在现实中需要知道具体的图形类型才能求面积，所以对概念上的“图形”
  求面积时没有意义的！
 
面向对象中的抽象类：
  -可用于表示现实世界中的抽象概念
  -是一种只能定义类型，而不能产生对象的类
  -只能被继承并重写相关函数
  -直接特征是相关函数没有完整的实现

抽象类与纯虚函数：
  -C++语言中没有抽象类的概念
  -C++中通过纯虚函数实现抽象类
  -纯虚函数是指只定义原型的成员函数
  --个C++类中存在纯虚函数就成为抽象类

纯虚函数的语法规则：
class Shape
{
public:
    virtual double area() = 0;
};

  "=0"用于告诉编译器当前是声明纯虚函数，因此不需要定义函数体
.抽象类只能用作父类被继承
.子类必须实现纯虚函数的具体功能
.纯虚函数被实现后成为虚函数
.如果子类没有实现纯虚函数，则子类成为抽象类

.满足下面条件的C++类则称为接口
  -类中没有定义任何的成员变量
  -所有的成员函数都是公有的
  -所有的成员函数都是纯虚函数
  -接口时一种特殊的抽象类

小结：
1.抽象类用于描述现实世界中的抽象概念
2.抽象类只能被继承不能被创建对象
3.C++中没有抽象类的概念
4.C++中通过纯虚函数实现抽象类
5.类中只存在纯虚函数的时候成为接口
6.接口时一种特殊的抽象类


