+++
# Project title.
title = "Mobile Robot Visual Localization and 3D Map Generation"

# Date this page was created.
date = 2016-05-27T00:00:00

# Project summary to display on homepage.
summary = "Visual odometry using monocular camera and Kinect sensor for outdoor and indoor localization and map generation of a mobile robot"
# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["Other"]

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
url_pdf = "files/papers/cv_project_localization_and_map_generation.pdf"
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

In this project, we will implement a Visual Odometry method on a Roomba iCreate 2 which is equipped with a Microsoft Kinect RGB-D sensor for localization and map generation. Although the mobile robot is moving on a 2D plane (ground), the localization and map generation algorithms are for 3D environments, so the final results are in 3D. At the end, we will evaluate our approach by comparing resulted localization with results from robot odometry, LIDAR sensor localization, or GPS data. Finally, we made a ROS package which includes different nodes for various parts of the algorithm.


{{< figure src="mobile1.jpg" title="Indoor localization using graph-based SLAM with Kinect, LIDAR, and robot odometry." >}}
