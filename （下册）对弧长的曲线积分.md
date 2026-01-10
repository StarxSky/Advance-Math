# 对弧长的曲线积分的概念以及性质
> 定义： 定义$ L$ 为$ xOy$平面内的一条光滑的弧线，函数$ f(x, y)$在$ L$上有界。在$ L$上插入任意的一系列的点$ P_1, P_2, \dots, P_n$，将$ L$分成$ n$个小的弧线$ L_1, L_2, \dots, L_n$。设$ \Delta L_i$为第$ i$个小弧段的长度.做乘积$ f(P_i) \Delta L_i ; (i = 1, 2, ......, n)$，进行求和则有：$$ \sum_{i = 1}^{n}{f(P_{i})\Delta L_{i} }$$当弧段中长度最大者$ \lambda \to 0 $时，上式子有极限，且于分割点的方式无关，同时于所取点也无关系，则有：$$ \int_{L} f(x, y) ds = \lim_{\lambda \to 0} \sum_{i = 1}^{n}{f(P_{i}) \Delta L_{i}}$$其中， $ f(x, y) $为**被积函数**，积分限$ L$为**积分弧段**（我们总是假定函数$ f(x, y)$总是在积分弧段上连续的， 且弧长$ L$是光滑的，分段光滑）同时该定义也可以推广到积分弧度为空间时的积分弧段: $$ \int_{L}f(x, y, z) ds = \lim_{\lambda \to 0}\sum_{i = 1}^{n} {f(\delta_i, \phi_i, \tau_i)\Delta L_{i}}$$ 上式称为**对弧长$L$的曲线积分**或者**第一类曲线积分** 。 注意！如果积分弧段$ L$为**闭曲线**(端点相互连接的曲线弧段)时，那么函数$ f(x, y)$在闭曲线$ L$上对弧长的曲线积分记为:$$ \oint_{L} f(x, y) ds $$

### 一. 相关性质
* 性质1: $ \alpha , \beta $ 为常数,则: $$ \int_{L} [\alpha f(x, y) + \beta f(x, y) ]ds = \alpha \int_{L}{f(x, y) ds} + \beta \int_{L} f(x, y) ds $$

* 性质2: 若积分弧段$ L$ 可以分成两段光滑的弧段$ L_1$ 与$ L_2$，则有:$$ \int_{L} f(x, y) ds = \int_{L_1} f(x, y) ds + \int_{L_2} f(x, y) ds $$

* 性质3: 假设在曲线弧$ L$上$ f(x, y) \leq g(x, y)$则：$$ \int_{L} f(x, y) ds \leq \int_{L} g(x, y) ds$$特别的: $$ | \int_{L} {f(x, y)}  ds  | \leq \int_{L} {|f(x, y)|} ds $$ 

### 二. 对弧长曲线积分的计算方法

> 定理: $f(x, y)$在曲线弧$ L$上有定义且连续,假设$ L$由以下参数方程定义: $$ x = x(t), y = y(t), \alpha \leq t \leq \beta$$ 且，有条件: （1） 函数$ x(t)$与函数$ y(t)$在区间$ [\alpha, \beta]$上连续且具有一阶连续的导数，同时$ \sqrt{x'(t)^{2} +  y'(t)^{2}} \ne 0$则有：$$ \int_{L} f(x, y) ds = \int_{\alpha}^{\beta} f[x(t), \space y(t)] \sqrt{x'(t)^{2} +  y'(t)^{2}} dt$$ 注意：$ \alpha < \beta$


证明： 首先假定，函数所在的弧长曲线$ L$上的点当参数$ t$发生改变时：$ \alpha \to \beta$，对应的$ L$上的点从点$ A$变化到点$ B$此时在曲线弧$L $上取一系列的点:
$$
A = P_{0}, P_{1}, .... ,P_{n-1}, P_{n} = B
$$

