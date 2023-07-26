Now, now, we hate these custom extensions probably as much as you do.
But still sometimes `Markdown` and `pandoc` come a little bit short,
so in the end a few custom hacks and shorthands are included.

### Error tag
The `@E` tag serves as a basic notifier for proofreading:

$$
    2 + 3 = 8
$$

@E What have you written here? This is not correct at all!

### TODO tag
Similarly you can use a `@TODO` tag to mark something as unfinished:

@TODO Finish this example

### Mathematics
The only thing we have so far is the shorthand

    $${
        ...
    }$$

which is functionally equivalent to

    $$
    \begin{aligned}
        ...
    \end{aligned}
    $$

Note that the example is not rendered as verbatim since it is processed before `pandoc`.
