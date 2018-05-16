---
title: Slide Template Using Duke University Color Palette & xaringan
author: John Little
date: '2018-05-15'
slug: slide-template-using-duke-university-color-palette-xaringan
categories:
  - Markdown
  - R
tags:
  - Xaringan
  - Slides
  - template
  - color palette
---

[Previously I wrote](post/compose-slides-in-r-with-xaringan-slides/) about Yihui Xie's [xaringan](https://slides.yihui.name/xaringan/) slides.  It's a great [package](https://github.com/yihui/xaringan) combining R Markdown with the remark.js slide tools and some Yihui Xie ingenuity. I was a fan when it came out and I'm a bigger fan after multiple uses.  In my mind, xaringan is perfection in need of only one small personal customization.  I wanted one feature:  an **R Markdown document template** that **stores** some of *my typical slide themes* **combined** with a *custom stylesheet* (CSS) for the [Duke University color palette](https://styleguide.duke.edu/color-palette/).  So I created the R Markdown document template as [`dukeslides`](/dukeslides/) ...

![thumbnails of slides: 1](/dukeslides/images/thumbs1.png) 

Here's how it works:

## Installation

**Install** the *development version* from [GitHub](https://github.com/) with:

``` r
# install.packages("devtools")
devtools::install_github("libjohn/dukeslides")
```
## Get Started

Create a new R Markdown document from the File menu 

In RStudio...

1. `New File -> R Markdown -> From Template -> Slide template for Duke University  {dukeslides}`
2. Click the `Knit` button to compile the slide into rendered HTML

Check out the [`dukeslides` documentation](http://www.johnlittle.info/dukeslides/) for more information, tutorials, documentation, bug reports, etc. To quickly see thumbnails illustrating the color palette via xaringan simply scroll through this post.

![thumbnails of slides: 2](/dukeslides/images/thumbs2.png) 

## Why did I do it?

Missing or wanting a feature in R/RStudio is an open invitation to learn something new.  Then, ideally, share a newly developed feature with other like-minded users.  Most likely the other like-minded users of `dukeslides` with R/R Markdown are already at Duke University, but that doesn't have to be true.  Others can use this Duke color palette without using the image/logo branding.  And, why not?  After all, &lt;blinking bias &gt;I think the Duke University colors are quite nice. &lt;/blinking bias&gt;

![thumbnails of slides: 3](/dukeslides/images/thumbs3.png) 

## Contributing custom CSS to xaringan 

Last October, Yihui Xie [requested help developing CSS themes](https://yihui.name/en/2017/10/xaringan-themes/). In response, you can find a nice and growing collection of CSS themes easily accessible by xaringan users.  After installing the xaringan package, type the following to see what is available: 

``` r
names(xaringan:::list_css())
```

More customization is still possible.  The process of contributing custom CSS stylesheets to xaringan [is referenced](https://slides.yihui.name/xaringan/#35) in the xaringan documentation. Now you can help by adapting and contributing more stylesheet themes.  

![thumbnails of slides: 4](/dukeslides/images/thumbs4.png) 


## Making an R Markdown Document Template

The other part of making a custom theme goes beyond the color palette.  For example, I use boilerplate closing slides in almost every presentation listing my name, position, department, etc.  Similarly, the markdown for making two column slides or colored boxes is not always in the top of my mind.  So, I created an R Markdown document template that has all of these common elements.  I find the document template more convenient than looking up syntax each time.  With this technique, I simply delete or customize the boilerplate markdown as needed.  

![thumbnails of slides: 5](/dukeslides/images/thumbs5.png) 

### What I learned

R Markdown document templates are easy to create.  The process requires reading only a brief document.  The challenge, however, may be in the need to create a package for redistribution of the document template.  According to what I read, *R Markdown templates are typically re-distributed within* **R packages**.  

> Learning Option #2:  how to make a package.


### Creating A Package

This too turns out to be straightforward.  After making my first document template as `dukeslides`, I plan to make a few more document templates since I tend to use R Notebooks with boilerplate text as well.  Now making a package sounds like a lot of work, and maybe it is.  Nevertheless, even if making a package with custom functions is technically challenging, making a document template is not a huge amount of work or overly technical.  And, bonus, making a document template helps you learn some of what you'll need to know if you decide to make a package with functions.


#### Here's How

[Read this documentation about document templates](https://rmarkdown.rstudio.com/developer_document_templates.html) and then leverage some other awesome packages.  The indispensable packages are `usethis` and `devtools`.  You can simplify and assist writing documentation for your package with `pkgdown`.  I'll refrain from describing this process in detail in favor of linking to some of the documentation I found useful.

- [`usethis`](http://usethis.r-lib.org/)
- Jim Hester's presentation from RStudio 2018 [[slides](https://www.rstudio.com/resources/videos/you-can-make-a-package-in-20-minutes/) | [streaming](https://www.rstudio.com/resources/videos/you-can-make-a-package-in-20-minutes/)]
- pkgdown [[documenation](http://pkgdown.r-lib.org/) | [article](http://pkgdown.r-lib.org/)]
- Quick-start:  Hilary Parker's [Writing an R package](https://hilaryparker.com/2014/04/29/writing-an-r-package-from-scratch/) 
- [Making Your First R Package](http://tinyheero.github.io/jekyll/update/2015/07/26/making-your-first-R-package.html)
- [How to develop good R packages](http://www.masalmon.eu/2017/12/11/goodrpackages/)
- [R Packages](http://r-pkgs.had.co.nz/) book by Hadley Wickham
- [Package Development Workshop materials](https://github.com/forwards/workshops/tree/master/eRum2018) presented at eRum2018
