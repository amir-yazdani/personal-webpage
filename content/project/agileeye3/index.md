+++
# Project title.
title = "Cheshm-e-Chabok 3-DOF Parallel Robot"

# Date this page was created.
date = 2013-04-27T00:00:00

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
  caption = "CAD model of Cheshm-e-Chabok 3-DOF spherical parallel robot"

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
This project includes design, kinematics and dynamics analysis of a 3-DOF Cartesian robot inspired by the AgileEye3 parallel robot.
I designed the robot and was the key member to do the kinematics and dynamics analysis using the Euler-Lagrangian method and also control of the device using computed-torque control method. This robot also provides fast 3-DOF spherical motion. We used this robot for tracking and also for simulating the motion of a human neck for a human head-like robot.

{{< figure src="agile3-11.jpg" title="The concept of dividing the limbs from the EE in Cheshm-e-Chabok 3-DOF parallel robot." >}}
