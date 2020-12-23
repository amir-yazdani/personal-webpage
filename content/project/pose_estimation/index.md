+++
# Project title.
title = "Human Posture Estimation in Teleoperation"

# Date this page was created.
date = 2019-04-27T00:00:00

# Project summary to display on homepage.
summary = "Human posture estimation from a haptic device based on a partially-observable dynamic model"
# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["HRI"]

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
  caption = "Visualizing particles from human model to estimate the posture"

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
Human posture estimation has been a challenging research problem and many solutions has been suggested for different applications. Mainly, marker-based motion capture system and markerless camera-bases systems are the most common methods to estimate human posture. Marker-based solutions are usually more accurate however they require a long preparation time for setting up markers and calibration of MoCap systems. Markerless approaches are more convenient since they does not requires attaching markers on human body. Both of those methods are based on using cameras and have many limitation in real applications.
with the recent developments in physical human-robot interaction, estimating human posture is a demanding task specially in ergonomics and safety analysis, and adaption of robot motion based on human posture and motion.
In this project we propose a novel method to estimate human posture in teleoperation. We believe that in physical interaction between human and the robot, only knowing the robot's trajectory is adequate to estimate the human's posture. We model the problem as a partially-observable dynamic model and use filtering and smoothing approaches to solve the problem.
