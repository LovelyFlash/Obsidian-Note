---
title: const修饰符
date created: 星期六, 十月 18日 2025, 7:12:52 晚上
date modified: 星期三, 十月 22日 2025, 5:08:55 下午
---

`const` 是 C++ 中一个非常重要的关键字，意为“常量”或“不可变”。它的核心目的是**强制执行不可变性 (Immutability)**，从而提高代码的安全性、可读性，并允许编译器进行更积极的优化。

# 1 `const` 的核心作用

`const` 的基本原则是：**一旦被** `const` **修饰，就不能被修改。** 编译器会强制执行这一约束。

# 2 `const` 的使用场景

`const` 可以修饰变量、指针、引用、函数参数、函数返回值以及类的成员函数。

# 2.1 修饰变量

常量变量：定义一个值不能被改变的变量。必须在声明时初始化。
`const` 的位置：`const` 可以在类型前或类型后，效果相同。
  
```C++
const int MAX_VALUE = 100; // MAX_VALUE 是一个常量，不能被修改
// MAX_VALUE = 200; // 错误
int const MIN_VALUE = 0; // 与 const int MIN_VALUE = 0; 相同
```

## 2.2 修饰指针

修饰指针时，`const` 的位置决定了是**指针本身**是常量，还是**指针指向的数据**是常量。

可以将一个指针赋给一个常量指针，但不能将一个常量指针赋给一个指针

**1. 指向常量的指针：** 数据是常量，指针可以改变。
`const int* ptr;` 或 `int const* ptr;`
指针 `ptr` 可以指向不同的 int 变量，但不能通过 ptr 来修改它所指向的 int 变量的值。

```C++
int a = 10, b = 20;
const int* ptr = &a; // ptr 指向常量 int
// *ptr = 15; // 错误：不能通过 ptr 修改 a 的值
ptr = &b;    // OK：ptr 可以指向另一个变量
  ```

**2. 常量指针：** 指针本身是常量，不能改变指向，但指向的数据可以改变。
`int* const ptr;`
指针 `ptr` 一旦初始化，就不能再指向其他变量，但可以通过 `ptr` 来修改它所指向的 `int` 变量的值。

```C++
int a = 10, b = 20;
int* const ptr = &a; // ptr 是一个常量指针，必须初始化
*ptr = 15; // OK：可以通过 ptr 修改 a 的值
// ptr = &b; // 错误：ptr 是常量，不能改变指向
```
  
**3. 指向常量的常量指针：** 指针和它指向的数据都是常量。
`const int* const ptr;`
既不能通过 ptr 修改数据，也不能改变 ptr 的指向。

  ```C++
int a = 10;
const int* const ptr = &a;
// *ptr = 15; // 错误
// ptr = &b; // 错误
```
  

## 2.3 修饰引用

**常量引用 (Reference to const)：** 引用所绑定的数据是常量，不能通过引用修改数据。
`const int& ref = x;`
**重要特性：** const 引用可以绑定到**左值**，也可以绑定到**右值**（临时对象），并且在绑定到右值时会延长右值的生命周期。
  
```C++
int a = 10;
const int& ref = a; // ref 绑定到 a，不能通过 ref 修改 a
// ref = 15; // 错误
const int& temp_ref = 20; // OK：const 引用可以绑定到右值 20
  ```

  

## 2.4 修饰函数参数

**防止函数修改参数：** 当参数以 const 引用或 const 指针传递时，函数内部不能修改该参数所指向或引用的数据。
**优势：** 提高函数安全性，明确函数意图，避免不必要的拷贝（对于大对象）。

  ```C++
void printValue(const int& value) {
    // value = 10; // 错误：不能修改 const 引用
    std::cout << value << std::endl;
}

void processData(const std::vector<int>* data) {
    // (*data)[0] = 5; // 错误：不能通过 const 指针修改数据
}
  ```

## 2.5 修饰函数返回值

**返回常量值：** 函数返回一个 const 值。
**目的：** 防止对函数返回的临时对象进行修改。
**注意：** 对于按值返回，通常是多余的，因为临时对象本身不能被修改。对于返回引用或指针，const 才有实际意义。

```C++
const std::string getGreeting() {
    return "Hello";
}
// getGreeting() = "Hi"; // 错误：不能修改 const 返回值
  ```

## 2.6 修饰成员函数 (const 成员函数)

**语法：** 在成员函数声明和定义末尾加上 const 关键字。
`ReturnType memberFunction() const;`
**目的：** 承诺该成员函数不会修改对象的任何**非** `mutable` **数据成员**。

**优势：**
- `const` **对象调用：** 只有 const 成员函数才能被 const 对象调用。这使得你的类接口更加健壮。
- **安全性：** 保证了对象的状态不会被意外改变。
- **重载：** const 和非 const 成员函数可以重载，允许根据对象的 const 属性调用不同的版本。

`mutable` **关键字：** 
可以修饰类的非静态数据成员。被 `mutable` 修饰的成员即使在 `const` 成员函数中也可以被修改。这通常用于那些不影响对象逻辑状态，但需要内部缓存或统计的成员。

```C++
class MyClass {
    int value;
    mutable int accessCount; // 即使在 const 成员函数中也可以修改
public:
    void incrementCount() const { // const 成员函数
        accessCount++; // OK：accessCount 是 mutable
        // value++; // 错误：value 不是 mutable
    }
};
  ```
  

# 3 `const` 的好处

1. **数据完整性 ：** 防止程序意外地修改不应该改变的数据，减少了编程错误。
2. **代码安全性：** 编译器会强制执行 const 约束，在编译阶段就能发现潜在的错误。
3. **可读性与意图清晰 ：** const 明确地向代码读者表明哪些数据是只读的，哪些函数不会改变对象状态，提高了代码的可理解性。
4. **编译器优化：** 编译器知道 const 数据不会改变，可以进行更积极的优化，例如将常量存储在只读内存中。
5. **更好的接口设计：** 允许函数接受 const 引用/指针参数，使得函数可以处理 const 对象，提高了函数的通用性和复用性。
