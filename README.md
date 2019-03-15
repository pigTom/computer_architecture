## 学习计算机体系结构

> 计算机指令有三种形式:  
> - 操作指令加上三个寄存器，比如add、sub等  
R type instruction

| op | rs | rt | rd | shamt | funct |  
| - | - |
| 6bits | 5bits | 5bits | 5bits | 5bits | 6 bits |

all R type of opcode is 0 and shamt is only used for shift operation
> - 操作指令加上两个寄存器再加上一个立即数，比如addi，lw等
I type instruction

| op | rs | rt | imm |   
| - | - | - | - |
| 6bits | 5bits | 5bits | 16bits |

> - 操作指令加上一个26位的立即数
