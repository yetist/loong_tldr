# lu12i.w

> 加载高12位立即数
> 操作码: `0b0001_010_si20_rd/0x14000000`, 掩码：`0xfe000000`
> 加载高12位立即数字([l]oad [u]pper [12]-bit [i]mmediate [w]ord)

- 将 20-bit 立即数 si20 最低位连接上 12 比特 0，符号扩展后写入寄存器 rd 中。

`lu12i.w rd, si20`

- 实例:

`lu12i.w rd, si20`
