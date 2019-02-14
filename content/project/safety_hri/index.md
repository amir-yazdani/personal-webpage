+++
# Project title.
title = "Safe Motion Planning in Shared Autonomy"

# Date this page was created.
date = 2016-03-27T00:00:00

# Project summary to display on homepage.
summary = "Safe and human-aware optimal and fault tolerant motion planning in human-robot intearction"
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
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++
As human and robot collaboration become more intimate, and more intelligent robots are being used in both healthcare and manufacturing environments, the safety of humans working closely with companion or co-robots is becoming a challenging issue. As a result, there is a great need for developing improved control algorithms and better guidelines to allow humans and robots to safely work together in a synergistic fashion. The nature of human variability requires the robot to be able to learn and adapt to these changes while maintaining safety in the presence of an often unpredictable human worker.

In this project, we use the algorithm we developed previously for collision-free and fault-tolerant motion planniong of serial robots and we add safety features including minimum seperation distance and relative velocity of robot and the human arm. We are also adding the motion prediction of human during normal pick and place task to improve the performanc of the motion planning algorithm in respect of both the safety and the productivity.

{{< figure src="safety_hri1.png" title="The shared autonomy scenario including the fauilure in the robot's joints." >}}
