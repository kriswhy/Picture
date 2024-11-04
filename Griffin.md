> **性质1（数论基本定理）**：若整数a与n互素，即$gcd(a,n)\equiv 1$，则a在模n下存在乘法逆元b，即$a\cdot b = 1$ mod $n$。扩展欧几里得算法可以证明并且求出b的值。

> **性质2**：$F_p$ 的所有非零元素在乘法下构成一个乘法群，这个群是循环群，阶为 $p-1$。这里的「阶」表示群中元素的个数。这个循环群中至少存在一个生成元$g$，可以生成群中的所有**非零**元素: $g^k$，其中$0\leq k\leq p-2$。

> **定理**：对于$F_p$，p为素数，当$gcd(d,p-1)=1$时，$f(x)=x^d$ mod $p$ 的取值可以覆盖$F_p$中所有非零元素。

证明：因为$F_p$ 的乘法群（即所有非零元素的集合）是一个循环群，其阶为 $p−1$。所以存在生成元$g$，可以生成群中的所有**非零**元素: $g^k$，其中$0\leq k\leq p-2$。

下面证明$f(x)$是一个置换。$f(x)=f(g^k)=g^{kd}$ mod $p$。也就是映射将$k\rightarrow kd$， 其中$k$是模$p-1$的整数。

所以接下来证明$k\rightarrow kd$ 是一个双射，即 $kd$ mod $(p-1)$ 覆盖0,1,2,..,p-2。

因为$gcd(d,p-1)=1$ 和性质1，存在$d^{-1}$。对于任意$m\in \{0,1,...,p-2\}$, 都存在唯一一个$k$ 使得$kd\equiv m$ mod $(p-1)$. 

所以$k\rightarrow kd$ 是一个双射，即$f(x)$是一个置换。





### Type-I/-II/-III Feistel schemes (https://eprint.iacr.org/2010/301.pdf)

![1729003509558](C:\Users\haoyang\Documents\WeChat Files\why459834346\FileStorage\Temp\1729003509558.png)