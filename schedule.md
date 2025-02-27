---
layout: page
title: HackEvent 22 @ Virginia Tech
subtitle: Oct 28-30 - 2022 Virginia Tech - Blacksburg, VA
use-site-title: true
header-img: "https://brand.vt.edu/content/brand_vt_edu/en/identity/logo-guidelines/jcr:content/content/adaptiveimage.transform/xl-medium/image.jpg"
share-img: "https://brand.vt.edu/content/brand_vt_edu/en/identity/logo-guidelines/jcr:content/content/adaptiveimage.transform/xl-medium/image.jpg"
---


# Schedule

#### Friday, Oct 22, 2022 
#### Location: Whittemore hall 300 on 28th Oct | MyBryde 209|218 for Oct 29th and 30th
#### All times are in ET 

<!-- #### [Link to the live sessions at ICML website](https://www.youtube.com). Note that registration to the ICML main conference is required in order to access the website. -->


<div class="container">
  <div class="row">
    <table class="table">
        {% for s in site.data.schedule %}
        <tr>
        <td>{{ s[1].start }}</td>

        {% if s[1].type == "General" %}
          <td>{{ s[1].event }}</td>
          <td></td>
        {% elsif s[1].type == "Invited" %}
          <td>Invited Talk</td>
          {% assign speaker_id = s[1].event %}
          {% assign speaker = site.data.speakers[speaker_id] %}
          <td>
            <i>{{ s[1].title }}</i><br>
          <a href="{{speaker.url}}">{{ speaker.name }}</a>, {{speaker.affiliation}}
          </td>

        {% elsif s[1].type == "Keynote" %}
          <td><b>Keynote</b></td>
          {% assign speaker_id = s[1].event %}
          {% assign speaker = site.data.speakers[speaker_id] %}
          <td>
            <i>{{ s[1].title }}</i><br>
          <a href="{{speaker.url}}">{{ speaker.name }}</a>, {{speaker.affiliation}}
          </td>
        {% elsif s[1].type == "Contributed" %}
          <td>Contributed Talk</td>
          <td><i>{{ s[1].event }}</i><br>{{ s[1].author }}</td>
        {% elsif s[1].type == "Session" %}
          <td><b>{{ s[1].event }}</b></td>
          <td></td>
        {% elsif s[1].type == "Panel" %}
          <td>Discussion Panel</td>
          <td><i>{{ s[1].event }}</i><br>{{ s[1].speakers }}</td>
        {% endif %}
        </tr>
        {% endfor %}
    </table>
  </div>
</div>
