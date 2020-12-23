+++
# Project title.
title = "Mobile Manipulation Planning"

# Date this page was created.
date = 2019-03-27T00:00:00

# Project summary to display on homepage.
summary = "Optimal Manipulation Planning for a mobile robot using Learned Objects Dynamic Models"
# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Motion Planning"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references
#   `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides = ""


# Links (optional).
url_pdf = ""
url_slides = ""
url_video = ""
url_code = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
#   url_custom = [{icon_pack = "fab", icon="twitter", name="Follow", url = "https://twitter.com/georgecushen"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder.
[image]
  # Caption (optional)
  caption = "PAM robot delivering a walker"

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
In this project we introduce a patient assistant mobile (PAM) robot to monitor patient behavior and provide a cost-effective physical presence to continuously observe a patient and the environment to prevent falls.

Many common objects found inside hospital rooms and personal dwellings have legs (e.g. walkers, tables, chairs, equipment stands). For a mobile robot operating in such environments, safely maneuvering these objects without collision is essential. Since providing the robot with dynamic models of all possible legged objects that may exist in such environments is not feasible, autonomous learning of an approximate dynamic model for these objects would significantly improve manipulation planning. Thus, we have developed a probabilistic algorithm that learns pre-categorized object models using minimal force and motion interactions between the robot and object.

We account for multiple manipulation strategies by formulating the manipulation planning as a mixed-integer convex optimization problem. The proposed manipulation framework considers the hybrid control system comprised of i) choosing which leg to grasp, and ii) continuous applied forces to move the aid.
