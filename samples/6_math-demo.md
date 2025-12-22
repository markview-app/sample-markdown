# Mathematical Equations & Formulas Demo

> **MarkView** renders beautiful LaTeX math equations with KaTeX — perfect for scientific and technical documentation.

## Fundamental Mathematics

### Basic Equations

The most famous equation in physics:

$$E = mc^2$$

The quadratic formula for solving $ax^2 + bx + c = 0$:

$$x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$$

Euler's identity, called "the most beautiful equation":

$$e^{i\pi} + 1 = 0$$

---

## Calculus & Analysis

### Derivatives

The definition of a derivative:

$$f'(x) = \lim_{h \to 0} \frac{f(x + h) - f(x)}{h}$$

The power rule:

$$\frac{d}{dx}(x^n) = nx^{n-1}$$

The product rule for $u(x)$ and $v(x)$:

$$\frac{d}{dx}[u(x)v(x)] = u'(x)v(x) + u(x)v'(x)$$

### Integrals

The fundamental theorem of calculus:

$$\int_a^b f(x) \, dx = F(b) - F(a)$$

Integration by parts:

$$\int u \, dv = uv - \int v \, du$$

A beautiful definite integral:

$$\int_0^\infty e^{-x^2} \, dx = \frac{\sqrt{\pi}}{2}$$

---

## Linear Algebra

### Matrices

A general $m \times n$ matrix:

$$
A = \begin{pmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mn}
\end{pmatrix}
$$

Matrix multiplication for $C = AB$:

$$c_{ij} = \sum_{k=1}^n a_{ik}b_{kj}$$

The determinant of a $2 \times 2$ matrix:

$$
\det\begin{pmatrix} a & b \\ c & d \end{pmatrix} = ad - bc
$$

### Vector Operations

The dot product of vectors $\mathbf{a}$ and $\mathbf{b}$:

$$\mathbf{a} \cdot \mathbf{b} = \sum_{i=1}^n a_i b_i = |\mathbf{a}||\mathbf{b}|\cos\theta$$

The cross product in 3D:

$$
\mathbf{a} \times \mathbf{b} = \begin{vmatrix}
\mathbf{i} & \mathbf{j} & \mathbf{k} \\
a_1 & a_2 & a_3 \\
b_1 & b_2 & b_3
\end{vmatrix}
$$

---

## Probability & Statistics

### Probability Distributions

The probability density function of the normal distribution:

$$f(x) = \frac{1}{\sigma\sqrt{2\pi}} e^{-\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^2}$$

The binomial probability mass function:

$$P(X = k) = \binom{n}{k} p^k (1-p)^{n-k}$$

Bayes' theorem:

$$P(A|B) = \frac{P(B|A)P(A)}{P(B)}$$

### Statistical Measures

The sample mean:

$$\bar{x} = \frac{1}{n}\sum_{i=1}^n x_i$$

The sample variance:

$$s^2 = \frac{1}{n-1}\sum_{i=1}^n (x_i - \bar{x})^2$$

The correlation coefficient:

$$r = \frac{\sum_{i=1}^n (x_i - \bar{x})(y_i - \bar{y})}{\sqrt{\sum_{i=1}^n (x_i - \bar{x})^2 \sum_{i=1}^n (y_i - \bar{y})^2}}$$

---

## Sequences & Series

### Famous Series

The Taylor series expansion of $e^x$:

$$e^x = \sum_{n=0}^\infty \frac{x^n}{n!} = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \cdots$$

The geometric series:

$$\sum_{n=0}^\infty ar^n = \frac{a}{1-r}, \quad |r| < 1$$

The harmonic series (divergent):

$$\sum_{n=1}^\infty \frac{1}{n} = 1 + \frac{1}{2} + \frac{1}{3} + \frac{1}{4} + \cdots$$

### Limits

The definition of $e$:

$$e = \lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n$$

L'Hôpital's rule for $\frac{0}{0}$ forms:

$$\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{x \to a} \frac{f'(x)}{g'(x)}$$

---

## Complex Analysis

### Complex Numbers

The complex exponential (Euler's formula):

$$e^{i\theta} = \cos\theta + i\sin\theta$$

De Moivre's theorem:

$$(\cos\theta + i\sin\theta)^n = \cos(n\theta) + i\sin(n\theta)$$

The magnitude of a complex number $z = a + bi$:

$$|z| = \sqrt{a^2 + b^2}$$

### Complex Functions

The Cauchy-Riemann equations for $f(z) = u + iv$:

$$
\frac{\partial u}{\partial x} = \frac{\partial v}{\partial y}, \quad
\frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x}
$$

