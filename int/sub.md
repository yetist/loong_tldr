# sub.<w|d>

> 减法, 格式：DJK，掩码：`0xffff8000`
> sub.w 操作码: `0b0000_0000_0001_0001_0_rk_rj_rd`/`0x00110000`
> sub.d 操作码: `0b0000_0000_0001_0001_1_rk_rj_rd`/`0x00118000`
> 更多信息： <https://loongson.github.io/LoongArch-Documentation/>

- 减字([sub]stract [w]ord), 寄存器 rj 的低32位减去寄存器 rk 的低32位数据，结果的低32位符号扩展后写入寄存器 rd 中。

`sub.w rd, rj, rk`

- 减双字([sub]stract [d]oubleword), 将寄存器 rj 中的数据减去寄存器 rk 中的数据,结果写入寄存器 rd 中。

`sub.d rd, rj, rk`

- 实例:

`add.w $t2, $t1, $t0`
`add.d $t2, $t1, $t0`
