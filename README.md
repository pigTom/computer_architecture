## 学习计算机体系结构

> 计算机指令有三种形式:  
> - 操作指令加上三个寄存器，比如add、sub等  
R type instruction

| op | rs | rt | rd | shamt | funct |  
| - | -| - | - | - |  - |
| 6 bits | 5 bits | 5 bits | 5 bits | 5 bits | 6 bits |

all R type of opcode is 0 and shamt is only used for shift operation
> - 操作指令加上两个寄存器再加上一个立即数，比如addi，lw等
I type instruction

| op | rs | rt | imm |   
| - | - | - | - |
| 6 bits | 5 bits | 5 bits | 16 bits |

> - 操作指令加上一个26位的立即数
J type instruction

| op | addr |
| - | - |
| 6 bits | 26 bits|

### Intel 80386寄存器
80386的寄存器可以分为8组（它们的宽度都是32位）：  
- 通用寄存器
> - EAX : 累加器
> - EBX : 基址寄存器
> - ECX : 计数器
> - EDX : 数据寄存器
> - ESI : 源地址指针寄存器
> - EDI : 目的地址指针寄存器
> - EBP : 基址指针寄存器
> - ESP : 栈地址指针寄存器

- 段寄存器
> 段寄存器也称段选择字，段选择符。除了8086的4个段外（CS,DS,ES,SS),
> 80386还增加了两个段FS，GS，这些段寄存器都是16位的，用于不同属性内存段的寻址，它们的含义如下：
> CS: 代码段(Code Segment)
> DS: 数据段(Data Segment)
> ES: 附加数据段(Extra Segment)
> SS: 堆栈段(Stack Segment)
> FS: 附加段
> GS: 附加段
- 指令指针寄存器
- 标志寄存器
- 系统地址寄存器
- 控制寄存器
- 调试寄存器
- 测试寄存器

### 中断、异常和系统调用
- 系统调用（system call)
> 应用程序主动向操作系统发出的服务请求

- 异常（exception）
> 非法指令或者其他原因导致当前指令执行失败（如：内存出错后的处理请求）

- 中断（hardware interrupt)
> 来自硬件设备的处理请求

------ 今天没有学习OS，不知道以后还能不能坚持下来。时间不够，而且也学不懂，
有人说你学这个东西有什么用吗，以后又不到。我想说我只是爱好它而已，
只是自己爱好而已，有没有用没有关系。-----
------ at shenzhen 2019-03-19 星期二 晴

