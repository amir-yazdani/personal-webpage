+++
# Project title.
title = "A Fully-Decoupled Cartesian 3-PRRR Parallel Robot"

# Date this page was created.
date = 2012-04-27T00:00:00

# Project summary to display on homepage.
summary = "Design, develop, kinematic and dynamic analysis of a decoupled 3-DOF parallel robot"
# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Parallel Robots"]

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
  caption = "The 3-DOF decoupled parallel robot"

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
This project includes design, develop, kinematics and dynamics analysis of a 3-DOF Cartesian robot inspired by the Tripteron robot.
I optimally designed the mechanism to maximize the singularity-free workspace using geometry approaches using SolidWorks considering all joint limits and mechanical interface of joints. Later, I was involved with the optimal collision-free path planning of this robot. The accuracy and working speed due to its parallel structure, features this robot to be used for material handling, fast pick and place tasks, and large-scale 3D printing.

{{< figure src="tripteron5.jpg" title="CAD model of the 3-DOF decoupled parallel robot." >}}

{{< figure src="tripteron3.jpg" title="Singularity-free workspace of the 3-DOF decoupled parallel robot." >}}
