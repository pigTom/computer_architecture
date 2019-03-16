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
- 指令指针寄存器
- 标志寄存器
- 系统地址寄存器
- 控制寄存器
- 调试寄存器
- 测试寄存器