将$ L$分割成一些曲线弧段:
$$
L_{1} =( P_1 - P_0 ), L_{2} =( P_{2} - P_{1}), .... , L_{n} = (P_{n} - P_{n-1})
$$
同时，对应的参数:
$$
\alpha = t_0 < t_1 < .... < t_{n-1} < t_n = \beta 
$$
根据对弧长的曲线积分定义有：
$$ 
\int_{L} f(x, y) ds = \lim_{\lambda \to 0}\sum_{i = 1}^{n} f(P_{i}) \Delta L_{i}
$$
在任意弧段选取点$ P_i {(x(\tau_{i}), y(\tau_{i}))}$对应于参数$ \tau_{i} \space$ 其中 $ \space t_{i-1} \leq \tau_{i} \leq t_{i} $。 根据思想“以直代曲”可知在第$ i$个曲线弧段上的切线长度为: 
$$
\Delta{L_{i}} = \int_{t_{i-1}}^{t_{i}}\sqrt{x'{(t)}^{2} +  y'{(t)}^{2}} dt
$$
应用积分中值定理$ \int_{a}^{b} f(x) dx = f(\omega)(b -a) \space ; \omega \in [a, b]$有: 
$$
\Delta{L_{i}} = \sqrt{x'{(\tau'_{i})}^{2} +  y'{(\tau'_{i})}^{2}}(t_{i} - t_{i-1})  \\ = \sqrt{x'{(\tau'_{i})}^{2} +  y'{(\tau'_{i})}^{2}} \Delta t_i
$$其中: 
$$
t_{i-1} \leq \tau'_{i} \leq t_{i}
$$
于是: 
$$ 
\int_{L} f(x, y) ds = \lim_{\lambda \to 0}\sum_{i = 1}^{n} f(P_{i})\Delta{L_{i}} = \lim_{\lambda \to 0}\sum_{i = 1}^{n}f[x(\tau_{i}), \space y(\tau_{i})] \sqrt{x'(\tau'_{i})^{2} +  y'(\tau'_{i})^{2}} \Delta{t_{i}} 
$$
因为函数$ \sqrt{x'(t) + y'(t)}$在区间$ [\alpha, \beta]$上连续，且一致连续，则:
对于区间$ [\alpha , \beta] $上的两点
$$ t_{i-1} \leq \tau'_{i} \leq t_{i} \\ t_{i-1} \leq \tau_{i} \leq t_{i}$$
假设:
$$
\tau'_{i} <  \tau_{i}
$$
那么根据函数的**一致连续性**可知：
当$\Delta{\tau} = |\tau_{i} - \tau'_{i} |$小于某个正数$ \delta$时: 
$$ 
| \sqrt{x'(\tau_{i})^{2} + y'(\tau_{i})^{2}} - \sqrt{x'(\tau'_{i})^{2} + y'(\tau'_{i})^{2}}| 
$$
可以小于任意给定的正数$ \epsilon $。 因此，$\sqrt{x'(\tau'_{i})^{2} + y'(\tau'_{i})^{2}} \space \to \sqrt{x'(\tau_{i})^{2} + y'(\tau_{i})^{2}} \space ; \space \tau'_{i} \to \tau_{i}$于是：
$$ 
\int_{L} f(x, y) ds = \lim_{\lambda \to 0} \sum_{i = 1}^{n} f[x(\tau_{i}), \space y(\tau_{i})] \sqrt{x'(\tau_i)^{2} + y'(\tau_i)^{2}} \Delta{t_{i}} \\  = \int_{\alpha }^{\beta} f[x(t), \space y(t)] \sqrt{x'(t)^{2} + y'(t)^{2}} dt \\ \alpha < \beta
$$
证毕

### 三. 计算特殊情形 
如果曲线弧$ L$由函数 
$$ 
x = \Phi{(x)}
$$
给出，那么可以将此看作特殊的参数方程: 
$$ 
L = \left\{
\begin{aligned}
x & =  \Phi{(t)} \\ 
y & = t
\end{aligned}
\right. \\
x_0 \leq (x=t) \leq X
$$
则：
$$ 
\int_{L}f(x, y)ds = \int_{x_0}^{X} f[\Phi(t), \space t]\sqrt{\Phi'(t) + 1}dt = \int_{x_0}^{X} f[x, \space \Phi(x)]\sqrt{ 1 + \Phi'(x)}dx
$$
该方法可以推广到空间中的曲线弧$\Lambda $曲线积分。
如果空间中的曲线弧$ \Lambda $由函数:
$$
\Lambda = \left\{
\begin{aligned}
x & =  \phi{(t)} \\ 
y & = \psi{(t)} \\
z & = \omega{(t)}
\end{aligned}
\right. \\
\alpha \leq  t \leq \beta
$$
则对应的曲线积分：
$$ 
\int_{\Lambda}{f(x, y, z)}ds = \int_{\alpha}^{\beta} f[x(t), \space \psi(t), \space \omega(t)] \sqrt{\phi'(t)^{2} + \psi'(t)^{2} + \omega'(t)^{2}} dt \\ \alpha < \beta
$$

