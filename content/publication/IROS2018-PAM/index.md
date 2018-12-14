+++
title = "Dynamics Model Learning and Manipulation Planning for Objects in Hospitals Using a Patient Assistant Mobile (PAM) Robot"
date = 2018-09-01T00:00:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Roya Sabbagh Novin", "Amir Yazdani", "Tucker Hermans", "Andrew Merryweather"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference paper
# 2 = Journal article
# 3 = Manuscript
# 4 = Report
# 5 = Book
# 6 = Book section
publication_types = ["1"]

# Publication name and optional abbreviated version.
publication = "In *IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)*, 2018."
publication_short = "In *IROS 2018*"

# Abstract and optional shortened version.
abstract = "One of the most concerning and costly problems in hospitals is patients falls. We address this problem by introducing PAM, a patient assistant mobile robot, that maneuvers mobility aids to assist with fall prevention. Common objects found inside hospitals include objects with legs (i.e. walkers, tables, chairs, equipment stands). For a mobile robot operating in such environments, safely maneuvering these objects without collision is essential. Since providing the  robot  with  dynamic models of all possible  legged objects  that  may  exist  in  such environments  is  not  feasible,  autonomous  learning  of  an approximate dynamic model for these objects would significantly improve  manipulation  planning.  We  describe  a  probabilistic method  to  do  this  by  fitting  pre categorized  object  models learned  from  minimal  force  and  motion  interactions  with  an object. In addition,   we   account   for multiple   manipulation strategies,  which  requires  a  hybrid  control  system  comprised of discrete grasps on legs and continuous applied forces. To do this,  we  use  a  simple  one-wheel  point-mass  model.  A  hybrid MPC-based manipulation planning algorithm was developed to compensate for modeling errors. While the proposed algorithm applies  to  a  broad  range  of  legged  objects,  we  only show results   for   the   case   of   a   2-wheel,   4-legged   walker   in   this paper. Simulation and experimental tests show that the obtained dynamic model is sufficiently accurate for safe and collision-free manipulation. When combined with the proposed manipulation planning algorithm, the robot can successfully move the object to  a  desired  position  without  collision."
abstract_short = ""

# Is this a selected publication? (true/false)
selected = false

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references 
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects = []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references 
#   `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides = ""

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []

# Links (optional).
url_pdf = "https://robot-learning.cs.utah.edu/_media/project/sabbagh-iros-2018-dynamics-learning.pdf"
url_preprint = ""
url_code = ""
url_dataset = ""
url_project = ""
url_slides = ""
url_video = ""
url_poster = ""
url_source = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
# url_custom = [{name = "Custom Link", url = "http://example.org"}]

# Digital Object Identifier (DOI)
doi = ""

# Does this page contain LaTeX math? (true/false)
math = true

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
[image]
  # Caption (optional)
  caption = "PAM mobile robot"

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""
+++


