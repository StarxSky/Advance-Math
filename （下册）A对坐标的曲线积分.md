# 对坐标的曲线积分的概念与性质
>定义： 设$ L$ 为$ xOy$平面上的一条**光滑的有向线弧**，函数$ P(x, y)$和$ Q(x, y)$在该弧段上**有界**。在沿着$L$上插入任意的点$ M_1(x_1, y_1), M_2(x_2, y_2) ..... M_{n - 1}(x_{n - 1}, y_{n -1 }) $将有向弧分成$n$个有向小弧段：$$ \overset{\frown}{M_{i-1}, M_{i}} \space ; \space i \in \{1, 2, 3, ... , n \space ; \space M_{0} = A, M_{n} = B\}$$ 设 ：$$ \Delta x_{i} = x_{i} -  x_{i - 1} \\ \Delta y_{i} = y_{i} - y_{i-1}$$ 同时，点$ (\delta_{i}, \epsilon_{i})$为有向弧段$\overset{\frown}{M_{i-1}, M_{i}} $上取得的任意的一点，做乘积$$ P(\delta_{i}, \epsilon_{i})\Delta x_{i} \space ; \space  i \in (1,2 ,3,4....., n ) $$,并做和式：$$ \sum_{i = 1}^{n}{P(\delta_{i}, \epsilon_{i}) \Delta x_{i} } $$如果当各个弧段之中的最大长度值$\lambda \to 0  $时，该和式存在极限：$$ \lim_{\lambda \to 0}\sum_{i = 1}^{n} {P(\delta_{i}, \epsilon_{i}) \Delta x_{i}}$$
且极限的值与弧段的分发无关，也与点$ (\delta_{i}, \epsilon_{i})$的取法无关，那么此极限称为：**“在弧段$ L$上对坐标$ x$的曲线积分”**.记作：$$ \int_{L} P(x, y) dx = \lim_{\lambda \to 0}\sum_{i = 1}^{n}{P(\delta_{i}, \epsilon_{i}) \Delta x_{i}}$$
同理可得到 **“在弧段$ L$上对坐标$y$的曲线积分”** ：$$ 
\int_{L} Q(x, y)dy = \lim_{\lambda \to 0}\sum_{i = 1}^{n }{Q(\delta_{i}, \epsilon_{i}) \Delta y_{i}}$$
上述两个积分也被称为 **" 第二类曲线积分"** 同时，上述曲线积分可以推广到空间中的有向曲线弧$ \Lambda $上：$$ \int_{\Lambda }P(x, y, z) dx = \lim_{\lambda \to 0}\sum_{i = 1}^{n}{P(\delta_{i}, \epsilon_{i}, \zeta_{i}) \Delta x_{i}} \\ \int_{\Lambda }P(x, y, z) dy = \lim_{\lambda \to 0}\sum_{i = 1}^{n}{P(\delta_{i}, \epsilon_{i}, \zeta_{i}) \Delta y_{i}} \\ \int_{\Lambda }P(x, y, z) dz = \lim_{\lambda \to 0}\sum_{i = 1}^{n}{P(\delta_{i}, \epsilon_{i}, \zeta_{i}) \Delta z_{i}}  $$应用上一般出现：$$ \int_{L}P(x, y) dx + Q(x, y) dy= \int_{L} P(x, y) dx + \int_{L}Q(x, y) dy$$也可以写成向量相乘的形式：$$ \int_{L}F(x, y) \cdot dr $$其中：$$ F(x, y) = P(x, y) + Q(x, y) \\ dr = dx \mathbf{i} + dy \mathbf{j}$$

---
性质：
1. $$ \int_{L}[\alpha F_1(x, y) + \beta F_{2}(x,y) ] \cdot dr = \int_{L}{\alpha F_{1}(x, y) \cdot dr + \int_{L}\beta F_2(x,y) \cdot dr}$$
其中, $\alpha, \beta$ 为任意的常数.

2. 如果有向线段$ L$可以分成两段光滑的有向线段$ L_{1}, \space L_{2}$则：$$ \int_{L}F(x, y) \cdot dr = \int_{L_{1}}F(x, y) \cdot dr + \int_{L_2} F(x, y) \cdot dr$$

3. 对于有向线段弧$ L$,与其相反的方向的反向曲线弧记作$ L^{-}$有：$$ \int_{L^{-}}{F(x, y) \cdot dr} = - \int_{L}{F(x, y) \cdot dr} $$




