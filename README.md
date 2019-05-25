# 2016 级大三必修课的考题整理（不完全）

本 repo 未来会有更新，欢迎 watch。

## 目录

[通信软件设计](#通信软件设计)

[计算机网络](#计算机网络)

[软件过程改进](#软件过程改进)

[面向对象分析与设计【期中】](#面向对象分析与设计期中)

[面向对象分析与设计【期末】](#面向对象分析与设计期末)

[软件项目管理（SPM）【期中】](#软件项目管理spm期中)

[软件项目管理（SPM）【期末】](#软件项目管理spm期末)

[软件质量保证与测试/软件测试【期中】](#软件质量保证与测试软件测试期中)

[【待完成】软件质量保证与测试/软件测试【期末】](#软件质量保证与测试软件测试期末待完成)

## 通信软件设计

所有题目都没有要求写文字的语法（比如 signal，timer）这样的，但还是建议背一下，因为最后一道大题要用

#### 填空（1 题 3 分）

- 要求画出一些 sdl 和 msc 的图示
  - 如：建立进程实例的符号是什么？
- sdl 语言中系统之外的部分被称为？
- sdl simulator 生成出来的代码是什么编程语言的？
- 电话交换机中，当用户摘机之后，应当给用户播放`________`音？

#### 选择题：(1 题 3 分，很多题目只有 3 个选择)
- 给了一些 msc 图，询问了很简单的问题
- 给出三张 SDL 图，问哪张是错误的
  - 涉及到课本 P120 5.4.11 图形符号连接关系
  - 有的符号不能连在别的符号底下

#### 判断题（1 题 3 分）

- SDL 的进程、MSC 的消息、SDL 的信号，哪些能带参数，哪些不能？
  - 看书即可得到答案
- 还有一些别的基础知识

#### 简答题（10 分）

协议分析的过程中需要做哪些工作？

#### MSC 绘制（15 分）

火车站里有一台取票机，该取票机有打印机、键盘、触控屏等输入设备，视作外部设备。该取票机与中央取票系统（称为“后台”）相连，从后台获取用户火车票相关的信息。该取票机的使用流程如下：

1. 用户刷身份证，取票机向后台申请认证该用户；
2. 后台向用户发送取票短信，上面有该用户的取票密码；
3. 取票机向后台发送用户输入的密码；
4. 验证成功后，后台给取票机发送用户所购买的火车票信息；
5. 用户在取票机上选择想要打印的火车票；
6. 取票机向打印机发送打印指令，打印所选火车票。

在火车票最终被打印之前，用户都可以随时退出该系统。在退出该系统之后，用户必须重新刷身份证才能重新使用。用户操作有时间限制，若超时，视为用户退出该系统。

请为下列情况绘制 MSC 图：

1. 用户成功取到火车票
2. 用户超时未输入取票密码
3. 用户在打印火车票前中途退出系统

#### SDL 绘制（15 分）

画出取票机控制软件的进程状态机图。

## 计算机网络

因为很多题目回忆不起来了，甚至连题型都记不起来了，所以请参考 14 级的题目。

这里重点讲一些比较难的知识点：

- 时分复用、频分复用和码分复用是什么意思？
- 信号调制的几种方法分别是什么？
  - 但是没考星座图
- CRC 码是一种 `___` 码。
  - 让我很震惊的是，没有考计算 CRC
- 给你两个字节，问你汉明距离是多少
  - 令我极度震惊的是，没有考计算汉明码
- 在什么协议下会出现隐爆终端问题？
  - 中文课本 P215，英文课本 4.2.5 节
- 虚电路与包转发相关
  - 虚电路需要沿路建立连接吗？
  - TCP 协议建立连接后，每一个包都会在网络上走同一条路线吗？
- 和电子邮件相关的一些协议有哪些？分别是干嘛的？
- 填空题考了一道作业题：ip 地址聚合
- tcp 的 fin flag 有什么用？
- 什么网络使用交换机这一设备？
- 经典以太网用的是什么样的介质访问控制（MAC）协议？
- 用于域内/域外路由的有哪些协议？
- TCP 里**每一个字节**都有一个序号吗？
- TCP 用什么机制进行错误处理？
- Wi-Fi 基于无线电，容易受到干扰而出错，那么里面有没有使用**纠**错码呢？
  - 注意不是**检**错码
- 大题：为什么实时音视频业务需要使用 UDP 协议？请给出两个基于 UDP 的协议。
- 大题：为什么用于域内路由的协议不能用于域外路由？
- 大题：链路状态路由的原理是什么？

## 软件过程改进

题目太多忘了。请背 PPT，推荐背~~黄色资源~~标有黄字的 PPT。这次考的内容非常细致，甚至考了你开例会的时候要做什么这种题。总而言之 PPT 全部背下来是没错的。

## 面向对象分析与设计【期中】

期中题目全都是师兄们带带相传的大题，请参考往届学长资料。

## 面向对象分析与设计【期末】

本届试题为全英文试题，且没有客观题。

1. 4 分简答题
   1. DCD <u>stands for（的全称是）</u> 什么？
      1. ~~高慧（监考中）：「DCD 就是设计类图的意思啊！」~~
      2. ~~根据过往试题，每年都会考某个缩写的含义/全称。鉴于考场上知道 DCD 全称的人太少，来年不会再考 DCD 的全称。~~
   2. pattern（模式）是什么？
   3. 我们写 operation contract（操作契约）的 purpose（目的）是什么？
   4. 请结合实际，用一个例子来说明关联类（association class）是什么
   5. ……以及别的带带相传的大题。
      1. RUP 是不会考的，放心。
      2. ~~知乎，2014：[RUP 早就被业界抛弃了](https://www.zhihu.com/question/23208040/answer/23949523)~~
2. 20 分大题
   1. GRASP 的最常用的三个模式是什么？举例说明在哪些场景下能够使用
   2. GoF 中有三个模式常常在一起使用，请问这三个模式是什么，并说明它们面对的问题和解决的答案
   3. 给出形如下面代码的通信图（考试时给出的是通信图，为了不插入图片，在此用代码代替），其中系统操作（第 0 个方法调用）是构造了一个`Controller`对象（对应代码中的 main 方法）。画出对应的 UML 顺序图：

```java
// 你接下来看到的不是代码而是 UML 通信图
// 请脑补这张通信图的样子...

class Register {
    public Register(ProductCatalog catalog) {
        // do something...
    }
}

class Controller {
    public Controller() {
        var catalog = new ProductCatalog();
        var register = new Register(catalog);
    }
}

class ProductCatalog {
    private Map<int, Product> products;

    public ProductCatalog() {
        products = new Map<int, Product>();
        this.createSpec();
    }

    public void createSpec() {
        while (true) {
            // 你不需要管 id, price, name 是从哪来的
            var prod = new Product(id, price, name);
            products.put(id, prod);
        }
    }
}

class Product {
    public Product(int productId, int price, String name) {
        // 省略...
    }
}

// ......

public static void main(String[] args) {
    var controller = new Controller();
}

```

## 软件项目管理（SPM）【期中】

期中考试是敲警钟的考试，所以老师们出了很难的题目。本次期中考试要求深入理解掌握挣值分析、SPSP 模型和历时分析的关键路径法和资源优化法；题目将这些知识点融入到了两道综合题之中。（具体题目忘了）

所谓的「深入掌握」，就是说光看 PPT 记住了上面的内容也不行，需要熟练掌握做题方法，请多多留意。

## 软件项目管理（SPM）【期末】

SPM 慕课上的题目非常重要，毕竟老师为了控制难度，会多出慕课上面的原题给大家放水。如果不背慕课原题就吃大亏了。

本届试题为中文试题。

#### 填空题（15 分，1 分/小题）

此处填空题也出现了不少慕课原题。这里只描述需要背的内容：

- WBS 的全称
- 马斯洛需求层次中最高层次的需求是什么
- 需求规格审计属于什么类型的活动？
- Scrum 模型的四个管理会议是什么

#### 选择题（20 分，1 分/小题）、判断题（15 分，1 分/小题）

都是慕课原题，背就是了

#### 大题 1：PERT（10 分）

考察用 PERT 进行项目历时估算。题目给出了如下任务图：

```
    +-----+     +-------+     +-------+     +-------+
    |     |     |       |     |       |     |       |
    | 开始 +--- >+ 任务1 +---->+ 任务2  +---->+ 结束  |
    |     |     |       |     |       |     |       |
    +-----+     +-------+     +-------+     +-------+

```

并给出各任务的耗时：*（数据乱编，仅供参考）*

|        | 乐观耗时 | 一般耗时 | 悲观耗时 |
| ------ | -------- | -------- | -------- |
| 任务 1 | 4        | 8        | 18       |
| 任务 2 | 3        | 5        | 13       |

问：

1. 这是 PDM 还是 ADM？
2. 根据 PERT 方法给出任务 1、2 完成的时间期望。
3. 项目在 23 天内完成的概率是？
   1. 最气的是，题目并没有给出 +σ、+2σ、+3σ 对应的概率取值，明明连高考都给出来了。请把 68.27%、95.45% 和 99.73% 这三个数字背下来。

#### 大题 2：历时估算——关键路径法（15 分）

题目给出一张 PDM 网络图，涉及到了 A、B、C……G 共 7 个任务。

（题目给出的图与 https://zhuanlan.zhihu.com/p/60518717 中的图类似）

问：

1. 画出关系依赖矩阵
   1. 如果 i 到 j 有一条有向边，那么 P<sub>ij</sub>=1
2. 将最早开始时间、最晚开始时间等填入图中
3. 找出关键路径
4. 项目的总耗时是多少？
5. 任务 F 的**总**浮动是多少？
   1. 注意区分总浮动和**自由**浮动
6. **将题目给出的 PDM 图画成 ADM 图**
7. 任务 G 【注：是最后一个任务】的最晚开始时间（LS）的计算依据是什么？

#### 大题 3：挣值分析（10 分）

题目给出了一个项目预算 - 成本 - 完成度表，并要求基于这个表格进行挣值分析：

*（以下数据是瞎编的，仅用于说明题目）*

**表 1**、预算表

| 周     | 1    | 2    | 3    | 4    | 5    | 6    | 7    | 8    |
| :----: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| 任务 1 | 10   | 15   | 5    |      |      |      |      |      |
| 任务 2 |      |      | 10   | 15   | 5    | 10   | 15   | 5    |
| 任务 3 |      |      |      |      |      |      | 5    | 5    |

**表 2**、实际成本表

|   周   |  1   |  2   |  3   |  4   |  5   |  6   |  7   |  8   |
| :----: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| 任务 1 |  10  |  18  |  8   |      |      |      |      |      |
| 任务 2 |      |      |  12  |  15  |  8   |  12  |  17  |  10  |
| 任务 3 |      |      |      |      |      |      |  6   |  5   |

**表 3**、实际完成度表

| 周     | 1    | 2    | 3    | 4    | 5    | 6    | 7    | 8    |
| :----: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| 任务 1 | 5%   | 15%  | 100% |      |      |      |      |      |
| 任务 2 |      |      | 10%  | 15%  | 20%  | 35%  | 45%  | 55%  |
| 任务 3 |      |      |      |      |      |      | 5%   | 10%  |

问：

1. 根据挣值分析的知识回答：
   1. 第 6 周周末的 BCWS、BCWP、ACWP 分别为？
   2. 第 6 周周末的 SPI 和 CPI 分别是多少？并说明这两个指标的现实意义。
   3. 项目最终将花费多少成本？
2. 请画出该项目到第 6 周周末的燃尽图。

#### 大题 4：决策树（5 分）

课本例题。某企业在下年度有甲、乙两种产品方案可供选择。每种方案都面临滞销、一般、和畅销三种市场状态。各状态的概率和损益值如下：

| 任务 \ 市场状态 | 滞销（P=0.2） | 一般（P=0.3） | 畅销（P=0.5） |
| :-------------: | :-----------: | :-----------: | :-----------: |
|       甲        |      20       |      70       |      100      |
|       乙        |      10       |      50       |      160      |

使用决策树法求出甲、乙的 EMV 来选择其中一套方案。

#### 大题 5：敏捷项目实验（5 分）

给出你们组 SPM 项目的一个 Epic，以及它分解得出的 Story，然后用标准格式写出一个 Story。

~~（如果 SPM 项目抄了学长代码的话就现场编吧）~~



## 软件质量保证与测试/软件测试【期中】

这次的期中测试是**开卷考**，不仅所有人可以携带纸质资料考试，而且本届的 1~3 班还能**携带手机考试**。老师认为「如果不符合规定的话，就把它当作一个**大作业**也行。」

本次的试题为全中文。

#### 判断题（写出正误，2 分/题，共 20 分）

此处记录几道有代表性的题目：

1. 软件缺陷产生主要归咎于软件设计。
2. 在 McCabe 圈复杂度计算中，代码的圈复杂度 V(G) = N - E + 2。（N 为节点的数量，E 为边的数量）
3. 在自底向上的集合测试中，有时候需要编写桩模块。
4. 在三明治测试方法中，中间层使用的是大爆炸集成的方式。
5. 软件的易用性，指的是软件产品或系统具有易于操作和控制的属性的程度。
6. Beta 测试是用户在开发环境上的测试，也可以是开发机构内部用户在模拟实际操作环境下进行的测试。

#### 填空题（2 分/题，共 20 分）

此处记录几道有代表性的题目：

1. `________`是交付后测量缺陷程度的标准，是开发团队内部识别与纠正的缺陷在整个开发周期中占全部缺陷的比例。
2. 软件之间是否正确交互与共享信息是`________`测试的目标。

#### 简答题（10 分/题，共 20 分）

1. 举例说明软件缺陷判别规则
2. 举例说明用正交表设计测试用例的步骤

#### 大题（共 40 分）

此处开始是一题一页的大题，每小题分值未知。

#### 大题 1：边界值分析法

现有一个程序，程序要求输入三角形的三条边长度 A、B 和 C（取值范围为 1 <= A <= 100，1 <= B <= 100，1 <= C <= 100），如果 A、B、C 不能组成三角形，程序将输出“不能组成三角形”，否则将输出所组成的三角形的类型（等腰三角形、等边三角形、直角三角形）。请使用边界值分析法设计测试用例。

#### 大题 2：决策表

功率在 50 以上、维修记录不齐全且运行时长为 10 年以上的汽车，应优先进行维修。请写出该程序的**判定表**。

#### 大题 3：路径测试

给出如下的程序流程图，输入为 X 和 Y，请设计测试用例，要求分别达到语句覆盖、判定覆盖、条件覆盖、判定/条件覆盖、条件组合覆盖、物理路径覆盖。对于每个测试用例，请写出 X 和 Y 的取值，以及在流程图中经过的路径（流程图的边的小字为该路径的名字，用该名字来表示路径）。

流程图如下：

```c
// 以下你看到的是一张形如 http://t.cn/E9DynQu 的流程图
// 其中，用 if 语句代替了判断节点，用带小写字母的注释代替了边的文字
// 例：X = 9，Y = 6 时，经过的路径为 a、c、h、i。

void program(int X, int Y) {
    // a
    if (X > 8 && Y > 5) {
        // c
        if (X > 16 || Y > 10) {
            // f
            function_3();
        }
        // h
    } else {
        // b
        if (X > 0 || Y > 0) {
            // e
            function_2();
        } else {
            // d
            function_1();
        }
        // g
    }
    // i
}
```





## 软件质量保证与测试/软件测试【期末】（待完成）