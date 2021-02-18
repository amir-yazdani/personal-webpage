+++
title = "Human Posture Estimation and Ergonomics Analysis Solely from the Robot in Physical Human-Robot Interaction"
date = 2019-04-10T00:00:00  # Schedule page publish date.
draft = false

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
time_start = 2019-04-18T14:00:00
time_end = 2019-04-18T14:15:00
all_day = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = []

# Abstract and optional shortened version.
abstract = "Ergonomic analysis of human posture plays a vital role in long-term, work-related safety and health. Since application of physical human-robot interaction (HRI) such as telesurgery and telemanipulation is becoming more prevalent we must consider the important problem of ensuring comfort and ergonomics of the operator in order to reduce the risk of musculoskeletal disorders, improve efficiency, and reduce error over long periods of work. Motivated by this problem, we envision an autonomous solution to improve ergonomics and worker safety in telemanipulation that includes three main steps: (1) estimating the human operator’s posture, (2) analysing the ergonomics and injury risk of the estimated posture, and (3) providing feedback from the robot to the human user to encourage moving toward a better posture. Current methods for human posture estimation in the literature, including marker-based and markerless posture estimations, are limited in many ways. Both of these approaches rely on vision systems which might be infeasible to set up in real workplaces. In this presentation, we focus on the first two problems and suggest a new approach to estimate posture of the human upper body in using only data observed from the robot and analyze the ergonomics of the posture. The main feature of telemanipulation that distinguishes it from other applications of posture estimation is the physical attachment of the human body to the master robot in one or more points. We believe that we can use this feature to estimate human posture without using any additional sensors other than the robot. We model the human upper body using a redundant, partially observable dynamic system. This allows us to naturally formulate the estimation problem as probabilistic inference and solve the inference problem using a standard particle filter. We formalize this as a probabilistic inference problem where, we measure the robot’s stylus trajectory (including pose and velocity) as the observation and infer the unobserved human posture (joint angles and angular velocities). We encode human factors and biomechanics knowledge into our partially observable dynamics model. We use anthropometry models to estimate the segment lengths of the human body and impose limits on joint angles. We incorporate multiple observations over time enabling us to perform inference using a standard particle filter. We evaluate our approach using simulation and human-subject experiments and compare it with the human posture estimations from a commercial motion capture system and an off-the-shelf depth-based markerless posture-estimation algorithm. We use RULA assessment tool to analyze the ergonomics of the task based on the estimated posture. In simulation, as expected, the model with full measurement has the lowest RMS error across all the experiment tasks. As the complexity of task increases, the effect of measurements becomes more pronounced. However, the highest RMS error achieved using the “no-measurement model” remains less than 10 deg. We see that the estimated joint angles track the ground truth posture relatively close. However, due to redundancy of the human model, we can see noticeable errors in some joints, even though the hand estimate tracks the stylus well. In human subject test, it is obvious that markerless posture estimation using Kinect V2 has a poor performance in comparison with motion capture and particle filter algorithm. Although the markerless algorithm could successfully track a human standing in open areas, it was unable to track the human well while sitting behind the desk and working with the robot. The results from the motion capture system were also sometimes wrong or jumpy in some tasks, especially for the wrist joint. Overall, the posture estimated from our approach and from motion capture system generally agree with an average deviation of around (17 deg).  The RULA score we provide also agrees with the score given by ergonomists. In this presentation, we addressed a new problem in physical HRI: human posture estimation from the robot without any additional sensors and automatic ergonomic analysis of the estimated posture. We define the problem as a partially observable dynamical system and use a particle filter to estimate posture of a 10-DOF model of the human upper body. The proposed approach can fit different populations of users with different body segment lengths and can be easily implemented in different applications."

# Name of event and optional event URL.
event = "National Occupational Injury Research Symposium (NOIRS) 2018"
event_url = "https://www.cdc.gov/niosh/noirs/2018/default.html"

# Location of event.
location = "Salt Lake City, UT"

# Is this a featured talk? (true/false)
featured = false

# Projects (optional).
#   Associate this talk with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects = ["pose_estimation"]

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []

# Slides (optional).
#   Associate this talk with Markdown slides.
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

# Does the content use math formatting?
math = true

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
[image]
  # Caption (optional)
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Right"
+++
