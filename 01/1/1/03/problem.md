### Simple mathematics
This is fairly simple inline mathematics. Newton would probably be proud about this rendition of $F = ma$,
just like Einstein for this nice and provocative $E = mc^2$, or Schrödinger would praise us for $H\Psi = E\Psi$.

It is easy to cross-reference [@eq:testing-1] too,
$$
    \Int[0][\infty]{e^{-x}}{x} = 1,
$$ {#eq:testing-1}
or if we wish to refer to it with a different word, it can be math block [-@eq:testing-1] too.

and we even have a special `$${ ... }$$` tag for aligned equations,
$${
    a &= b, \\
    c &= d.
}$$


### DeGeŠ macros {#sec:011103-macros}
Why would anyone want to type
$$
    \int\limits_{0}^{\infty} e^{-x^2}\,\mathrm{d}x \quad\text{and}\quad \int\limits_{\partial \Omega} \vec{E}\,\mathrm{d}\Omega,
$$ {#eq:testing-int-ugly}
when you can type a much nicer and semantic
$$
    \Int[0][\infty]{e^{-x^2}}{x} \QText{and} \Int[\pdiff\Omega]{\vec{E}}{\Omega}?
$$ {#eq:testing-int-nice}

Another fine example of a shorthand is
$$
    \Sum[i = 0][n]{2^i a_i} = \Product[j = 0][m]{b_j^3 j^4 + 1}.
$$ {#eq:testing-agg}

We can also do this with sets,
$$
    \Union[i=-\infty][0]{x_i} = \Intersection[j = 0][\infty]{y_j}
$$ {#eq:testing-sets}

#### Derivatives and integrals
Just compare
$$
    \left. \frac{\mathrm{d} f(x)}{\mathrm{d} x} \right|_{x = 0}
    \QText{and}
    \DrvEval{f(x)}{x}{0}.
$$

We also have empty derivatives
$$
    \DrvE[3]{x}{e^{\cos x - \sin x}} +
    \PDrvE[4]{y} f(x, y)
$$
and parenthesized derivatives
$$
    \DrvP[2]{1 + \cos x + \cos^2 x + \cos^3 x}{x}
    \QText{and}
    \PDrvP{\beta^\alpha + \alpha^\beta}{\alpha}
$$

A more complex use case with evaluated expressions and integrals would be
$$
    \Int[0][1]{x^2}{x} =
    \EvalB{\frac{x^3}{3}}{0}[1] =
    \left(\Eval{\frac{x^3}{3}}{x = 1} - \Eval{\frac{x^3}{3}}{x = 0}\right) =
    \left(\frac{1}{3} - 0\right) =
    \frac{1}{3}.
$$

A full list follows:
$$
    \Int[-\infty][0]{x^3}{x} +
    \IntD[\Omega]{\vec{x}}{\vec{S}} +
    \IntDV[\Omega]{x}{S} +
    \IntC[\pdiff \Omega]{\vec{j}}{\vec{\ell}} +
    \IntCV[\pdiff \Omega]{j}{\ell}.
$$

$$
    \IInt[\Real^2]{x^2 + y^2}{x}{y} +
    \IIntP[\Real^2]{x^2 + y^2}{x}{y} +
    1
$$

$${
    \Int[-\infty][\infty]{e^{-x^2}}{x} +
    \IntP{y^3 + 2y^2 - y + 1}{y} \\
}$$

Dot and cross integral and their auto-vectorized versions:
$$
    \IntD[\vec{A}][\vec{B}]{E}{\ell} = \IntDV[\vec{C}][\vec{D}]{E}{\ell},
    \IntC[\pdiff V]{\vec{F} + \vec{G}}{\vec{s}} = \IntCV[\pdiff V]{x}{u}.
$$


#### Three-dimensional integrals
$$
    \IIIntPV[(0, 0, 0)][(1, 1, 1)]{r^2 + 2 r}{\vec{r}}
$$

#### Number sets
Just a couple of shorthands:
$$
    \Natural \subset \Integer \subset \Rational \subset \Real \subset \Complex \subset \Quaternions
$$
and we also have
$$
    \NaturalZero, \RealPos, \RealNeg, \RealNonneg, \RealNonpos
$$
