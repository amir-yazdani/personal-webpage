+++
# Project title.
title = "The Search for Twitter Spam Bots"

# Date this page was created.
date = 2017-12-20T00:00:00

# Project summary to display on homepage.
summary = "Find Twitter spam bots using machile learning algorithms"
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
url_pdf = "files/papers/Amir Yazdani- search-twitter-bots-report.pdf"
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


This project includes finding spammer and bot accounts in Twitter using machine learning techniques. The dataset is provided at the [Kaggle website](https://www.kaggle.com/c/uofu-ml-fall-2017) and I have compared the performance of the following algorithms:

* ID3 Decision Tree
* CART: Classification and Regression Trees
* Gaussian Naive Bayes
* SVM
* Logistic Regression
* SVM + CART
* Bagged Forest CART

The results show that Bagged Forest Cart algorithm and CART has the best accuracy on finding spam account.





{{< figure src="twitter_table.png" title="" >}}


{{< figure src="twitter_accuracy.png" title="Accuracy of different algorithms." >}}
