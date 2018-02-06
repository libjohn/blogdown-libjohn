+++
# Date this page was created.
date = "2018-02-06"

# Project title.
title = "Code Example:  List to Data Frame"

# Project summary to display on homepage.
summary = "This code example illustrates `purrr` and `repurrrsive`"

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = ""

# Tags: can be used for filtering projects.
# Example: `tags = ["presentation","code"]`
tags = ["code"]

# Optional external URL for project (replaces project detail page).
# external_link = "/project/custom/twitterj/slides.html"

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = ""
caption = "Duke's Tableau Day.  July 26, 2017"

+++

&nbsp;

The code example illustrates how to take a list column in a dataframe and wrangle it, thus making it easier to analyze.  See the [HTML output](/code_example/json_to_dataframe_unnest.nb.html) is for the R Notebook, [list_to_dataframe.Rmd](https://github.com/libjohn/dataframe_with_list) and 

From a Jenny Bryan Workshop but similar to [Purrr tutorial](https://jennybc.github.io/purrr-tutorial/):  [Food Markets in New York](https://jennybc.github.io/purrr-tutorial/ex26_ny-food-market-json.html)   



#### Date
2018-02-06

#### Example Code, Abbreviated

```
library(tidyverse)
library(repurrrsive)

dataframe_list <- tibble(
  name = map_chr(got_chars, "name"),
  title = map(got_chars, "titles")
)

dataframe_list %>% 
  mutate(n_titles = map_int(title, length)) %>% 
  filter(n_titles > 1) %>% 
  select(name, title) %>% 
  unnest()
```