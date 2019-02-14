+++
# Project title.
title = "Collision-Free Optimal Path Planning"

# Date this page was created.
date = 2015-04-27T00:00:00

# Project summary to display on homepage.
summary = "Collision-Free optimal path planning of serial robots using MPC and convex optimization"
# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
# tags = ["Pose estimation", "particle filter"]

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
  caption = "TaArm 4-DOF redundant planar serial robot."

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

This project focuses on the optimal path planning of redundant planar serial robots, while avoiding obstacles within its workspace. A synergy-based algorithm between convex optimization, disjunctive programming and receding horizon is employed to the end of achieving advantages such as finding the global optimum solution and low computational time.

This algorithm can handle both static and dynamic obstacles due to its replanning scheme. It has been implemented on redundant serial robots, parallel robots, mobile robots and a group of mobile robots.

{{< figure src="mpc1.jpg" title="Simulation results of minimum time (left) and minimum path (right) optimal path planning with dynamic obstacles." >}}

{{< figure src="mpc23.jpg" title="Simulation results of optimal path planning on thre Tripteron parallel robot." >}}
