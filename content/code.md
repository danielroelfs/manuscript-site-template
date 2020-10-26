---
title: Code
author: Daniel Roelfs
date: 2020-10-25
output:
  md_document:
    preserve_yaml: TRUE
---

This page serves to document the code associated with your paper. I’d
recommend not to copy-paste the code from your scripts verbatim in here,
but instead to use this page to document the organization of the
different scripts.

For instance, here’s an R script that does some stuff: [here’s an R
script](scripts/example_r.R)

And for good measure, here’s a Python script: [here’s a Python
script](scripts/example_python.py)

I recommend that you use simple markdown to write this document. It is
the simplest and most consistent way. Add your scripts to the
`files/scripts/` folder in the website root directory. Link the scripts
with the code above and add a description to inform the reader about the
purpose of each script. Obviously, it’s still important to have
well-commented code within your scripts, but this script serves to guide
the reader through the pipeline, and to document how the scripts link
together.

Because I know this functionality will be appreciated by some, I also
added the possibility to knit Rmarkdown documents to markdown (see the
`code.Rmd` file in the `content/` directory). You can go into any text
editor you use to edit the other `.md` files. Example will follow later.

Now let’s see what we can do when we knit in Rmarkdown. Here’s some code
loading a package:

    library(tidyverse)

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.0 ──

    ## ✔ ggplot2 3.3.2     ✔ purrr   0.3.4
    ## ✔ tibble  3.0.4     ✔ dplyr   1.0.2
    ## ✔ tidyr   1.1.2     ✔ stringr 1.4.0
    ## ✔ readr   1.4.0     ✔ forcats 0.5.0

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()

And here’s a random plot:

    ggplot(mtcars, aes(x = wt, y = mpg)) + 
      geom_point() +
      geom_smooth() +
      labs(x = "Weight (x 1000lbs)",
           y = "Miles per Gallon") +
      theme_minimal()

    ## `geom_smooth()` using method = 'loess' and formula 'y ~ x'

![](code_files/figure-markdown_strict/example-plot-1.png)

The `.md` file will show something like
this:

    ![](code_files/figure-markdown_strict/example-plot-1.png)

Here also counts:

> “I didn’t have time to write a short letter, so I wrote a long one
> instead.”
>
> \- Mark Twain

Or: anything is better than nothing
