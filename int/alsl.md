# alsl.<w[u]|d>

> 算术逻辑左移
> alsl.w 操作码: 0b0000_0000_0000_010_sa2_rk_rj_rd/0x00040000, 掩码:0xfffe0000
> alsl.wu 操作码: 0b0000_0000_0000_011_sa2_rk_rj_rd/0x00060000, 掩码:0xfffe0000
> alsl.d 操作码: 0b0000_0000_0010_110_sa2_rk_rj_rd/0x002c0000, 掩码:0xffde0000

- 算术逻辑左移字([a]rithmetic [l]ogical [s]hift [l]eft [w]ord)，将寄存器 rj 的低32位数据逻辑左移(sa2+1)位后加上寄存器 rk 的低32位数据, 结果的低32位符号扩展写入寄存器 rd 中。

`alsl.w rd, rj, rk, sa2`

- 无符号算术逻辑左移字([a]rithmetic [l]ogical [s]hift [l]eft [w]ord [u]nsigned)， 将寄存器 rj 的低32位数据逻辑左移(sa2+1)位后加上寄存器 rk 的低32位数据, 结果的低32位零扩展写入寄存器 rd 中。

`alsl.wu rd, rj, rk, sa2`

- 算术逻辑左移双字([a]rithmetic [l]ogical [s]hift [l]eft [d]oubleword)，将寄存器 rj 的数据逻辑左移(sa2+1)位后加上寄存器 rk 的数据, 结果写入寄存器 rd 中。

`alsl.d rd, rj, rk, sa2`

- 实例

`alsl.w $t4, $t4, $t5, 0x1`
`alsl.d $t0, $t0, $s4, 0x3`
