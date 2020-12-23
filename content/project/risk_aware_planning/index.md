+++
# Project title.
title = "Risk-Aware Planning for Patient Fall Prevention"

# Date this page was created.
date = 2020-10-02T00:00:00

# Project summary to display on homepage.
summary = "Risk-aware decision making to prevent high fall risk ambulation of patients"
# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Motion Planning", "HRI"]

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
  caption = "Simulation setup."

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
In order to assist the patient efficiently, we develop a risk-aware planning framework which finds the best manipulation plan that minimizes the fall risk probability with minimum robot effort.
We view the risk-aware planning problem from the perspective of probabilistic inference and solve it as a multi-objective optimization problem.
For the fall risk objective, we use a linear combination of expected value and CVaR to minimize the overall risk of fall while avoiding even low probabilities of high fall risks.
