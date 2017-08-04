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
summary = "R Markdown is the backbone of dynamic documents, literate data science, and reproducibility in R."


# Optional featured image (relative to `static/img/` folder).  
[header]
image = "headers/RMarkdownFlow.png"
caption = "Image credit: [**R Markdown by RStudio**](http://rmarkdown.rstudio.com/authoring_quick_tour.html)"
+++


## R Markdown is Awesome

*R Markdown is Awwwwwesoommmmmme*.  There, I said it. See, I have this niffty [new website](/) and it's produced via Blog*down* and **composed in R Markdown**.  To feed the blog section I plan on writing occassional posts such as this one.  But where do I start? (“Begin at the beginning," the King said, very gravely[^1]) ...  Well, these days I'm using R, a lot.  So initially, I was going to lead the blog with a post about [Xaringan slides](https://slides.yihui.name/xaringan/) -- another R Mark*down* option.  Then I realized I need to lead with R Markdown, because cool things enabled via RStudio are enhanced through R Markdown.  I'll come back to Xaringan slides another day.

### Why use R Markdown

R Markdown is easy to learn and easy to use.  When used with RStudio, R Markdown will enable report derivitives while the content remains readable and reproducible.  It's a benevolent cycle:  write a document once in R Markdown, derive reports with minimal effort, maintain the whole project with readable source material.  Or even better compose code in a [*literate programming*](https://en.wikipedia.org/wiki/Literate_programming) style, then generate your reports from your code.  For example, R Markdown can be used to create reports in the following formats:  slides, journal articles, PDF, Word files, web pages, web dashboards, web sites, dynamic quizes.

![](RMarkdownOutputFormats.png)

### What is R Markdown

R Markdown is a flavor of Markdown.  Markdown is a light-weight "language" used to add structure to text.  The mark*down* goal is to simplify mark*up* languages. The resulting simplicity means the content is less cluttered and easier to read. Easier because mark*up* languages are intended to be rendered by other programs before being read. Mark*down* can still be rendered into rich text -- more visually compelling documents -- while the simplicity maintains readability and clarifies document structure.  Additionally, markdown is a more compellingly [reproducible](https://en.wikipedia.org/wiki/Reproducibility) practice which yields quick report production and easy transformations into a variety of report formats.

### R Markdown v Markdown

All you need to learn is R Markdown a [glance at this summary example](https://en.wikipedia.org/wiki/Markdown#Example) -- quick and painless.  The good folks at RStudio have seen the markdown wisdom and incorporated the basics with minor tweaks.  You may have noticed I linked to a markdown example.  There are a few more featuers of R Markdown but the two "languages" are so similar that learning one is essentially learning the other.  Then learn more [R Markdown](http://rmarkdown.rstudio.com/authoring_quick_tour.html) to begin making your data science reports dyanmic and reproducible.

Now you know.  In future blog posts I plan to describe some of the other report tools I've composed via R Markdown.  Xaringan slides is coming soon.  Stay tuned...

[^1]: [Lewis Carroll](https://www.goodreads.com/quotes/6305-begin-at-the-beginning-the-king-said-very-gravely-and)