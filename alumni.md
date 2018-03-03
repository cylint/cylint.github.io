---
layout: page
title: Alumni
permalink: /get-involved/alumni
---

# Alumni Board
While the Alumni Board is comprised of specific positions, we encourage any and everyone to be active within the alumni group. Even if you can only spare a few minutes of your time, we could always use it! Please contact [Alex Ott](mailto:ajott@mtu.edu) to get on our Alumni Executive Board email list.

{% include spotlight-inline.html
  name="Wilmer Lidke"
  position="Alumni President"
  email_address="wblidke@mtu.edu"
  cover-image="http://mtutriangle.org/wp-content/uploads/2016/08/wilmer100.jpg"
content="
"%}

{% include spotlight-inline.html
  name="Troy Bouman"
  init-year="09"
  position="Alumni Treasurer"
  email_address="tmbouman@mtu.edu"
  cover-image="http://mtutriangle.org/wp-content/uploads/2016/01/XGTNE9b-Imgur.jpg"
  content="
I graduated from Tech in 2012 after 5 awesome years. During my time as an active I was the VP of New Member Education and Treasurer!
"%}

{% include spotlight-inline.html
  name="Alex Ott"
  init-year="11"
  position="Alumni Secretary"
  email_address="ajott@mtu.edu"
  cover-image="http://mtutriangle.org/wp-content/uploads/2016/01/Ott-Photo.jpg"
  content="
I graduated from Michigan Tech in 2016 with a BS in Engineering Management, after 4 years as an active and 1 year as an alumnus. I served in a number of positions, including VP of Member Development and as the Alumni Relations Chair.
"%}

# Committees

Committees are established to better serve the Alumni and Active Organizations. While there may be any number of provisional committees at any time, these committees in particular are intended to provide long-term and in-depth support to the Fraternity.

## Member Development Committee
{% include spotlight-inline.html
  name="Mike Spenle"
  position="Alumni Member Development Committee Chair"
  init-year="13"
  email_address="mdspenle@mtu.edu"
  cover-image="http://mtutriangle.org/wp-content/uploads/2015/12/spenle.png"
  content="
"%}

{% for file in site.static_files %}
{% if file.path contains "/assets/docs/newsletters/" %}
- [{{ file.basename }}]({{ file.path | relative_url }})
{% endif %}
{% endfor %}
