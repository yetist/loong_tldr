# addi.<w|d>

> 立即数加法，忽略算术溢出。格式:DJSk12, 掩码: `0xffc00000`
> addi.w 操作码: `0b0000_0010_10_si12_rj_rd`/`0x02800000`
> addi.d 操作码: `0b0000_0010_11_si12_rj_rd`/`0x02c00000`
> 更多信息： <https://loongson.github.io/LoongArch-Documentation/>

- 立即数加字([add] [i]mmediate [w]ord)，将寄存器 rj 的低32位加上 12-bit 立即数 si12，结果的低32位符号扩展后写入寄存器 rd 中。

`addi.w rd, rj, si12`

- 立即数加双字([add] [i]mmediate [d]ouble word)， 将寄存器 rj 的加上 12-bit  立即数 si12，结果符号扩展后写入寄存器 rd 中。

`addi.d rd, rj, si12`

- 实例

`addi.w $t2, $t1, 4095`
`addi.d $t2, $t1, 4095`
