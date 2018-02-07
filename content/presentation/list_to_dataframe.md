+++
# Date this page was created.
date = "2018-02-06"

# Project title.
title = "Code Example:  List to Data Frame"

# Project summary to display on homepage.
summary = "This code example illustrates `purrr` and `repurrrsive`"

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "lego-rstats_014-smaller.jpg"

# Tags: can be used for filtering projects.
# Example: `tags = ["presentation","code"]`
tags = ["code", "scraping"]

# Optional external URL for project (replaces project detail page).
# external_link = "/project/custom/twitterj/slides.html"

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = "lego-rstats_039.jpg"
caption = "Jenny Bryan's Lego-themed glamour shots illustrating R Data Structures"

+++

&nbsp;

The following code example illustrates how to take a list column inside a data frame and wrangle it -- making it easier to analyze. For more information, see the [HTML output](/code_example/json_to_dataframe_unnest.nb.html). for the R Notebook, [list_to_dataframe.Rmd](https://github.com/libjohn/dataframe_with_list).


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

#### References

This example comes from a Jenny Bryan Workshop, *[What they forgot to teach you about R](https://github.com/jennybc/what-they-forgot)*.  Similar examples can be found in Bryan's [Purrr tutorial](https://jennybc.github.io/purrr-tutorial/).  Specifically...

- [List as variables in a data frame](https://jennybc.github.io/purrr-tutorial/ls13_list-columns.html#lists_as_variables_in_a_data_frame)
- [Food Markets in New York](https://jennybc.github.io/purrr-tutorial/ex26_ny-food-market-json.html)   

#### Image Credit:

https://github.com/jennybc/lego-rstats