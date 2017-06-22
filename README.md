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