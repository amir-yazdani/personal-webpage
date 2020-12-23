+++
title = "Estimating Human Teleoperator Posture Using Only a Haptic-Input Device"
date = 2020-02-24T00:00:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Amir Yazdnai", "Roya Sabbagh Novin", "Andrew Merryweather", "Tucker Hermans"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference paper
# 2 = Journal article
# 3 = Manuscript
# 4 = Report
# 5 = Book
# 6 = Book section
publication_types = ["2"]

# Publication name and optional abbreviated version.
publication = "Submitted to *IEEE Robotics and Automation Letter* and *IROS 2020*"
publication_short = "In *RA-L* and *IROS 2020*"

# Abstract and optional shortened version.
abstract = "Ergonomic analysis of human posture plays a vital role in understanding long-term, work-related safety and health. Current analysis is often hindered due to difficulties in estimating human posture. We introduce a new approach to the problem of human posture estimation for teleoperation tasks which relies solely on a haptic-input device for generating observations. We model the human upper body using a redundant, partially observable dynamical system. This allows us to naturally formulate the estimation problem as probabilistic inference and solve the inference problem using a standard particle filter. We show that our approach accurately estimates the posture of different human users without knowing their specific segment lengths. We evaluate our posture estimation approach from a haptic-input device by comparing it with the human posture estimates from a commercial motion capture system. Our results show that the proposed algorithm successfully estimates human posture based only on the trajectory of the haptic-input device stylus. We additionally show that ergonomic risk estimates derived from our posture estimation approach are comparable to those estimates from gold-standard, motion-capture based pose estimates."
abstract_short = ""

# Is this a selected publication? (true/false)
selected = true

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects = ["pose_estimation"]

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
url_pdf = ""
url_preprint = "https://arxiv.org/abs/2002.10586"
url_code = ""
url_project = "pose_estimation"
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
  caption = "Mobile manipulation to deliver a walker to a patient"

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = ""
+++
