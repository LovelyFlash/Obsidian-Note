---
title: volatile 和 mutable
date created: 星期三, 十月 22日 2025, 5:30:37 下午
date modified: 星期三, 十月 22日 2025, 9:22:48 晚上
---

# 1 `volatile`

volatile：不稳定的、易挥发的、变化无常的
- 变量可能会被意想不到的改变； 
- 优化器不对该变量的读取进行优化，用到该变量时重新读取；
- 修饰的变量可由操作系统、硬件、并发执行的线程在程序中进行修改。

以下情况下，应在变量前加 volatile：
- 多任务环境下，各任务间共享的变量；
- 中断服务程序中修改的供其他程序检测的变量；
- 存储器映射的硬件寄存器。

构造或析构函数和静态函数成员的参数表后不能出现 const 或 volatile。

# 2 `mutable`

mutable：可变的
- 是 const 的反义词，为突破 const 的限制而设计；
- 只能用来修饰数据成员，使其永远处于可变得状态；
- 不能与 const、volatile 或 static 同时出现。

```C++
class A {
	int x;
	static int y; 
	mutable int z; 
public:
	void f() const { 
		x = x + 1; // 编译时报错，无法修改 x 
		y = 20; // 无误，静态成员在 const 成员函数中可以修改
		z = 30; // 无误，z 被 mutable 修饰
	} 
};
```

# 3 对函数的影响

参数表后出现 const、volatile 或 const volatile 会影响函数成员的重载： 
- 普通对象应调用参数表后不带 const 和 volatile 的函数成员；
- const 和 volatile 对象应分别调用参数表后出现 const 和 volatile 的函数成员。 
参数表后出现 volatile，表示调用函数成员的对象是<font color="#ff0000">挥发对象</font>，意味存在<font color="#ff0000">并发执行</font>的进程，正在修改当前对象。

```C++
classDate{
private: 
	int year, month, day;
public:
	Date(intyear, intmonth, intday) {
		this->year = year; 
		this->month = month; 
		this->day = day; 
	}
	voidModifyYear(intyear) {
		this->year = year; 
	}
	voidDisplayYear() const {   
		cout << year << endl; 
	}
	voidDisplayMonth() { 
		cout << month << endl; 
	} 
};

constDatenational_day(1949, 10, 1);
national_day.DisplayYear();
national_day.ModifyYear(1948); // error
national_day.DisplayMonth( ); // error
```

```C++
class A {
	int a;
public:
	int f() {
		a++; return a;
	} // this 类型为 A* const this
	int f( ) const {
		return a; 
	} // this 类型为：const A* const this
	int f( ) volatile {
		return a++; 
	} // this 类型为：volatile A * const this**
	int f() const volatile {
		return a;
	} // this 类型为：const volatile
}
```
