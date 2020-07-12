## 学习笔记

<a name="ycYeT"></a>
### 编程语言基础知识

<br />语言按照语法分类：<br />

- 非形式语言：中、英文等，没有严格的语法定义
- 形式语言：计算机语言，有严格的语法定义
   - 分类方法（乔姆斯基谱系）
      - 0型 无限制文法
      - 1型 上下文相关文法
      - 2型 上下文无关语法
      - 3型 正则文法


<br />乔姆斯基谱系几个分类方法，是上下包含关系，0 型包含 1、2、3 型，1 型包含 2、3 型，反过来就不行了。

<a name="WXJIk"></a>
### 产生式

<br />描述方法（最经典，BNF）：<br />

- 语法结构名：<> 括号里面的内容
- 语法结构
   - 基础结构，称终结符
   - 复合结构，称非终结符
- 引号和中间的字符表示终结符
- 可有括号 ()
- 量词
   - *
   - +
- 逻辑 |


<br />举例：<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594562493283-d0ece463-bde9-4259-922d-d4f8d0b35f56.png#align=left&display=inline&height=344&margin=%5Bobject%20Object%5D&name=image.png&originHeight=344&originWidth=915&size=223063&status=done&style=none&width=915)<br />

<a name="vrlIx"></a>
### 理解乔姆斯基谱系（通过产生式）

<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594563037154-450fc798-0ceb-4ad3-ba38-98dd53a26688.png#align=left&display=inline&height=326&margin=%5Bobject%20Object%5D&name=image.png&originHeight=326&originWidth=658&size=121820&status=done&style=none&width=658)<br />
<br />JS 总体上属于上下文无关文法，表达式大部分属于正则文法。<br />
<br />**JS 标准中的产生式书写方法：**<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594563262632-e3327ff1-a2b7-45d0-9d09-eea879db3412.png#align=left&display=inline&height=164&margin=%5Bobject%20Object%5D&name=image.png&originHeight=329&originWidth=645&size=135774&status=done&style=none&width=322.5)<br />

<a name="QIvoE"></a>
### 现代语言的分类

<br />先将形式化语言里非形式化部分（特例）：<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594563403661-09f0b4ff-62cb-432a-8617-f6c69da6ed1c.png#align=left&display=inline&height=323&margin=%5Bobject%20Object%5D&name=image.png&originHeight=323&originWidth=831&size=372689&status=done&style=none&width=831)<br />
<br />形式语言分类

