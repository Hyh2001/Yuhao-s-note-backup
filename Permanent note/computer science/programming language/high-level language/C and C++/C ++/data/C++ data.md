## 整型
```C 
char < int // for length
```

### 无符号(unsigned)

### 有符号(signed)

### 内存关系

长整型 $\geq$ 整型 $\geq$ 短整型

```C
	long int > int > short int
```

## 浮点型
```C
	float < double
```

## 指针

### 运算符

#### &

```C
&x
```
取x的地址

#### *
```C
*x
```
取存在x地址中的值

### 指针对象
```C
int *a,*b;
```
#### 绝对地址赋值
需要进行类型转换
```C
x = (int*)0XB8000000;
```
### 内存分配
#### new

	int *x = new int;

##### 动态数组

	int *x = new int[10];

#### delete

	delete x;
一个delete对应一个new

##### 动态数组

	delete []x;

## 聚合类型

### 结构体

### 共用体(联合体）

允许您在相同的内存位置存储不同的数据类型。您可以定义一个带有多成员的共用体，但是任何时候只能有一个成员带有值。（只保留最后一次赋值的值）

	union
	{ member definition;
	    member definition; ...
	    member definition;
	} [one or more union variables];

#### 匿名共用体

没有名称，这个共用体的成员可以被直接使用

##### example

	struct widget
	{
    char brand[20];
    int type;
    union
    {
        long id_num;    // anonumous union
        char id_char[20];    // other widgets
    };
	widget prize;
	if (prize.type == 1)
    cin >> prize.id_num;　　// 使用变量id_num
	else
    cin >> prize.id_char;　　// 使用变量id_char

### 枚举体(enum)

	enum name { a = n,b,c,d...};  //a,b,c,d 只能为标识符

#### 变量创建

	enum name x;

#### 赋值

	x = a;

## 自动类型推断

让编译器根据对象的类型自动推断变量类型

	auto x;

## 寄存器存储

建议编译器使用CPU寄存器来存储自动变量

	register int x;
