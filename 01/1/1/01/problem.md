### Basic text
This is our first sample paragraph. It does not say much.

If we want to start a new one, we need to include one empty line.
More empty lines work just the same, but don't add anything else of any value,
so we should not write like that.

We often like to _emphasize something_ or make it **bold**. Or sometimes even ***both at the same time***!
Sometimes we also like to write text in `monospace`, for instance code or variable names.
If we need a footnote^[and we often do], we can do it like this.

Pay attention to quotes: DeGeŠ processes text "automatically" and selects proper quotation marks for the language.


#### Deeper levels
Most DeGeŠ documents use first and second section levels for their internal structure,
leaving third and higher levels, such as `\subsection{}` or `<h3>...</h3>` and so forth for general use.

##### Exceptions
Of course, if your template class is defined differently, no one is stopping you from changing this.

### Lists
We have included the `enumitem` package and can write lists nicely.
There are many reasons to use \LaTeX.

-   Perhaps the best thing about \LaTeX\ is its ability to typeset mathematics.
-   Or maybe that we can split, compose and template documents, as opposed to storing them
    in a single mysterious file.
-   And store files in `git` in reasonable directories.

However sometimes \LaTeX\ is way too verbose, too powerful and allows us to do too much.
This is where DeGeŠ comes in:

1.  Instead of \LaTeX, we write stuff in `Markdown`.
    It is not that powerful and does not allow that much, but it is often a good thing.
    With `pandoc` it can be converted to \LaTeX\ easily. Or to `HTML` as well:
    sometimes having a structured, clickable document is much better than
    a perhaps prettier but cumbersome PDF file.
1.  We avoid a ton of boilerplate. Just compare including a picture, see [-@sec:pictures].
1.  We can store files in a structured way, especially if the documents have
    a firmly set structure that repeats in various issues.
1.  We provide a huge number of custom macros (see section [-@sec:011103-problem]) that are much easier to memorize (and also type).
    They work both with \LaTeX\ and HTML, which is great.
    And if we wish to use them outside DeGeŠ, no problem.
1.  We can avoid most typographic corrections in the text: no more manual `\,` or `\!`.
    Seriously, if you ever find yourself using those in a document, something is very wrong.

### Unicode
Note the fancy Greek letters
$$
    \alpha \beta \gamma \delta \epsilon \zeta \eta \theta \iota \kappa \lambda
    \mu \nu \xi \omicron \pi \rho \sigma \tau \upsilon \phi \chi \psi \omega
    \varepsilon \varphi \varkappa \varpi
$$
however since we are using XeLaTeX, we can write Greek directly as
«Πάνω στην άμμο την ξανθή γράψαμε τ’ όνομά της· ωραία που φύσηξεν ο μπάτης και σβήστηκε η γραφή.»
or Ukrainian... Будь ласка, напишіть мені, якщо вам щось потрібно.
