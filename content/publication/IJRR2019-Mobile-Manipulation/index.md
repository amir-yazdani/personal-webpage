+++
title = "A Model Predictive Approach for Online Mobile Manipulation of Nonholonomic Objects using Learned Dynamics"
date = 2019-12-20T00:00:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Roya Sabbagh Novin", "Amir Yazdani", "Andrew Merryweather", "Tucker Hermans"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference paper
# 2 = Journal article
# 3 = Manuscript
# 4 = Report
# 5 = Book
# 6 = Book section
publication_types = ["2"]

# Publication name and optional abbreviated version.
publication = "Sybmitted to *The International Journal of Robotics Research (IJRR)*"
publication_short = "In *IJRR 2019*"

# Abstract and optional shortened version.
abstract = "A particular type of assistive robots designed for physical interaction with objects could play an important role assisting with mobility and fall prevention in healthcare facilities. Autonomous mobile manipulation presents a hurdle prior to safely being able to utilize robots in real life applications such as healthcare and warehouse robots. In this article, we introduce a mobile manipulation framework based on model predictive control using learned dynamics models of objects. We focus on the specific problem of manipulating legged objects such as those commonly found in healthcare environments and personal dwellings (e.g. walkers, tables, chairs, equipment stands). We describe a probabilistic method for autonomous learning of an approximate dynamics model for these objects. In this method, we learn pre-categorized object models by using a small dataset consisting of force and motion interactions between the robot and object. In addition, we account for multiple manipulation strategies by formulating the manipulation planning as a mixed-integer convex optimization problem. The proposed manipulation framework considers the hybrid control system comprised of i) choosing which leg to grasp, and ii) continuous applied forces to move the object. We propose a manipulation planning algorithm based on model predictive control to compensate for modeling errors and find an optimal path to manipulate the object from one configuration to another. We show results for several objects with different wheel configurations. Simulation and physical experiments show that the obtained dynamics models are sufficiently accurate for safe and collision-free manipulation. When combined with the proposed manipulation planning algorithm, the robot can successfully move the object to a desired pose while avoiding collision."
abstract_short = ""

# Is this a selected publication? (true/false)
selected = false

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects = ["pam"]

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references
#   `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides = ""

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []

# Links (optional).
url_pdf = ""
url_preprint = "https://arxiv.org/abs/1912.09565"
url_code = "https://www.google.com/url?q=https%3A%2F%2Fgithub.com%2FRoyaSabbagh%2Fmanipulation_planning&sa=D&sntz=1&usg=AFQjCNHjVJGbouN-_WUiahRHmnaMdi_QtA"
url_custom= [{name = "website", url = "https://sites.google.com/view/mobile-manipulation-planning"}]
url_project = "pam"
url_slides = ""
url_video = "https://youtu.be/mw9qBr66bVQ"
url_poster = ""
url_source = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
# url_custom = [{name = "Custom Link", url = "http://example.org"}]

# Digital Object Identifier (DOI)
doi = ""

# Does this page contain LaTeX math? (true/false)
math = true

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
[image]
  # Caption (optional)
  caption = "Mobile manipulation to deliver a walker to a patient"

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""
+++

{{< figure src="model_comparison.PNG" title="Final displacement errors with and without feedback." >}}


{{< figure src="sim_results.PNG" title="The final position and orientation errors in simulation experiments for all objects through all tasks." >}}


{{< figure src="real_results.PNG" title="Physical experiments results from two tasks." >}}
