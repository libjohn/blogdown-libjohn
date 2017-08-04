+++
title = "R Markdown is so very Reproducible"
author = "John Little"
date= "2017-08-03"
# slug = "rmark2"
categories = [
  "Markdown",
  "R",
  "Blog Thoughts",
  "Reproducibility"
]
tags = [
  "Markdown", 
  "Reproducibility", 
  "R Markdown"
]
math = false
summary = "R Markdown is the backbone of R's dynamic documents, literate data science, and reproducibility."


# Optional featured image (relative to `static/img/` folder).  
[header]
image = "headers/RMarkdownFlow.png"
caption = "Image credit: [**R Markdown by RStudio**](http://rmarkdown.rstudio.com/authoring_quick_tour.html)"
+++


## R Markdown is Awesome

*R Markdown is Awwwwwesoommmmmme*.  There, I said it. See, I have this nifty [new website](/).  It's produced via Blog*down* and **composed in R Markdown**.  To feed my blog section I plan on writing occasional posts such as this one.  But where do I start? (“Begin at the beginning," the King said, very gravely[^1]) ...  

These days I use R, a lot and  I use R Markdown to compose reports while documenting analysis. R scripts, R Notebooks, are composable with R Markdown.  Using R Markdown I wrote an e-book for an OpenRefine workshop, this website, web dashboards, and interactive quizzes.  I make slide presentations constantly.  Different packages make this activity possible but the common thread, aside from R, is R Markdown.  Initially, I was going to launch my blog with a post about [Xaringan slides](https://slides.yihui.name/xaringan/).  Then I realized I need to lead with R Markdown -- duh -- because R Markdown enhances the readability and document structure for many reports enabled with R/RStudio.  I'll come back to Xaringan slides another day.

### Why use R Markdown

R Markdown is easy to learn and easy to use.  When used with RStudio, R Markdown will enable report derivatives while the content remains readable and reproducible.  It's a benevolent cycle:  write a document once in R Markdown, derive reports with minimal effort, maintain the whole project with readable source material. In this way you put [*literate programming*](https://en.wikipedia.org/wiki/Literate_programming) into practice by generating your reports from your code.  Notably you don't need to be a coder or an analyst to benefit from using R Markdown as your document generator.  With R Markdown you can transform your content into many formats including slides, journal articles, PDF, Word files, web pages, web dashboards, web sites, dynamic quizzes, LaTex.  (But wait, there's more!)

![](/post/2017-08-03-rmarkdown/RMarkdownOutputFormats.png "Image Credit:  RStudio RMarkdown Output Formats http://rmarkdown.rstudio.com/authoring_quick_tour.html")
<!-- Image Credit:  RStudio http://rmarkdown.rstudio.com/authoring_quick_tour.html -->  

### What is R Markdown

R Markdown is a flavor of Markdown.  Markdown is a lightweight "language" used to add structure to text.  The mark*down* goal is to simplify mark*up* languages. The resulting simplicity means the content is less cluttered and easier to read. Easier because mark*up* languages are intended to be rendered by other programs before being read. Mark*down* can still be rendered into rich text -- more visually compelling documents -- while the simplicity maintains readability and clarifies document structure.  Additionally, markdown is a more compellingly [reproducible](https://en.wikipedia.org/wiki/Reproducibility) practice which yields quick report production and easy format transformations.

### Learn R Markdown in 20 seconds

Learning R Markdown is quick and painless.  Glance at [this summary example](https://en.wikipedia.org/wiki/Markdown#Example) and you've practically learned the whole spec.  You may have noticed I linked to a markdown example.  The good folks at [RStudio](//rstudio.com) have seen the  wisdom of markdown and incorporated the spec with minor tweaks to make R Markdown.  The few extra features of R Markdown are useful while the differences in the two "languages" are so similar that learning one is essentially learning the other.  Learn more [R Markdown](http://rmarkdown.rstudio.com/lesson-1.html) ([*cheatsheet*](https://www.rstudio.com/wp-content/uploads/2016/03/rmarkdown-cheatsheet-2.0.pdf)) and make your data science reports dynamic and reproducible.

Now you know.  In future blog posts I will describe  packages and report tools I've composed via R Markdown.  Xaringan slides is coming soon.  Stay tuned...

[^1]: [Lewis Carroll](https://www.goodreads.com/quotes/6305-begin-at-the-beginning-the-king-said-very-gravely-and)