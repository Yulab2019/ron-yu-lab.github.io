---
title: "Yu Lab - Pictures"
layout: piclay
excerpt: "Yu Lab -- Pictures"
permalink: /pictures/
---

# Pictures


## Spring 2018 Team

![]({{ site.url }}{{ site.baseurl }}/images/teampic/team_alt.jpg){: style="width: 100%"}


[//]: # ## 2018 Holiday Party
[//]: # Qianq Qiu and his family
[//]: # <figure>
[//]: # <center><img src="{{ site.url }}{{ site.baseurl }}/images/picpic/2018_holiday/qiang_fam_1.jpg" width="50%"></center>
[//]: # <center><img src="{{ site.url }}{{ site.baseurl }}/images/picpic/2018_holiday/qiang_fam_2.jpg" width="50%"></center>
[//]: # </figure>

# Gallery
{% assign number_printed = 0 %}
{% for pic in site.data.pictures %}

{% assign even_odd = number_printed | modulo: 4 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/picpic/gallery/{{ pic.image }}" class="img-responsive" width="95%" />
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd > 2 %}
</div>
{% endif %}


{% endfor %}

{% assign even_odd = number_printed | modulo: 4 %}
{% if even_odd == 1 %}
</div>
{% endif %}

{% if even_odd == 2 %}
</div>
{% endif %}

{% if even_odd == 3 %}
</div>
{% endif %}

<p> &nbsp; </p>