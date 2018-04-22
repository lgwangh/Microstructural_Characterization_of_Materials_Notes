X射线衍射分析
=============

定性物相分析
------------

标准卡片 PDF
++++++++++++

标准卡片上记载了晶体的： 

- 晶系、空间群、晶格常数
- 光学性质、颜色、其他一些物理性质
- 来源、制备方式
- 衍射面间距、相对衍射峰强度（以最强为100）、晶面指数； **三个最强的被特别标出**
- 实验条件

索引方法
++++++++

相比衍射强度，晶面间距的数据更为准确而不易受影响，因此可以根据最强的三个衍射峰对应的晶面间距进行检索。实际上检索系统综合运用了多种算法。 

定量物相分析
------------

对于多相混合物中的某一相，衍射强度为： 

.. math::

	&I_j=\frac{1}{2\bar{\mu}_l}\left[\frac{V f_j}{V_c^2}P|F|^2L_pe^{-2M}\right]_j\\
	&其中f_j为体积分数，\bar{\mu}_l为试样总体的线吸收系数\\
	&设与f_j无关的部分C_j=\left[\frac{V}{V_c^2}P|F|^2L_pe^{-2M}\right]_j\\
	&则I_j=\frac{C_j f_j}{\bar{\mu}_l}=\frac{C_j f_j}{\rho\bar{\mu}_m}=\frac{C_j \omega_j}{\rho_j\bar{\mu}_m}\\
	&其中质量分数\omega_j满足\sum_{j=1}^n \omega_j=1

一般而言， :math:`\bar{\mu}_m` 随 :math:`f_j` 变化，因而 :math:`I_j` 与 :math:`f_j` 并非线性关系。

直接对比法
++++++++++

对于试样中的 n 种相，各取一根不重叠的衍射钱，以其中一相作为参考（第一相）。则各相强度可表示为： 

.. math::

	&f_j=\frac{C_1 I_j}{C_j I_1}f_1\\
	&结合之前的关系，可知 f_j=\frac{\frac{C_1 I_j}{C_j I_1}}{\sum_{j=1}^n\frac{C_1 I_j}{C_j I_1}}

这样只要确定各物相的 :math:`\frac{C_1}{C_j}` 和 :math:`\frac{I_j}{I_1}` ，就可以确定体积分数。例如测定钢中残余奥氏体的含量：

.. math::

	f_{\gamma}=\frac{1}{1+\frac{C_{\gamma}I_{\alpha}}{C_{\alpha}I_{\gamma}}}


点阵结构分析
------------

可以根据 :math:`I\sim\theta` 曲线计算出点阵常数。对于立方晶系：

.. math::

	&a=\frac{\lambda}{2\sin \theta}\sqrt{H^2+K^2+L^2}\\
	&其中(H\ K\ L)为衍射面指数

误差分析
++++++++

实际上会存在很多误差。包括： 

- 测角仪引起的误差： :math:`2\theta` 的 0° 误差、 :math:`2\theta` 刻度误差、试样表面离轴误差、入射线垂直发散误差
- 试样引起的误差：试样平面性误差、试样晶粒大小误差、试样透明度误差
- 其他误差：角因子偏差、定峰误差、温度变化误差、X射线折射误差、特征辐射非单色误差    

对晶面间距 :math:`d` 取全微分： 

.. math::

	\frac{\Delta d}{d}=\frac{\Delta\lambda}{\lambda}-\frac{\Delta\theta\cos\theta}{\sin\theta}

为了减小误差（即 :math:`|\frac{\Delta d}{d}|` ），应从以下方面入手： 

- 减小 :math:`\Delta\lambda\ \to` 改进X射线源
- 增大 :math:`\lambda\ \to` 使用轻元素作为X射线管靶材，同时会降低分辨率
- 减小 :math:`\Delta \theta\ \to` 改进测角仪
- 增大 :math:`\theta` ，接近 90° 时能消除多种误差 :math:`\to` 选取适当的实验数据

计算方法
++++++++

- 外推法：由于 :math:`\frac{\Delta a}{a}\propto\cos^2\theta` ，取 :math:`\theta>60^\circ` 时的 :math:`(\cos^2\theta,a)` 样本点拟合，其纵截距即为 :math:`a_0` 。对于更低角度的数据，可采用 :math:`(\cos^2\theta(\frac{1}{\sin\theta}+\frac{1}{\theta}),a)` 样本点拟合的方式。
- 内标法：利用已知的内标样品（一般是 :math:`Si` 或 :math:`SiO_2` ），根据 :math:`d_{hkl}\sin\theta_{hkl}=d_s\sin\theta_s` 计算。
- 线对法：利用同一次测量所得到的两根衍射线的线位差值计算点阵参数。

应力测量分析
------------


衍射谱线形分析
--------------
