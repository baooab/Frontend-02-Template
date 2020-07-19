## 表达式的优先级

按照优先级从高到低，分别是：Member > new > Call Expression > Update > Unary > Exponental > 乘法和加法 > 移位 > 关系 > 相等比较 > 位运算 > 逻辑 > 条件。

下面依次解释：

### Member

- a.b
- a[b]
- foo\`string\`
- super.b
- super['b']
- new.target
- new Foo()

### new

new Foo

### Call Expression

- foo()
- super()
- foo()['b']
- foo().b (点运算符被 Call Expression 拉低了优先级)
- foo()\`abc\`

### Update

- a++
- a--
- --a
- ++a

### Unary

- delete a.b
- void foo()
- typeof a
- +a
- -a
- ~a
- !a
- await a

### Exponental

\*\*：JS 唯一右结合的运算符

### 乘法和加法

- Multiplicative: *、/、%
- Additive: +、-

### 移位

\>\>、<<、\>\>\>

### 关系

\>、<、\>=、<=、instanceof、in

### 相等比较

==、!=、====、!==

### 位运算

&、^、|

### 逻辑

&&、||

### 条件

? :

（完）
