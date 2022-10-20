---
layout: page
title: HackEvent 22 @ Virginia Tech
subtitle: Oct 28-30 - 2022 Virginia Tech - Blacksburg, VA
use-site-title: true
header-img: "https://brand.vt.edu/content/brand_vt_edu/en/identity/logo-guidelines/jcr:content/content/adaptiveimage.transform/xl-medium/image.jpg"
share-img: "https://brand.vt.edu/content/brand_vt_edu/en/identity/logo-guidelines/jcr:content/content/adaptiveimage.transform/xl-medium/image.jpg"
---



# Speakers
<div class="container" style="margin-top: 25px;margin-bottom: 40px;">
  {% for p in site.data.speakers %}
  {% if forloop.index<8 %}
  <div class="row">
    <div class="col-sm">
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% include profile.html p=p %}
    </div>
    <div class="col">
    {% capture id %}{{ p[1] }}{% endcapture %}
    {% include profile_detail.html p=p %}
    </div>
  </div>
  <br>
  {% endif %}
  {% endfor %}
</div>
