---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
# this was copied from https://github.com/mmistakes/minimal-mistakes/blob/master/docs/_pages/home.md
<!-- layout: home -->
<!-- author_profile: true -->
layout: splash
permalink: /
hidden: true
header:
  overlay_color: "#5e616c"
  overlay_image: /assets/images/home.jpg
excerpt: >
  A personal blog containing my notes from different fields I've learned.<br />
feature_row:
  - image_path: /assets/images/ml.jpg
    alt: "customizable"
    title: "Machine Learning"
    excerpt: "Everything about machine learning"
    url: "/ml/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
  - image_path: /assets/images/misc.jpg
    alt: "fully responsive"
    title: "Miscellaneous"
    excerpt: "Everything about everything else."
    url: "/misc/"
    btn_class: "btn--primary"
    btn_label: "Learn more"
---

{% include feature_row %}
