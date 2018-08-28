+++
# Date this page was created.
date = "2018-08-28"

# Project title.
title = "Code Example:  geom_sf choropleth with coastline"

# Project summary to display on homepage.
summary = "This code example illustrates a choropleth made with ggplot::geom_sf()"

# Optional image to display on homepage (relative to `static/img/` folder).
image_preview = "ny_with_coast.png"

# Tags: can be used for filtering projects.
# Example: `tags = ["code","gis"]`
tags = ["code", "scraping"]

# Optional external URL for project (replaces project detail page).
# external_link = "/project/custom/twitterj/slides.html"

# Does the project detail page use math formatting?
math = false

# Optional featured image (relative to `static/img/` folder).
[header]
image = "headers/ny_with_coast_wide.png"
caption = "Population choropleth with coastline"

+++

&nbsp;

This code example adds a coastline overlay ontop of a population choropleth of population.  Census tracts extend over water and obscure the landform geography.  A good coastline is a great find.  See the GitHub [Repo showing a full code](https://github.com/libjohn/ben_g_nymap) treatment.


#### Date
2018-08-28

#### Example Code, Abbreviated

``` r
ggplot() +
  geom_sf(data = borroughs, aes(fill = pop)) +
  viridis::scale_fill_viridis(direction = -1) +
  geom_sf(data = coast, color = "black", fill = "black") +
  coord_sf(xlim = c(-73.7, -74.3), ylim = c(40.45, 40.95)) + 
  theme(panel.background = element_rect(fill = "transparent"), 
        panel.grid.major = element_line(color = "transparent"), 
        axis.text.x = element_blank(), 
        axis.text.y = element_blank(), 
        axis.ticks = element_blank())
```

