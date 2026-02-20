# Stokes
> 定义： $ \Lambda$为分段光滑的有向闭曲线，其围成一个分片光滑的有向曲面$ \Sigma$，$ \Lambda$的正向与曲面$ \Sigma$的侧符合右手定则，函数$ P(x, y,z), Q(x, y,z), R(x, y,z) $在曲面$ \Sigma$上（联同边界曲线$ \Lambda$）具有一阶连续偏导数那么有：$$ \iint_{\Sigma} \begin{vmatrix}
dydz & dzdx & dxdy \\
\frac{\partial{}}{\partial{x}} & \frac{\partial{}}{\partial{y}} & \frac{\partial{}}{\partial{z}} \\ 
P & Q & R
\end{vmatrix} = \oint_{\Lambda} Pdx + Qdy + Rdz$$上述公式称为斯托克斯公式，该公式表达了由闭曲线所围成的曲面上的积分与其边界曲线积分之间的关系。

利用两类曲面积分之间的关系可以得到斯托克斯公式的另一种形式：$$ \iint_{\Sigma} \begin{vmatrix}
cos\alpha & cos\beta & cos \gamma \\
\frac{\partial{}}{\partial{x}} & \frac{\partial{}}{\partial{y}} & \frac{\partial{}}{\partial{z}} \\ 
P & Q & R
\end{vmatrix}  = \oint_{\Lambda} Pdx + Qdy + Rdz$$其中的$\bar{n} = (cos\alpha, cos\beta, cos\gamma) $为有向曲面$ \Sigma$在点$ (x, y,z)$的单位法向量。

# 环流量
> 定义：假设存在向量场$$ A(x, y, z) = P(x, y, z) i+ Q(x, y,z) j + R(x, y,z)k$$函数$ P, Q,R$在定义域内均连续，且存在定义域内的一条分段光滑的有向闭曲线$\Lambda$。同时，$ \tau $为该分段光滑有向闭曲线上的一个单位切向量。那么有对于向量场$ A$的环流量 $$ \oint_{\Lambda}A\cdot \tau ds$$

# 旋度

