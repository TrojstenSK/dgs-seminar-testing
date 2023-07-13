Now, now, we hate these custom extensions probably as much as you do.
But still sometimes `Markdown` and `pandoc` come a little bit short,
so in the end a few custom hacks and shorthands are included.

### Error tag
Serves as a basic notifier for proofreading:

$$
    2 + 3 = 8
$$

@E What have you written here? This is not correct at all!

### TODO tag

@TODO Finish this example

### Mathematics
The only thing we have so far is a shorthand

    $${ 
        ...
    }$$ 

which is functionally equivalent to

    $$
    \begin{aligned}
        ...
    \end{aligned}
    $$
