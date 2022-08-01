---
title: "Resources"
date: 2022-07-24T16:19:23-04:00
math: true
draft: false
---

WolframAlpha

Geogebra

Desmos 

Paulsnotes

MyNotes

*your*Notes ;)

[Algebra](/algebra)

# Gauss' Divergence Theorem
Let $\textit{W}$ be a symmetric elementary region in space. Denote by $\delta W$ the oriented closed surface that bounds \textit{W}. Let \textbf{F} be a smooth vector field defined on \textit{W}. Then:

$$\iiint_{W}^{} (\Delta \cdot \textbf{F}) dV = \iint_{\partial W}^{} \textbf{F} \cdot dS.$$

$$
\begin{tikzpicture}
\begin{axis}
\addplot[color=red]{exp(x)};
\end{axis}
\end{tikzpicture}
%Here ends the 2D plot
\hskip 5pt
%Here begins the 3D plot
\begin{tikzpicture}
\begin{axis}
\addplot3[
    surf,
]
{exp(-x^2-y^2)*x};
\end{axis}
\end{tikzpicture}
%Here ends the 3D plot

\end{document}
$$
