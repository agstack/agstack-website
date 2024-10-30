---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: splash
header:
  overlay_color: "#fff"
  overlay_filter: "0.5"
  overlay_image: /assets/img/arial-fields.jpg
  actions:
    - label: "Join AgStack"
      url: "/membership"
  #caption:
excerpt: "The AgStack Foundation supports global agriculture through the creation, maintenance, and enhancement of open digital infrastructure."
intro: 
  - excerpt: '<p>Digital technology holds tremendous promis to advance agriculture at the scale and speed needed to make a difference to our world.</p><p>Globally accessible, open source, digital infrastructure is the solution needed to achieve the necessary scale and speed.</p>'
explore: 
    - excerpt: '<h1><a href="/projects">Explore AgStack Projects</a></h1>'
projects:
    - image_path: /assets/img/placeholders/apples-rectangle.jpg
      title: "project 1"
      excerpt: "excerpt 1"
      url: "/projects"
      btn_label: "project 1 btn"
      btn_class: "btn--primary"
    - image_path: /assets/img/placeholders/bean-rectangle.jpg
      alt: "A fresh green bean hanging from its plant next to some pink bean flowers, all cushioned by bean leaves"
      title: "project 2"
      excerpt: "excerpt 2"
      url: "/projects"
      btn_label: "project 2 btn"
      btn_class: "btn--primary"
    - image_path: /assets/img/placeholders/wheat-rectangle.jpg
      alt: "A close up of ripe wheat, bowed with the weight of the grain and ready to harvest"
      title: "project 3"
      excerpt: "excerpt 3"
      url: "/projects"
      btn_label: "project 3 btn"
      btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}
{% include feature_row id="explore" type="center" %}