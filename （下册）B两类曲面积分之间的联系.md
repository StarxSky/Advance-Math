### 两类曲面积分之间的联系

首先给出曲面$ \Sigma$由方程$ z = z(x, y)$确定，有关两类曲面积分之间的联系的结论：$$ \boxed{\iint_{\Sigma} P(x, y, z) dydz + Q(x, y, z) dzdx + R(x, y, z)dxdy \\ = \iint_{\Sigma} {[Pcos\alpha + Qcos\beta + Rcos\gamma ]} dS  }$$
其中，$$ dS = \sqrt{1 + z_{x}^{2} + z_{y}^{2} } dxdy$$ $$ n = (cos \alpha , cos \beta, cos \gamma) = (\frac{-\frac{\partial{z}}{\partial{x}}}{\sqrt{1 + \left(\frac{\partial{z}}{\partial{x}}\right)^{2} + \left(\frac{\partial{z}}{\partial{y}}\right)^{2}}}, \frac{-\frac{\partial{z}}{\partial{y}}}{\sqrt{1 + \left(\frac{\partial{z}}{\partial{x}}\right)^{2} + \left(\frac{\partial{z}}{\partial{y}}\right)^{2}}}, \frac{1}{\sqrt{1 + \left(\frac{\partial{z}}{\partial{x}}\right)^{2} + \left(\frac{\partial{z}}{\partial{y}}\right)^{2}}})$$ 为曲面$ \Sigma$的单位法向量。该法向量是通过对平面方程$$ F(x, y,z) = z - z(x, y) $$求其梯度：$$ \nabla F = (-\frac{\partial{z}}{\partial{x}},- \frac{\partial{z}}{\partial{y}}, 1)$$得到的。

---

该式子也可以记作向量形式：$$ \boxed{\iint_{\Sigma} {\bar{A} \cdot \bar{dS}} = \iint_{\Sigma} {\bar{A }\cdot \bar{n}dS} }$$其中$ A = (P, Q, R)$ 并且$ n = (cos \alpha, cos \beta , cos \gamma)$且$$ \bar{dS} = \bar{n} dS = (dydz, dzdx, dxdy)$$
 