<!---
vim: ft=tex:tw=80
--->

# Lista 1

Gustavo Silveira Frehse - GRR20203927 - 21 de Abril de 2023

## 1

\begin{align*}
    \langle e_i | v \rangle &= \left\langle e_i \middle| \sum \alpha_j e_j \right\rangle\\
    &= \sum \langle e_i | \alpha_j e_j \rangle\\
    &= \sum \alpha_j \langle e_i | e_j \rangle\\
    &= \sum \alpha_j\\
    &= \alpha_i
\end{align*}

## 2
Seja $v = \sum \beta_j e_j$ e $w = \sum \gamma_j e_j$.

Como
\begin{align*}
    \langle u | v \rangle = \langle u | w \rangle, \forall u \in H
    &\Rightarrow \langle e_j | v \rangle = \langle e_j | w \rangle \\
    &\Rightarrow \beta_j = \gamma_j \\
    &\Rightarrow v = w
\end{align*}

e

\begin{equation*}
    v = w \Rightarrow \langle u | v \rangle = \langle u | w \rangle, \forall u \in H
\end{equation*}

então

\begin{equation*}
    v = w \Leftrightarrow \langle u | v \rangle = \langle u | w \rangle, \forall u \in H
\end{equation*}

## 3

### a

Se $L$ é auto-adjunto, então $L^\dagger = L$. Assim

\begin{align*}
    a_{ij} &= \langle e_i | L(e_j) \rangle\\
    &= \langle L^\dagger(e_i) | e_j \rangle\\
    &= \langle L(e_i) | e_j \rangle\\
    &= \overline{\langle e_j | L(e_i) \rangle}\\
    &= \overline{a_{ji}}
\end{align*}

Logo $A = \overline{A}^t$

### b

Se $L$ é unitária então $\langle a | b \rangle = \langle L(a) | L(b) \rangle$.
Assim

\begin{align*}
    \langle a | b \rangle &= \langle L(a) | L(b) \rangle\\
    &= \langle L^\dagger(L(a)) | b \rangle\\
    &\Leftrightarrow a = L^\dagger(L(a))\\
    &\Leftrightarrow L^\dagger = L^{-1}\\
\end{align*}

Seja $B = \overline{A}^t = [b_{ij}]$ e $C = A^{-1} = [c_{ij}]$

\begin{align*}
    b_{ij} &= \overline{\langle e_j | L(e_i) \rangle}\\
    &= \langle L(e_i) | e_j \rangle\\
    &= \langle e_i | L^\dagger e_j \rangle\\
    &= \langle e_i | L^{-1} e_j \rangle\\
    &= c_{ij}
\end{align*}

Logo $B = C$ e portanto $\overline{A}^t = A^{-1}$

## 4

Seja $\lambda$ e $v$ um autovalor e um autovetor de um operador
autoajunto $L$:

\begin{equation*}
    L (v) = \lambda v
\end{equation*}

Assim 

\begin{align*}
    \langle v | L(v) \rangle = \langle L(v) | \lambda v \rangle &\Leftrightarrow
    \langle v | \lambda v \rangle = \langle \lambda v |  v \rangle\\
    &\Leftrightarrow
    \overline{\lambda}\langle v | v \rangle = \lambda\langle v |  v \rangle\\
    &\Leftrightarrow \overline{\lambda} = \lambda\\
    &\Leftrightarrow \lambda \in \mathbb{R}
\end{align*}

