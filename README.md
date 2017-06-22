## README

How to Build this site manually

1. Clone the github repo into RStudio
2. library(blogdown)

    - Dependencies:
    - devtools::install_github('rstudio/blogdown')
    - blogdown::install_hugo()
    - blogdown::install_theme('jbub/ghostwriter')
    
3. blogdown::serve_site()
4. Edit via Rmarkdown or markdown in the `content` directory and subdirs

    - Initially you would have edited the `config.toml`, plus `layouts`, and `static` directories

5. For Manual Deployment...  Stop blogdown server; drag `public` directory to netlify.com deploy

## ISSUES

- At least on Windows in RStudio (in my experience), trying to use RStudio to git add the `static` and `themes` directories will cause **git** to **hang** or **freeze** within the GIT *GUI* tab.  This may be because there are a large number of files within those directories.  To fix this kill RStudio; delete .git/lock-file ; goto CLI Shell and manually add `static` and `themes` (i.e. `git add static .`)