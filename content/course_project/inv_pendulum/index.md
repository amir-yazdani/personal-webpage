+++
# Project title.
title = "Double-inverted pendulum"

# Date this page was created.
date = 2016-04-27T00:00:00

# Project summary to display on homepage.
summary = "Design, develop, and LQR control of a double-inverted pendulum on a cart"
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
url_pdf = "Jacob-Amir-Pendulum final report.pdf"
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
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
Course: ME EN 6240- Advanced Mechatronics

Control of the unstable inverted pendulum is a common research topic in the area of Dynamics and Controls. The project goal was to design, implement and test all of the mechanical, electrical, and software systems necessary to stabilize and control a double inverted pendulum. Mechanical design was completed in Solidworks and the manufactured parts were 3D printed. Electrical signal conditioning was accomplished through passive and active componentry and then integrated to a dsPIC microcontroller.

All final software was developed in MATLAB Simulink then converted to C code to be used in the dsPIC. The MATLAB development environment provides an easy to use system for future attempts at controlling the system. Swing up and control of a single inverted pendulum was successful though further controller tuning could yield a better system performance. 

The hardware and software for a double inverted pendulum
was successfully implemented though stable control was never
achieved. Further tuning of the LQR controller parameters would
yield a stable system.


{{< figure src="pend1.png" title="The double-inverted pendulum on a cart." >}}


{{< figure src="pend2.png" title="Simulation result of the step response for the double-inverted pendulum" >}}
