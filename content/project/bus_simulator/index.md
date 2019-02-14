+++
# Project title.
title = "Bus Driving Simuator"

# Date this page was created.
date = 2010-04-27T00:00:00

# Project summary to display on homepage.
summary = "Design a novel 4-DOF moving platform for bus driving simulators"
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
  caption = "Nasir bus driving simulator."

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

This project includes the design and development of three types of urban bus driving simulators at Virtual Reality Laboratory at Khajeh Nasir Toosi University of Technology in Iran under contract with Tehran Bus Company. I designed a novel 4-DOF serial-parallel robot to be the base platform of driving simulators. It is a hybrid mechanism benefiting from the advantages of both serial and parallel mechanisms. The main challenge in this project was to design a mechanism structure based on the required motion for the driving simulators to provide the user with the most realistic feeling of driving. The final design is a 2-PSS+1U mechanism and the robot provides surge, pitch, roll, and heave motions. The fixed base is connected to the moving platform by two limbs with PSS as the kinematic arrangement. A fixed passive leg is connected by a U joint to the moving platform which removes four DOFs from the moving platform, resulting in a two DOF parallel mechanism. Except for the fixed limb, each leg is connected to the base and moving platform with spherical joints. The passive limb is connected to the moving platform with a universal joint.

Inverse kinematics of the mechanism is also solved to find four different working modes of the mechanism to map the required motion of moving platform into actuators. Forward kinematics of the system is also solved using elimination and resultant techniques. The design of the mechanism also includes determining singularities of the robot and its singularity-free workspace and it is done by a CAD software and interval analysis approach. Interval Analysis method has the advantages of being able to deal with almost any constraint and any number of DOF and is proved to be efficient in computing the most difficult case of 6-dimensional workspaces. To find the Jacobian matrix of the mechanism, first, the kinematical screw system (KSS) of all the limbs constituting the mechanism is obtained. Then, the constraint imposed on the moving platform by the limbs are found which can be done by applying the concept of the reciprocal screw system to the KSS of all the limbs. Finally, each row of the Jacobian matrix is computed by resorting again to the concept of the reciprocal screw and obtain the corresponding KSS by locking the actuators.
{{< figure src="simulator1.jpg" title="CAD model of the 4-DOF serial-parallel mechanism for bus dribing simulator." >}}
