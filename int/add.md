# add.<w|d>

> 加法, 格式:DJK，掩码: `0xffff8000`
> add.w 操作码: `0b0000_0000_0001_0000_0_rk_rj_rd`/`0x00100000`
> add.d 操作码: `0b0000_0000_0001_0000_1_rk_rj_rd`/`0x00108000`
> 更多信息： <https://loongson.github.io/LoongArch-Documentation/>

- 加字([add] [w]ord)，把寄存器 rk 的低32位加到寄存器 rj 的低32位，结果的低32位符号扩展后写入寄存器 rd。 忽略算术溢出。

`add.w rd, rj, rk`

- 加双字([add] [d]ouble word)，把寄存器 rk 的数据加上 rj 中的数据，结果写入寄存器 rd 中。忽略算术溢出。

`add.d rd, rj, rk`

- 实例:

`add.w $t2, $t1, $t0`
`add.d $t2, $t1, $t0`
