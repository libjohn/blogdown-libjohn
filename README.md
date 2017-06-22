## README

How to Build this site manually

1. Clone the github repo into RStudio
2. `library(blogdown)` [Resources:  [github](https://github.com/rstudio/blogdown), [Yihui's Book](https://bookdown.org/yihui/blogdown/)]

    - Dependencies:
    
        - devtools::install_github('rstudio/blogdown')
        - blogdown::install_hugo()
        - blogdown::install_theme('jbub/ghostwriter')
    
3. `blogdown::serve_site()`
4. Edit via *Rmarkdown* or *markdown* in the `content` directory and subdirs

    - Initially, you will have edited the `config.toml`, plus `layouts`, and `static` directories (e.g. CSS, templates, etc. and such)

5. Deployment on [Netlify](http://netlify.com)  

    - For Manual Deployment, Optionally stop blogdown server.  Drag `public` directory to netlify.com deploy
    - For Continuous Depolyment, set up according to the [Netlify Docs](https://www.netlify.com/docs/continuous-deployment/) pointing to the `/public` of an appropriate github repository.

        - I used Command = `hugo_0.19`.  I Probably need to follow the [additional steps](https://www.netlify.com/blog/2017/04/11/netlify-plus-hugo-0.20-and-beyond/) for beyond version 0.20, but version 0.19 works and it was easiest.

## ISSUES

- At least on Windows in RStudio (in my experience), trying to use RStudio to git add the `static` and `themes` directories will cause **git** to **hang** or **freeze** within the GIT *GUI* tab.  This may be because there are a large number of files within those directories.  To fix this kill RStudio; delete .git/lock-file ; goto CLI Shell and manually add `static` and `themes` (i.e. `git add static .`)