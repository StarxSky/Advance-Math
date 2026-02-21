# Stokes
> 定义： $ \Lambda$为分段光滑的有向闭曲线，其围成一个分片光滑的有向曲面$ \Sigma$，$ \Lambda$的正向与曲面$ \Sigma$的侧符合右手定则，函数$ P(x, y,z), Q(x, y,z), R(x, y,z) $在曲面$ \Sigma$上（联同边界曲线$ \Lambda$）具有一阶连续偏导数那么有：$$ \iint_{\Sigma} \begin{vmatrix}
dydz & dzdx & dxdy \\
\frac{\partial{}}{\partial{x}} & \frac{\partial{}}{\partial{y}} & \frac{\partial{}}{\partial{z}} \\ 
P & Q & R
\end{vmatrix} = \oint_{\Lambda} Pdx + Qdy + Rdz$$上述公式称为斯托克斯公式，该公式表达了由闭曲线所围成的曲面上的积分与其边界曲线积分之间的关系。

利用两类曲面积分之间的关系可以得到斯托克斯公式的另一种形式：$$ \boxed{\iint_{\Sigma} \begin{vmatrix}
cos\alpha & cos\beta & cos \gamma \\
\frac{\partial{}}{\partial{x}} & \frac{\partial{}}{\partial{y}} & \frac{\partial{}}{\partial{z}} \\ 
P & Q & R
\end{vmatrix} dS = \oint_{\Lambda} Pdx + Qdy + Rdz}$$其中的$\bar{n} = (cos\alpha, cos\beta, cos\gamma) $为有向曲面$ \Sigma$在点$ (x, y,z)$的单位法向量。

# 环流量
> 定义：假设存在向量场$$ A(x, y, z) = P(x, y, z) i+ Q(x, y,z) j + R(x, y,z)k$$函数$ P, Q,R$在定义域内均连续，且存在定义域内的一条分段光滑的有向闭曲线$\Lambda$。同时，$ \tau $为该分段光滑有向闭曲线上的一个单位切向量。那么有对于向量场$ A$的环流量 $$ \boxed{\oint_{\Lambda}A\cdot \tau ds}$$
根据两类曲线积分之间的关系有：$$\boxed{\oint_{\Lambda} A\cdot \tau ds = \oint_{\Lambda} A\cdot dr = \oint_{\Lambda} Pdx +Qdy +Rdz}$$其中，$$ \tau ds = dr = (dx , dy, dz)$$这是因为我们假设该闭曲线$\Lambda$由向量方程：$$\Lambda :\space r = x(t)i + y(t)j + z(t)k$$所确定。而$ \tau = (cos\alpha, cos\beta, cos\gamma)$为该曲线的一个单位切向量。且$ ds = \sqrt{x^{'2}+y^{'2}+z^{'2}}dt$。因此：$$ \tau ds = (x^{'}, y^{'}, z^{'})=(dx, dy, dz) = dr$$


# 旋度

> 定义： 假设存在一个向量场：$$ A(x, y,z) = P(x, y,z)i + Q(x, y,z)j + R(x, y,z)k $$其中函数$P, Q, R$均连续，且可一阶连续偏导。那么称:$$ \begin{vmatrix}
i & j & k \\
\frac{\partial{}}{\partial{x}} & \frac{\partial{}}{\partial{y}} & \frac{\partial{}}{\partial{z}} \\ 
P & Q & R
\end{vmatrix} =(\frac{\partial{R}}{\partial{y}} -\frac{\partial{Q}}{\partial{z}})i + (\frac{\partial{P}}{\partial{z}} - \frac{\partial{R}}{\partial{x}})j +(\frac{\partial{Q}}{\partial{x}} - \frac{\partial{R}}{\partial{y}})k $$为向量场$ A$的**旋度**记作：$$ \boxed{\mathbf{rot}(A) = \nabla \times A = \begin{vmatrix}
i & j & k \\
\frac{\partial{}}{\partial{x}} & \frac{\partial{}}{\partial{y}} & \frac{\partial{}}{\partial{z}} \\ 
P & Q & R
\end{vmatrix}}$$
若向量场$A$的旋度处处为零，那么向量场称为**无源场**。而一个**无源**，**无旋度**的场称为**调和场**: $$ \mathbf{div}(A) = 0 ; \mathbf{rot}(A) =0$$


利用两类曲面积分之间的关系可以得到斯托克斯公式的另一种形式：$$ \iint_{\Sigma} \begin{vmatrix}
cos\alpha & cos\beta & cos \gamma \\
\frac{\partial{}}{\partial{x}} & \frac{\partial{}}{\partial{y}} & \frac{\partial{}}{\partial{z}} \\ 
P & Q & R
\end{vmatrix} dS  = \oint_{\Lambda} Pdx + Qdy + Rdz$$其中的$\bar{n} = (cos\alpha, cos\beta, cos\gamma) $为有向曲面$ \Sigma$在点$ (x, y,z)$的单位法向量。根据旋度的定义，我们可以将斯托克斯公式改写为：$$ \boxed{ \iint_{\Sigma} \begin{vmatrix}
cos\alpha & cos\beta & cos \gamma \\
\frac{\partial{}}{\partial{x}} & \frac{\partial{}}{\partial{y}} & \frac{\partial{}}{\partial{z}} \\ 
P & Q & R
\end{vmatrix} dS = \iint_{\Sigma}\mathbf{rot}(A) \cdot \mathbf{\bar{n}}  dS  = \iint_{\Sigma}\mathbf{rot}(A)\cdot \bar{dS} = \oint_{\Lambda} Pdx + Qdy + Rdz }$$又因为：$$ \oint_{\Lambda} A\cdot \tau ds = \oint_{\Lambda} A\cdot dr = \oint_{\Lambda} Pdx +Qdy +Rdz$$因此：$$\boxed{\iint_{\Sigma}\mathbf{rot}(A) \cdot \bar{dS} = \oint_{\Lambda} A \cdot \tau ds }$$