- 用途
   - 数据描述语言
      - ![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594563616755-f9a8d1c8-7d17-441c-ae33-490697d8035c.png#align=left&display=inline&height=38&margin=%5Bobject%20Object%5D&name=image.png&originHeight=75&originWidth=430&size=21816&status=done&style=none&width=215)
   - 编程语言
      - ![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594563625309-c88b361d-4787-422a-95f4-a36102190a17.png#align=left&display=inline&height=65&margin=%5Bobject%20Object%5D&name=image.png&originHeight=130&originWidth=410&size=49384&status=done&style=none&width=205)
- 表达方式
   - 声明式语言
      - ![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594563657437-2620441e-d363-44a8-88c6-4c0ccf8610dd.png#align=left&display=inline&height=37&margin=%5Bobject%20Object%5D&name=image.png&originHeight=74&originWidth=421&size=33289&status=done&style=none&width=210.5)
   - 命令性语言
      - ![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594563684697-83342057-d50f-40ae-b98e-90f66bcb5a4b.png#align=left&display=inline&height=54&margin=%5Bobject%20Object%5D&name=image.png&originHeight=107&originWidth=413&size=31793&status=done&style=none&width=206.5)



<a name="vBUNB"></a>
### 编程语言的性质


- 图灵完备性
   - 命令式 —— 图灵机
      - goto
      - if/while
   - 声明式 —— lambda
      - 递归



- 动态与静态
   - 动态
      - 该语言是在用户设备/线上服务器上运行的，
      - 是在产品实际使用时执行的
      - 对应一个概念 Runtime
   - 静态
      - 该语言是在程序员的设备上运行的（静态类型检查），
      - 发生在产品开发时
      - 对应一个概念 Cmopiletime

<br />

- 类型系统
   - 动态与静态
      - 动态：在用户的机器里能够找到的类型
      - 静态：只在程序员编写代码的时候，能够保留类型信息
   - 强类型与弱类型（类型转换）
      - 强类型：默认不会发生类型转换
      - 弱类型：默认会发生类型转换
   - ![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594564526749-8439c7d6-6426-48ba-9b13-4aafed43f9af.png#align=left&display=inline&height=147&margin=%5Bobject%20Object%5D&name=image.png&originHeight=196&originWidth=316&size=48244&status=done&style=none&width=237)


<br />
<br />
<br />

<a name="8qKWU"></a>
### Atom：组成 JavaScript 语言的最小元素

<br />语法 Grammer<br />

- Literal 字面值
- Variable
- Keywords
- Whitespace
- Line Terminaltor


<br />运行时 Runtime<br />

- Types
- Execution Context



<a name="xV9JK"></a>
### 类型


- Number
- String
- Boolean
- Object
- Null
- Undefined
- Symbol：用于 Object 属性名。最常用的前面 5 个


<br />typeof null 结果是 object 是 bug，已经不准备修复了。<br />

<a name="8xNyE"></a>
### Number


- 实现：IEEE 754 Double Float
   - Sign(1)
   - Exponent(11)
   - Fraction(52)
- 语法
   - DecimalLiteral
      - 0
      - 0.
      - .2
      - 1e3
   - BinaryIntegerLiteral
      - 0b111
   - OctalIntegerLiteral
      - 0o10
   - HexIntegerLiteral
      - 0xFF


<br />小案例：<br />

```javascript
0.toString() // error, . 被当成小数点了
0 .toString() // "0"
```


<a name="GGSaT"></a>
### String

<br />核心概念<br />

- Character：一个字符用一个码点（Code Point）表示
- Code Point
- Encoding


<br />各种字符集<br />

- ASCII：拉丁字母，一共 127 个字符
- Unicode：万国码
   - 0x0000~0xffff，两个字节
- UCS
- GB
   - GB2312
   - GBK（GB13000）
   - GB18030
- ISO-8859（欧洲）
- BIG5（台湾，大五码）


<br />编码方式<br />

- UTF


<br />Unicode 中的 ASCII 范围内字符使用 UTF8 编码，用一个字节（8位）表示一个字符。 UTF8 编码用两个字节表示一个字符。<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594550432578-425ed301-9a08-4b9b-8427-fb992a0b6dae.png#align=left&display=inline&height=213&margin=%5Bobject%20Object%5D&name=image.png&originHeight=213&originWidth=825&size=91499&status=done&style=none&width=825)<br />
<br />语法：<br />

- 双引号："abc"
- 单引号：'abc'
- 模板函数：`abc`


<br />问题： ![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594550918194-03d703c6-5689-47b5-89fe-f7f3f6e648ae.png#align=left&display=inline&height=72&margin=%5Bobject%20Object%5D&name=image.png&originHeight=72&originWidth=622&size=41256&status=done&style=none&width=622)<br />
<br />答案（根据ES5）：![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594550946080-d4fe43dd-f94a-40a0-a82a-bc2380b7f64d.png#align=left&display=inline&height=127&margin=%5Bobject%20Object%5D&name=image.png&originHeight=127&originWidth=818&size=126343&status=done&style=none&width=818)<br />
<br />模板字符串<br />
<br />`ab${x}abc${y}abc`<br />
<br />JS 引擎视角（括号里的是 JS 语法，括号之外是字符串本体）<br />

- `ab${
- }abc${
- }abc`



<a name="Ap6p5"></a>
### 对象（基础知识）

<br />使用类的方式来描述对象<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594551557076-7a603f5a-147c-480f-95d4-22f05a4b03d0.png#align=left&display=inline&height=348&margin=%5Bobject%20Object%5D&name=image.png&originHeight=348&originWidth=896&size=154962&status=done&style=none&width=896)<br />
<br />使用类的方式来描述对象<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594551843302-841460c8-8fc2-495b-b9c6-4e191d976091.png#align=left&display=inline&height=394&margin=%5Bobject%20Object%5D&name=image.png&originHeight=394&originWidth=875&size=229243&status=done&style=none&width=875)<br />
<br />

> 在设计对象的行为时，要遵循“行为改变状态”的原则。


<br />**对象的描述：**<br />
<br />原生对象的描述非常简单，只需要关心原型和属性两个部分即可。<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594552634535-f2e38a11-2d45-4e1b-a929-9832dfc422be.png#align=left&display=inline&height=325&margin=%5Bobject%20Object%5D&name=image.png&originHeight=325&originWidth=387&size=36242&status=done&style=none&width=387)<br />
<br />**对象属性：**<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594552710293-91f270a1-3ab5-4513-a045-9ce458b21cc9.png#align=left&display=inline&height=183&margin=%5Bobject%20Object%5D&name=image.png&originHeight=183&originWidth=527&size=24892&status=done&style=none&width=527)<br />
<br />属性名可以是字符串类型，也可以是 Symbol 类型的。而属性值的情况，又可以分为数据属性和访问器属性。<br />
<br />**数据属性和访问器属性的特征分布：**

![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594552857765-420fbb8b-222d-499d-97e5-74c01080bada.png#align=left&display=inline&height=331&margin=%5Bobject%20Object%5D&name=image.png&originHeight=331&originWidth=861&size=195008&status=done&style=none&width=861)<br />
<br />**原型链**<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594552948931-175d36df-7c3a-48ec-b722-9badc2c3d1f5.png#align=left&display=inline&height=352&margin=%5Bobject%20Object%5D&name=image.png&originHeight=352&originWidth=602&size=129753&status=done&style=none&width=602)<br />
<br />分四类：<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594553040544-c92f5502-d77b-4b27-a002-cc17e4287177.png#align=left&display=inline&height=202&margin=%5Bobject%20Object%5D&name=image.png&originHeight=202&originWidth=625&size=116086&status=done&style=none&width=625)<br />

1. 基本的面向对象能力。创建对象、访问和设置对象属性，定义属性特征值。
1. 操作原型的能力，基于原型的API
1. 基于分类的方式来描述对象，虽然底层基于原型，但是从语法上，是基于类的面向对象的方式
1. 历史包袱，不伦不类，不建议使用



<a name="HD0ho"></a>
### 特殊对象

<br />函数对象：带有内部属性 [[call]]的对象。<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594553249942-d3247f70-3dbb-4e83-ae92-78df79780b4b.png#align=left&display=inline&height=324&margin=%5Bobject%20Object%5D&name=image.png&originHeight=324&originWidth=842&size=241445&status=done&style=none&width=842)<br />
<br />数组的 length 属性，Object.prototype 不能在设置原型对象了……<br />
<br />![image.png](https://cdn.nlark.com/yuque/0/2020/png/103346/1594553282386-605aab23-2039-42c2-88fb-9dfbbe95b0bd.png#align=left&display=inline&height=135&margin=%5Bobject%20Object%5D&name=image.png&originHeight=135&originWidth=647&size=39728&status=done&style=none&width=647)<br />
<br />
<br />

