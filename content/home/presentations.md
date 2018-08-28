+++
# Presentation widget is based on the project widget.
# There are several files that make this work.  
# Customization is primarily done in the 'static' 
# and 'layouts' directories.
# Other files that make this work:
# content/presentation
# layouts/presentatin/
# layouts/presentation/widgets/presentations.html  #note plural
# inside this file: {{ range $project := where $.Data.Pages "Type" "presentation" }}
# 
# Note: this widget will only display if `content/presentation/` contains presentations.

date = "2016-04-20T00:00:00"
draft = false

title = "Presentations"
subtitle = ""
widget = "presentations"

# Order that this section will appear in.
weight = 30

# View.
# Customize how projects are displayed.
# Legend: 0 = list, 1 = cards.
view = 1

# Filter toolbar.
# Add or remove as many filters (`[[filter]]` instances) as you like.
# Use "*" tag to show all projects or an existing tag prefixed with "." to filter by specific tag.
# To remove toolbar, delete/comment all instances of `[[filter]]` below.
[[filter]]
  name = "All"
  tag = "*"
  
[[filter]]
  name = "API"
  tag = ".api"
  
[[filter]]
  name = "Code Example"
  tag = ".code"  

[[filter]]
  name = "CSS"
  tag = ".css"
  
[[filter]]
  name = "Dashboards"
  tag = ".dashboards"
  
[[filter]]
  name = "DSVIL"
  tag = ".dsvil"
  
[[filter]]
  name = "GIS"
  tag = ".gis"

[[filter]]
  name = "JSON"
  tag = ".json"
  
[[filter]]
  name = "OpenRefine"
  tag = ".openrefine"

[[filter]]
  name = "Parsing"
  tag = ".parsing"

[[filter]]
  name = "Rfun"
  tag = ".rfun"
  
[[filter]]
  name = "Text Mining"
  tag = ".mining"
  
[[filter]]
  name = "Twitter"
  tag = ".twitter"
  
[[filter]]
  name = "Visualization"
  tag = ".visualization"

[[filter]]
  name = "Web Scraping"
  tag = ".scraping"
+++

