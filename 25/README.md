-----------------------类的静态成员变量-----------------

1.成员变量的回顾
.通过对象名能够访问public成员变量
.每个对象的成员变量都是专属的
.成员变量不能在对象之间共享


2.新需求
.统计在程序运行期间某个类的数目
.保证程序的安全性（不能使用全局变量）
.随时可以获取当前对象的数目

3.静态成员变量
-静态成员变量属于整个类所有
-静态成员变量的生命周期不依赖于任何对象
-可以通过类名直接访问公有静态成员变量
-所有对象共享类的静态成员变量
-可以通过对象名访问公有静态成员变量

.静态成员变量的特性
-在定义时直接通过static关键字修饰
-静态成员变量需要在类外单独分配空间
-静态成员变量在程序内部位于全局数据区（与静态局部变量，全局变量一样）
.语法规则：
static Type ClassName::VarName = value;

4.小结
.类中可以通过static关键字定义静态成员变量
.静态成员变量隶属于类所有
.每一个对象都可以访问静态成员变量
.静态成员变量在全局数据区分配空间
.静态成员变量的生命周期为程序运行期 
