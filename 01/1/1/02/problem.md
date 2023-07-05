One of the greatest contributions to the sweet world of \TeX\ is the `siunitx` package,
which enables us to write physical units in a concise, semantic way. While strictly speaking
they do not need to be enclosed in `$...$` math mode, in DeGeŠ it is necessary as long as
HTML output is desired, since otherwise they would not be processed.
This will hopefully changed in future releases.

### Basic units
We know that $c = \SI{299792458}{\metre\per\second}$ and that
$G \approx \SI{6.67430(15)e-11}{\cubic\metre\per\kilo\gram\per\second\squared}$.
$$
    \SI{20}{\metre\per\second} \cdot \SI{4.6}{\kilo\newton} = \SI{92}{\kilo\watt}.
$$

### Angles
In this section we show how angles are formed. For instance $\ang{10} + \ang{10.5 +- 4}$.

$\ang{73;14;22.3} + \ang{114;35;19.4} = \ang{187;49;41.7} \doteq \ang{187.82}$

### Ranges
\numrange{33}{37} crows are flying at \SIrange{31}{35}{\metre\per\second}
and \numrange[range-phrase={ to }]{4}{6} ducks are swimming at
\SIrange[range-phrase={ to }]{30}{45}{\atto\parsec\per\second}.

### Number and unit lists
Prime numbers are \numlist{2;3;5;7;11;13;17} and some nice lengths are \SIlist{4;6;8;12;16}{\micro\metre}.
And we can rap about \SIlist[list-separator={ and }]{5;5;5}{\milli\litre}.
