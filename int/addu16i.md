# addu16i.d

> 16位立即数双字加法([add] [u]pper [16]-bit [i]mmediate [d]ouble word), 格式: DJSk16
> 操作码： `0b0001_00_sk16_rj_rd`/`0x10000000`, 掩码: `0xfc000000`
> 更多信息： <https://loongson.github.io/LoongArch-Documentation/>

- 将 16-bit 立即数 si16 逻辑左移 16 位后符号扩展，再加上寄存器 rj 中的数据，结果写入寄存器 rd 中。

`addu16i.d rd, rj, si16`

- 实例

`addu16i.d $t0, $t0, 2`
