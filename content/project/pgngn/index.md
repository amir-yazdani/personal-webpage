+++
# Project title.
title = "Progressive Growing Natural Gas Network (PGNGN)"

# Date this page was created.
date = 2014-04-27T00:00:00

# Project summary to display on homepage.
summary = "PGNGN algorithm for determining singularity-free workspace of parallel robots"
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
  caption = "Singularity-free workspace of a parallel robot using PGNGN."

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

This project, proposes a new extension of the Growing Neural Gas Network, called the Progressive Growing Neural Gas Network (PGNGN), for the application of kinematic investigation of parallel mechanisms, with more emphasis on the singularity-free workspace determination. In fact, PGNGN leads to a general approach in order to obtain the topology of the workspace. In this algorithm, the network starts to grow by taking into account new data points close to its border neurons by resorting to the so-called boundary data generation procedure.

 By considering singularity loci expression, the separated parts are detected and each part will pursue learning, adding units and connections, until a given performance criterion will be reached. Finally, after finding cavities, if any exists, the maximal circle for each part of the workspace is found. A graphical user interface (GUI) is developed providing the users with easy access to the important parameters in which the singularity-free workspace of three planar three-degree-of-freedom (3-DOF) parallel mechanisms are investigated in which two of them, namely, 3-RRR and 3-PRR parallel mechanisms, are among the most complicated parallel mechanisms due to their highly nonlinear and complicated singularity loci expressions. Results reveal the applicability and reliability of the proposed PGNGN-based approach for obtaining the singularity-free workspace of planar parallel mechanisms.

{{< figure src="pgngn11.jpg" title="maximal circle singularity-free workspace determination of 3-PRR planar parallel mechanism for its (þþþ) working mode." >}}
