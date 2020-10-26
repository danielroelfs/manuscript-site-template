---
title: Data
author: Daniel Roelfs
date: 2020-10-25
---

Here is where we can store the data from the publication. Ideally, you'd link all files necessary to rerun the analyses using the scripts from the [code](#code) section of this website. Be aware that the file limit for GitHub respositories is 100MB, so if you want to upload files larger than that (e.g. GWAS summary statistics) you'd need to link it to somewhere else, for instance [Open Science Framework](https://osf.io/) (file size limit of 50GB) or [Academic Torrents](https://academictorrents.com) (no limit). If you want to keep all your files together in the source directory of this site anyway, you can add the files larger than 100MB to the `.gitignore` file to tell Git to not push these files to your repository.

Here's an example of how to link to files in this page:

For instance: [here's a csv file](/data/mtcars.csv)

And [here's a plain text file](/data/plain_text.txt)

This link is generated like this:

    [here's a csv file](/data/mtcars.csv)

Here's how you can link to for instance a file on OSF:

    [Here's a file on OSF](https://osf.io/6tewj/)

Which will look like this:

[Here's a file on OSF](https://osf.io/6tewj/)

Internal links to for instance the [code](#code) section are generated as follows:

    [code](#code) (Note the `#` before the page name)

Populate this page with links and short descriptions of what is linked and a short meaning of the variables. Concise, readable, descriptions are better than really long and complex descriptions, but anything is better than nothing!
