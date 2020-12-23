+++
# Project title.
title = "Manipulation Planning of A Box Using A Mobile Robot"

# Date this page was created.
date = 2016-05-27T00:00:00

# Project summary to display on homepage.
summary = "Collision-Free push planning for manipulation of A box with a mobile robot"
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
url_pdf = "files/papers/motion_planning_project_report.pdf"
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

Mobility is one of the most important factors that contributes to quality of life. Each year, about 35% of individuals over age 65 experience one or more falls. Falls are the third leading cause of chronic disability worldwide6. In this project, we tried to address the concerns with home falls with a low-cost, intelligent mobile robot that will provide mobility aids, such as a walker, in the event that it determines that risk of fall is high.

As the project for Motion Planning course, a simplified version of the aforementioned bigger problem was defined in a simulation-based approach. In the proposed project, the problem includes the manipulation of a walker around an obstacle-filled area using a mobile robot from a start position to a goal position. For simulation studies, all objects will be projected to the 2D plane. The mobile robot is shows as a circle, the walker is shown as a box, and obstacles as shown as simple blue polygons. Several assumptions for the problem have been made:

* Only pushing has been used for manipulating the box.
* Start and goal position of the box and start position of the robot are known.
* Obstacles and their position are known.

The proposed approach to solve the above problem includes a high-level planner for push planning for the box and a lower level planner for motion planning of the robot. Based on what has been learned up to the point of proposal, a modified A* planning algorithm as a high-level planner in combination with RRT algorithm were proposed as the solution. The main contribution of this project is the development of a collision-free push planning algorithm for a box by a mobile robot which includes a higher-level A* planner and a lower level RRT planner. Simulation studies have been done in Python for different environments and with different start and goal positions for the robot and box. Results reveal the ability of the algorithm to do a collision-free manipulation for the box.


{{< figure src="pushplanning2.jpg" title="Simulation results on different environments. In left column, robot initial poses are yellow, box initial poses are red, box goal poses are green. In right column, robot path are yellow, box bath are green and visited nodes for box are red." >}}

{{< youtube SSRHkvtLvPM >}}
{{< youtube C7T5bCbeFek >}}
{{< youtube ua2OfplkcjE >}}
