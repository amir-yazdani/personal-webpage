+++
# Project title.
title = "Fault-Tolerant Motion Planning"

# Date this page was created.
date = 2015-06-27T00:00:00

# Project summary to display on homepage.
summary = "Fault-tolerant and collision-free motion planning of serial robots"
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
  caption = "TaArm 4-DOF redundant planar serial robot."

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

In this project we focused on making the motion planning of the robots fault-tolerant. We started with the simple Pseudo inverse approach to making the joint trajectory planning of planar redundant serial robots the fault tolerant. We made a 4-DOF planar robot (TaArm) to do the experimental studies to show the performance of the proposed method.

{{< figure src="fault1.jpg" title="End-effector’s linear velocity of the manipulator. The failure occurs at tf = 15s and the simulation time is 20s." >}}

The Pseudo inverse method has some limitations so we mixed the failure-tolerant problem with optimal motion planning problem and provided an algorithm that solves both at the same time. The new algorithm is based on convex optimization, MPC, and quadratic programming and prevents collision between obstacles/human and robot by real-time re-planning and minimizes harmful velocity jumps when a failure occurs in robot actuators while the robot completes the desired task. We modeled the joint failure into the optimization problem and solved task completion problem, minimizing velocity jump due to failure problem and optimal collision-free motion planning problem at the same time.

{{< figure src="fault2.jpg" title="Angular velocity of the 1st joint. The failure occurs at t=14s in the 3rd joint and the whole simulation time is 20s." >}}
