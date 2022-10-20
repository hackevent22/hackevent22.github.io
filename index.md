---
layout: page
title: HackEvent 22 @ Virginia Tech
subtitle: Oct 28-30 - 2022 Virginia Tech - Blacksburg, VA
use-site-title: true
header-img: "https://brand.vt.edu/content/brand_vt_edu/en/identity/logo-guidelines/jcr:content/content/adaptiveimage.transform/xl-medium/image.jpg"
share-img: "https://brand.vt.edu/content/brand_vt_edu/en/identity/logo-guidelines/jcr:content/content/adaptiveimage.transform/xl-medium/image.jpg"
---

<!-- <div class="sharethis-inline-share-buttons"></div>
<meta name="thumbnail" content="./img/logo.png" /> -->

# Overview
HACKEVENT 2022 will be a hybrid 2-2.5 day event organised by Advanced Research computing at Virginia Tech. The goal of this event is to educate students empirically on how to efficiently leverage computer architecture and software for heterogeneous applications and develop critical thinking towards synergistic evaluation of software and hardware for applications ranging from artificial intelligence to distributed systems.  The event will feature guest lectures, hands-on training sessions and tutorials from professionals in industry and academia.  The event will be free for students currently pursuing a degree in any academic institution. The event will take place in Eastern Time Zone (New York).  Upon successful completion of the event the students will receive a completion certificate and prizes for a mini competition also to be held with the event.

**Announcements**
* Our Flyer is out Now!!! Check [this out](./postermaroon.pdf) 
* Our schedule is [announced](https://hackevent22.github.io/schedule/)!
* Our Speakers are finalized and [available](https://hackevent22.github.io/) now!

<!-- * [Link to the **live sessions** at Hackevent website](https://www.youtube.com). Note that registration to the hackevent is required in order to access the ARC resources. -->

**KeyNote:** Oct 28, 2022- 5PM by Dr Wu Feng <br>
**Registration Deadline:** Oct 25, 2022 (Anywhere on Earth) <br>
**Account Access ARC Resources:** Oct 26, 2022 <br>
**IBM Sessions:** Oct 28-30th, 2022 <br>
**Sessions by Open OnDemand:** Oct 30th, 2022 <br>
**Session by Neural Magic:** Oct 29th, 2022 <br>


<hr>

# Speakers [(More Info)](https://hackevent22.github.io/speakers/)
<div class="container" style="margin-top: 20px;margin-bottom: 0px;">
  <div class="row">
  <h2> Keynote Speakers </h2>
  {% for p in site.data.speakers %}
  {% if forloop.index<=5 %}
  {% capture id %}{{ p[0] }}{% endcapture %}
  {% include profile.html p=p %}
  {% endif %}
  {% endfor %}
  </div>
  <h2> Invited Speakers </h2>
  <div class="row">
  {% for p in site.data.speakers %}
  {% capture id %}{{ p[0] }}{% endcapture %}
  {% if forloop.index>5 %}
  {% include profile.html p=p %}
  {% endif %}
  {% endfor %}
  </div>
</div>

<hr>

# Organizers
<!-- prettier-ignore -->
<div class="container" style="margin-top: 20px;margin-bottom: 0px;">
  <div class="row">
    {% for p in site.data.organizers %}
    {% capture id %}{{ p[0] }}{% endcapture %}
    {% if forloop.index<=4 %}
    {% include profile.html p=p %}
    {% endif %}
    {% endfor %}
  </div>
  <div class="row">
  {% for p in site.data.organizers %}
  {% capture id %}{{ p[0] }}{% endcapture %}
  {% if forloop.index>4 and forloop.index<=8%}
  {% include profile.html p=p %}
  {% endif %}
  {% endfor %}
  </div>

</div>
<hr>


<!-- prettier-ignore -->
<!-- original list class in the template
  <ul class="list-group list-group-flush">
      <li class="list-group-item col-xs-6 col-sm-4 col-md-3">{{ p }}</li> 
<h3>Confirmed:</h3>-->

<hr>





<!-- # Related Venues

<div class="container" style="margin-bottom: 10px;"></div>

- [Automated Knowledge Base Construction (AKBC'20)](http://www.akbc.ws/2020/)
- [Workshop on Semantic Deep Learning (SemDeep'20)](http://www.dfki.de/~declerck/semdeep-6/)
- [Workshop on Deep Learning for Knowledge Graphs (DL4KG'20)](https://alammehwish.github.io/dl4kg_eswc_2020/)
- [Workshop on Semantic Explainability (SEMEX'20)](http://www.semantic-explainability.com/)
- [Workshop on Statistical Relational AI (StarAI'20)](http://www.starai.org/2020/)
- [Workshop on Neural-Symbolic Learning and Reasoning (NeSys'19)](https://sites.google.com/view/nesy2019/home), see more on <http://www.neural-symbolic.org/>

<div class="container" style="margin-bottom: 10px;"></div> -->

<hr>

Contact: [hackevent-22g@vt.edu](hackevent-22g@vt.edu)
