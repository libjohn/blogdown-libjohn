# Widget Mirroring

I attempted to change the URL (relative path) of `/publication` to `/workshop` but was **unsuccessful**.  

The following actions were attempted to enable index.html#workshop

## Experimental -- Publications to Workshops

Note:  This approach should be a more sustainable way to accomplish using a different URL for a particular widget.  I want to use the url `/workshop` instead of `/publication`.  At the moment is does not appear to work completely.  

1. Add to config.toml *before* `[params]` settings

```
[permalinks]
    publication = "/workshop/:slug"
```

2. alter the menu link in the config.toml

```
[[menu.main]]
  name = "Workshops"
  url = "#workshops"
  weight = 2`

```

3. Update `title` in the corresponding markdown file inside `content/home` (e.g. `workshops.md` based on `publications_selected.md`)

```
title = "Workshops"
subtitle = ""
widget = "publications_selected"
```

### Template files that might/may affect this goal

- ~\themes\hugo-academic\layouts\publicaton\single.html

    - ~\layouts\workshop\single.html

- ~ \themes\hugo-academic\layouts\partials\widgets\publications.html

    - ~\layouts\partials\widgets\workshops.html


- ~\...\publications_selected.html

    - ~\themes\hugo-academic\layouts\partials\publication_li_detailed.html
    - ~\...\publication_li_simple.html
    - ~\...\publication_links.html

- content/home/workshops.md
- content/home/workshops_selected.md


