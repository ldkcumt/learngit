# [知识点]

<b><details><summary>1.结构体与类的区别</summary></b> 

* 分别以struct和class命名

* 成员访问控制有差异，默认情况下，结构体的成员是public，类的成员是private

</details>

<b><details><summary>2.C++的特性?</summary></b> 

> 类与对象
>> 类是抽象的，对象是类的实例

> 构造函数
>> 
- 构造函数的名字和类名相同，没有返回值
- 构造函数用来对类中的成员变量进行初始化

> 析构函数
>>
- 释放对象所占有的资源
- 反向的构造函数，不允许有返回值
- 不能带参数，一个类中有且只有一个析构函数

> 函数的重载 overload
>>
- 有多个构造函数，函数名一样，只是参数的类型和个数不一样
- 只有函数的返回类型不同是不能构成函数的重载

> this指针
>>
- 是一个隐含的指针
- 指向对象本身，代表对象的地址

> 类的继承
>>
- 父类和子类，子类除了自己的成员变量和方法外，还可以继承父类的成员变量和方法
- public：可以在任何地方被访问
- protected：只能在该类及其子类中访问
- Private：只能在该类中访问

> 多重继承
>>
- 一个类可以从多个基类中派生
- 多个基类中若有相同的变量和方法，可能会带来麻烦

> 虚函数与多态
>>在基类的函数前加上virtual关键字，在派生类中重写该函数，运行时将会根据对象的实际类型类调用相应的函数。如果对象类型是派生类，就调用派生类的函数；如果对象类型是基类，就调用基类的函数。

> 纯虚函数
>>
- 不具体实现的虚函数
- 含有纯虚函数的类叫抽象类，这种类不能声明对象，只是作为基类为派生类服务
- 派生类中必须完全实现基类的纯虚函数，否则，派生类也变成了抽象类，不能实例化对象。

> 函数的覆盖
>>
- 基类函数必须是虚函数
- 发生覆盖的两个函数要分别位于派生类和基类中
- 函数名称与参数必须完全相同
- 覆盖总是和多态关联在一起

> 函数的隐藏
>>
- 派生类的函数与基类函数完全相同，即函数名和参数都相同，只是基类函数没有使用virtual关键字，此时基类函数将被隐藏
- 派生类函数与基类函数同名，但参数不同，不管基类的函数是否有virtual关键字，基类函数都将被隐藏

> 引用和指针变量
>>
- 引用就是一个变量的别名
- 指针是地址，指针变量要存储地址值，可以修改指针变量所保存的地址值，从而指向其他的内存

</details>

<b><details><summary>3.Const char* 和 char* const</summary></b> 
- Const char* 指向常量的指针
- Char* const 指针常量

</details>

<b><details><summary>4.进程间通信方式</summary></b> 
- 剪贴板
- 匿名管道
- 命名管道
- 邮槽

</details>

<b><details><summary>5.线程同步</summary></b> 
- 利用事件对象实现线程同步
- 利用关键代码段实现线程同步
- 线程锁

</details>

<b><details><summary>6.指针</summary></b> 
- 一个整型数

    int a;

- 一个指向整型数的指针（A pointer to an integer）

    int *a;

- 一个指向指针的的指针，它指向的指针是指向一个整型数( A pointer to a pointer to an intege)

    int **a;

- 一个有10个整型数的数组( An array of 10 integers) 

    int a[10];

- 一个有10个指针的数组，该指针是指向一个整型数的。(An array of 10 pointers to integers) 

    int *a[10];

- 一个指向有10个整型数数组的指针( A pointer to an array of 10 integers)

    int (*a)[10];

- 一个指向函数的指针，该函数有一个整型参数并返回一个整型数(A pointer to a function that takes an integer as an argument and returns an integer) 

    int (*a)(int);

- 一个有10个指针的数组，该指针指向一个函数，该函数有一个整型参数并返回一个整型数( An array of ten pointers to functions that take an integer argument and return an integer )

    int (*a[10])(int)

</details>

# [测试题]

<b><details><summary>一个指向整型数的指针</summary></b> 

    分别以struct和class命名

</details>