The residue theorem:

$$\oint_C f(z) \, dz = 2\pi i \sum_{k=1}^n \text{Res}(f, z_k)$$

---

## Differential Equations

### Ordinary Differential Equations

The general first-order linear ODE:

$$\frac{dy}{dx} + P(x)y = Q(x)$$

Solution using integrating factor $\mu(x) = e^{\int P(x)dx}$:

$$y = \frac{1}{\mu(x)}\left[\int \mu(x)Q(x)dx + C\right]$$

### Partial Differential Equations

The heat equation:

$$\frac{\partial u}{\partial t} = \alpha \frac{\partial^2 u}{\partial x^2}$$

The wave equation:

$$\frac{\partial^2 u}{\partial t^2} = c^2 \frac{\partial^2 u}{\partial x^2}$$

Laplace's equation:

$$\nabla^2 u = \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} + \frac{\partial^2 u}{\partial z^2} = 0$$

---

## Advanced Topics

### Fourier Analysis

The Fourier series:

$$f(x) = \frac{a_0}{2} + \sum_{n=1}^\infty \left(a_n \cos\frac{n\pi x}{L} + b_n \sin\frac{n\pi x}{L}\right)$$

The Fourier transform:

$$\hat{f}(\omega) = \int_{-\infty}^\infty f(t)e^{-i\omega t} \, dt$$

The inverse Fourier transform:

$$f(t) = \frac{1}{2\pi}\int_{-\infty}^\infty \hat{f}(\omega)e^{i\omega t} \, d\omega$$

### Quantum Mechanics

The Schrödinger equation:

$$i\hbar\frac{\partial}{\partial t}\Psi(\mathbf{r},t) = \hat{H}\Psi(\mathbf{r},t)$$

The Heisenberg uncertainty principle:

$$\Delta x \cdot \Delta p \geq \frac{\hbar}{2}$$

### Machine Learning

The softmax function:

$$\sigma(\mathbf{z})_i = \frac{e^{z_i}}{\sum_{j=1}^K e^{z_j}}$$

Cross-entropy loss:

$$L = -\sum_{i=1}^n y_i \log(\hat{y}_i)$$

Gradient descent update rule:

$$\theta_{t+1} = \theta_t - \alpha \nabla_\theta J(\theta_t)$$

---

## Systems of Equations

### Linear Systems

A system in matrix form $A\mathbf{x} = \mathbf{b}$:

$$
\begin{pmatrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33}
\end{pmatrix}
\begin{pmatrix}
x_1 \\ x_2 \\ x_3
\end{pmatrix}
=
\begin{pmatrix}
b_1 \\ b_2 \\ b_3
\end{pmatrix}
$$

Cramer's rule for $x_i$:

$$x_i = \frac{\det(A_i)}{\det(A)}$$

---

## Inline Mathematics

You can write equations inline like $f(x) = ax^2 + bx + c$ or $\sum_{i=1}^n i = \frac{n(n+1)}{2}$ within paragraphs. This is useful for discussing mathematical concepts in flowing text, such as when we say that the derivative $\frac{dy}{dx}$ represents the instantaneous rate of change, or when we mention that $\pi \approx 3.14159$.

The golden ratio $\varphi = \frac{1 + \sqrt{5}}{2}$ appears frequently in nature and art. Similarly, the imaginary unit $i = \sqrt{-1}$ is fundamental to complex analysis.

---

## Special Characters & Symbols

Greek letters: $\alpha, \beta, \gamma, \delta, \epsilon, \theta, \lambda, \mu, \pi, \sigma, \omega$

Operators: $\sum, \prod, \int, \oint, \nabla, \partial, \infty$

Relations: $\leq, \geq, \neq, \approx, \equiv, \propto$

Set theory: $\in, \notin, \subset, \subseteq, \cup, \cap, \emptyset$

Logic: $\forall, \exists, \neg, \land, \lor, \implies, \iff$

Arrows: $\rightarrow, \Rightarrow, \leftrightarrow, \Leftrightarrow$

This comprehensive collection demonstrates the power of KaTeX! 📐✨
