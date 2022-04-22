---
title: Migrating from hugo-academic v.0.1x via blogdown upto blogdown v.1x & wowchemy/starter-hugo
author: John Little
date: '2022-04-20'
slug: Migrating from hugo-academic v.0.1x via blogdown upto blogdown v.1x & wowchemy/starter-hugo
categories:
  - hugo
  - blogdown
  - migration
tags: [Quarto, Netlify, web sites]
subtitle: ''
summary: 'I spent some time migrating and upgrading my old blogown/hugo site.  Now is a good time to upgrade.  Waiting longer may yield some benefit with the impending stable Quarto release, but now is a great time to migrate your Blogdown and Hugo-theme.'
authors: [admin]
lastmod: '2022-04-20T17:00:35-04:00'
featured: no
image:
  caption: ''
  focal_point: ''
  preview_only: no
projects: []
---

## Summary

I spent some time migrating and upgrading my old blogown/hugo site.  Now's a good time to upgrade.  Waiting longer may yield some benefit with the impending stable Quarto release, but now is a great time to migrate your Blogdown and Hugo-theme.


## Disclaimer

When I created this website I thought I might blog a bit more.  Not sure why I thought that, but that was my thought.  To be honest, if you're never gonna blog, maybe you want to use [Distill for R Markdown](https://rstudio.github.io/distill/).  But as much as I like distill (and I really do!), there's something slick about Hugo that I like even more.

### Hugo

For the uninitiated [Hugo](https://gohugo.io/) is a _static web site builder_ framework that allows nearly anyone to generate a website fairly quickly and easily.  There are some challenges of working in a [CLI](https://www.w3schools.com/whatis/whatis_cli.asp) world, but I believe it's a more stable environment.  If you don't use Hugo, you may be using a mouse-bound workflow to develop your website.  Nonetheless, I opine the Blogdown/Hugo way as an excellent reproducible workflow. 

To be Fair, when I started with Hugo and Blogdown (see below) in roughly 2017, both technologies were nascent and heading for the teen years.  I launched web sites and got them running stable.  Then I tried hard to wait out the teen years.  Those where some times.  Those teens years gave us hell.  But now the tools have progressed and come of age.  Now is good!

### Hosting

There are many ways to host your Hugo site.  I've found Hugo + netlify.com to be an excellent combination.  (Use RStudio to orchestrate your project as a GitHub Repo, configure Netlify with GitHub, and each git-push will serve up your edited changes.)  For at least the past five years I've used the free Netlify hosting tier.  I imagine this freemium will continue, but even if Netlify decides to stop hosting freely, I'm positive a competitor will jump in to offer an excellent alternative.  

### Blogdown

[Blogdown](https://pkgs.rstudio.com/blogdown/) is an R package developed through our RStudio friends.  It's an implementation of Hugo that makes it convenient to keep all your development and composition within the [RStudio IDE](https://www.rstudio.com/products/rstudio/download/).  This is a good thing.  

### Reproducibility

As I've said many times, the combination of R -- a data-first programming language -- plus the [Tidyverse](https://tidyverse.org) dialect, combined with the reproducible qualities of Markdown and version control are well considered.  These tools enable a workflow that overcomes the many many many barriers of a mouse-based workflow; one that is fraught with barriers to your publication and research legacy.  In short, if you want to have a simple and convenient way to save and show your work, it's time to move beyond the mouse.  Embrace version-control + Markdown as elements of your _Reproducible Workflows_.

### Wowchemy Hugo theme

One of the nice features of Hugo websites is that you can apply various themes to your content.  The Hugo-Academic theme was an early leader in helping academics create useful websites to promote publications, talks, and various aspects of an academic's life. That theme has now been superseded and branded as [wowchemy/starter-hugo-academic](https://github.com/wowchemy/starter-hugo-academic).  This theme remains well developed and useful; it _can be_ easy to work with. But it can also be a pain.  

Customize within the broad lanes that _starter-hugo-academic_ makes available.  Even though wowchemy and Hugo makes it possible to customized everything, wowchemy goes to great length to help you minimize your noodling and maximize  customization within a very convenient and attractive model that requires no HTML coding.  

My advice: try to keep yourself on track, stay within the lines, and keep the noodling to a minimum.  Focus on the customizing that wowchemy enables.  It enables a lot. You don't have to know anything about web development -- though it won't hurt.  (Actually, web skills may promote distraction.  Just try to stay focused.)

Fair warning, web development noodling can be hard and web development can be a time-sink.   

### Process / What I learned / Notes

Now is the time to migrate. The latest changes to Hugo, Blogdown, and the Webchemy/starter-hugo-academic make this an attractive time to migrate, upgrade, or start using this manner of web page authoring.  The following method worked for me.

1. Use RStudio to start a new project
1. Start that project in a new directory
1. Start that project as a blogdown website
1. Use the hugo theme `wowchemy/starter-hugo-academic`
1. Get comfortable with how the pieces fit together.  There is plenty of wowchemy and blogdown _get-started_ documentation
1. If you are migrating an old Hugo-Academic site, move things over on a case-by-case basis.  This may take some time; it may be somewhat fraught. But I found it's easier that trying to install new themes over the old site content.  Of course, my advice pertains to small and personal sites.  Big kids can figure out their own path.
1. Before you start, read this [Blogdown post](https://www.rstudio.com/blog/blogdown-v1.0/)
1. And you might consider waiting till Quarto's stable release, but I think now is a good time to jump.  Quarto will likely find a good audience and Quarto will likely document a clear migration paths.


### Quarto

If you're used to the R Markdown and RStudio world then you know some of the report rendering off-ramps and on-ramps can, occasionally, feel abrupt -- sort of make you feel like you just hit a gravel-road connector.  This is somewhat startling but rarely a problem.  Usually these bumps are easily traversed -- often I'm quickly back up to cruising speed. As near as I can tell, [Quarto](https://quarto.org/) is the report-render infrastructure improvement we've hoped for.  In my brief exploration Quarto brings consistency and solid documentation to the report rendering process, in much the same way that the Tidyverse brings consistency and documentation to R, and Tidymodels brings consistency and documentation to modeling and ML.  If anything, this makes it easier for the Python crowd to see the value of the RStudio ecosystem while still not requiring anyone to give up their favorite language -- I'm looking at you python-peeps.  

Honestly, R Markdown and the RStudio IDE is so much better as a development environment.  I don't _want_ to hate, but Jupyter, come back towards earth -- I'm thinking about an especially painful planetary report rendering workflow, but not limited to it.  Quarto is poised orbit around the sun rather than be a big blobby planet.  (I'm not talking about R v Python -- we can all get along. Deep breaths.) Quarto is icing on the cake.  Cake for everyone!!

### Conclusion

There are many moving pieces to report rending and web site development is simply one type of report.  Blogown, Hugo, and wowchemy have all made improvements to their offering.  All three work well together and now is a good time to migrate or get started.


