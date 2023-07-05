### Basic pictures {#sec:pictures}
The simplest case is including a picture that does not have to be changed anyhow,
just pasted into the document as-is:

![PDFs, PNGs and JPGs can be included directly](smiley.png){height=30mm #fig:smiley}

DeGeŠ will accept a missing or nonexistent picture as well:

![Missing picture](missing.pdf){height=40mm #fig:missing}

### Special cases {#sec:pictures-special}
For `SVG` files you can specify the extension naturally but DeGeŠ will
correctly convert it to a PDF file before embedding it in the \LaTeX\ build,
and will include it directly in HTML output:

![An example of a Scalable Vector Graphics file](scalable.svg){height=35mm #fig:scalable}

We even support plotting `gnuplot` files directly. There is a simple common framework
that adds the basic structure but it can be overridden. Just add it like this:

![A sample `gnuplot` plot](gnuplot.gp){height=50mm #fig:gnuplot}