# 对坐标的曲线积分的计算方法

> 定理：假设存在函数$ P(x, y)$ , $ Q(x, y)$在有向线段弧$ L$上有界且连续，同时该有向线段弧由参数方程$$ x = x(t) \\ y = y(t) $$给出，当参数$ t$递增地由$ \alpha \to \beta $ 相对应的点沿着有向线段弧从$ L$ 的起点$A \to B$，此时，如果函数$ x = x(t) $ 与 $ y = y(t)$在区间$t \in [\alpha , \beta]$上存在连续的一阶导数，同时: $$ x^{'2}(t) + y^{'2}(t) \neq 0 $$那么， $$ \int_{L}P(x, y) dx + Q(x,y) dy $$存在。且有：$$ \int_{L}P(x, y )dx + Q(x,y)dy = \int_{\alpha}^{\beta} \{P[x(t), y(t)]x^{'}(t) + Q[x(t), y(t)]y^{'}(t) \}dt$$
---
证明： 
设$ L$上任意插入点$ M_{1}, M_{2}, M_{3}.....M_{n-1}$将有向线段弧分成$n$个小弧段：$$ \overset{\frown}{M_{i-1}M_{i}} \space ; \space i \in \{1, 2, 3, ... , n \space ; \space M_{0} = A, M_{n} = B\}$$ 与每个点对应的参数值为$\alpha = t_0, t_1, .... , t_{n-1}, t_n = \beta $根据对坐标的曲线积分的定义有：$$ \int_{L} P(x, y) dx = \lim_{\lambda \to 0}\sum_{i = 1}^{n}{P(\delta_{i}, \epsilon_{i}) \Delta x_{i}}$$
此时点$ (\delta_{i}, \epsilon_{i})$对应参数$ \tau_{i} ; \space t_{i-1} < \tau_{i} < t_{i}$ 则： $$ \delta_{i} = x(\tau_{i}) \\ \epsilon_{i} = y(\tau_{i})$$又由于：$$ \Delta x_{i} = x_{i} - x_{i-1} = x(t_{i}) - x(t_{i-1})$$应用拉格朗日积分中值定理：$$ \Delta x_{i} = x^{'}(\tau_{i}^{'}) \Delta t_{i}$$于是$$ \int_{L} P(x,y)dx = \lim_{\lambda \to 0 }\sum_{i = 1}^{n} {P(\delta _{i}, \epsilon_{i}) x^{'}(\tau_{i}^{'})\Delta t_{i}} = \lim_{\lambda \to 0}\sum_{i = 1}^{n}{P[x(\tau_{i}), y(\tau_{i})] x^{'}(\tau^{'}_{i}) \Delta t_{i}}$$
又因为，函数$ P(x, y) $在区间$ [\alpha , \beta ]$上一致连续，因此，这里的$ \tau^{'}_{i}$可以替换为$ \tau_{i}$因此得到：$$ \int_{L} P(x, y) dx = \lim_{\lambda \to 0 }\sum_{i = 1}^{n} {P(\delta _{i}, \epsilon_{i}) x^{'}(\tau_{i})\Delta t_{i}} = \lim_{\lambda \to 0}\sum_{i = 1}^{n}{P[x(\tau_{i}), y(\tau_{i})] x^{'}(\tau_{i}) \Delta t_{i}}$$上述式子的最右边部分的极限为：$$ \int_{\alpha}^{\beta} {P[x(t), \space y(t)] x^{'}(t) dt}$$
因为函数$ P(x(t), y(t))x^{'}(t)$在区间$ [\alpha, \beta]$上连续所以该定积分一定存在。

类似地，我们可以得到$$ \int_{L}{Q(x, y) dy} = \lim_{\lambda \to 0}\sum_{i = 1}^{n}{Q(\delta_{i}, \epsilon_{i}) y^{'}(\tau_{i})\Delta t_{i}} =\int_{\alpha}^{\beta} {Q[x(t), \space y(t)] y^{'}(t) dt}$$

将上述两个最后的定积分相加得到：$$ \int_{L}P(x, y) dx + Q(x,y) dy = \int_{\alpha}^{\beta} {P[x(t), \space y(t)] x^{'}(t) dt + Q[x(t), \space y(t)] y^{'}(t) dt} \\ \space \\ = \int_{\alpha}^{\beta} { \{P[x(t), \space y(t)] x^{'}(t)  + Q[x(t), \space y(t)] y^{'}(t)  \}dt} $$
证毕。


