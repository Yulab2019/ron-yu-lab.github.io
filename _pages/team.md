---
title: "Yu Lab - Team"
layout: gridlay
excerpt: "Yu Lab: Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **We are  looking for a new postdoc and a laboratory assistant to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies)**!**

## Staff
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}




## PhD students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Graduate researchers
{% assign number_printed = 0 %}
{% for member in site.data.interns %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Visiting fellows

{% assign number_printed = 0 %}
{% for member in site.data.fellows %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %}

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %}

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.duration }} <br> Role: {{ member.info }}<br>email: <{{ member.email }}></i>
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


<table align="center" style="width:100%">
 <tr>
    <th>Postdoctoral Research Associate </th>
    <th>Research Technicians</th>
    <th>Graduate Researchers</th>
  </tr>
  <tr>
    <td>Jie He, 2005–2010</td>
    <td>Evan Gillespie, 2005–2007</td>
    <td>Vasha DuTell, 2013–2015</td>
  </tr>
  <tr>
    <td>Oxana Litvine, 2005–2007</td>
    <td>Peniel Zelalem, 2006–2007</td>
    <td>Dar Dahlen, 2013–2015</td>
  </tr>
  <tr>
    <td>SangSeong Kim, 2007–2012</td>
    <td>Arian Abdulla, 2007–2008</td>
    <td>Jason Catalico, 2016–2017</td>
  </tr>
  <tr>
    <td>Zhuoming Li, 2007–2011</td>
    <td>Nirjal Sapkota, 2007–2008</td>
    <td></td>
  </tr>
  <tr>
    <td>Sachiko Haga-Yamanaka, 2010–2014</td>
    <td>Aaron Scott, 2008–2009</td>
    <td></td>
  </tr>
  <tr>
    <td>Elden Yu, 2010–2011</td>
    <td>Justin Ryder, 2010–2011</td>
    <td></td>
  </tr>
  <tr>
    <td>Zhenhua Gui, 2010–2011</td>
    <td>Kristin Jensen, 2010–2011</td>
    <td></td>
  </tr>
  <tr>
    <td>Zulin Yu, 2010–2011</td>
    <td>Ian Smith, 2011–2012</td>
    <td></td>
  </tr>
  <tr>
    <td>Lakshmi Chandrashaka, 2011–2014</td>
    <td>Amurta Nath, 2012–2013</td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td>Daniel Lee, 2011–2013</td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td>Daniel Friedman, 2014–2015</td>
    <td></td>
  </tr>

</table>

<table align="center" style="width:100%">
  <tr>
    <th>Undergraduate Students</th>
  </tr>
  <tr>
    <td>2005 – Stowers Scholar: Emily Abdoler</td>
  </tr>
  <tr>
    <td>2006 – Stowers Scholar: Stefani Fontana & Sutton Ansley</td>
  </tr>
  <tr>
    <td>2007 – Stowers Scholar: Stephen Gradwohl</td>
  </tr>
  <tr>
    <td>2008 – Stowers Scholar: Justin Ryder & Jing Hu</td>
  </tr>
  <tr>
    <td>2009 – Stowers Scholar: Megan Fracol & Andrew Satterlee, Lingxue Zhang & Katharina Grauel </td>
  </tr>
  <tr>
    <td>2010 – Lingxue Zhang & Xinyun Peng, Internship</td>
  </tr>
  <tr>
    <td>2010 – Stowers Scholar: Megan Fracol, Andrew Satterlee, & Roman Becicka, Shan Shen & Tao Wang</td>
  </tr>
  <tr>
    <td>2011 – Stowers Scholar: Colleen McLaughlin, Vivekanandan Ramalingam, Amurta Nath, Wanlu Liu, Yilin Li, Yunming Wu & Martula Kolodziejczek </td>
  </tr>
  <tr>
    <td>2012 – Stowers Scholar: Matthew Bruce, Megan Hoffman, Nimish Mittal, Daniel Friedman, Yin (Jerry) Yue, Sri Karthika Shanmugam, Karthikeyan Murugesan & Zheng (Cindy) Xing</td>
  </tr>
  <tr>
    <td>2013 – Stowers Scholars: Rishabh Raj, Zita Hubler, Laura Nay and Florian Bilz</td>
  </tr>
</table>

<table align="center" style="width:100%">
  <tr>
    <th>Interns</th>
  </tr>
  <tr>
    <td>2014 – Stowers Scholar: Sruti Raja, Wenjing Xu</td>
  </tr>
  <tr>
    <td>2015 – Stowers Scholar: Mohamed Eltabbal; Intern: Clara Ma; St. Luke Hostpital Interns: Tyler Jost, Madison McCulloch, John Shook</td>
  </tr>
  <tr>
    <td>2016 – Stowers Scholar:	Ruohan Zhong, Grace Li-Haug, Sam Dore; Shashank Chepurwar; Paris VII intern: Malalaniaina Rakotobe</td>
  </tr>
  <tr>
    <td>2017 – Stowers Scholar:	Kevin Li, Renny Ma, Tyler Jost; Paris VII intern: Ronael Yablanka</td>
  </tr>
  <tr>
    <td>2018 – Stowers Scholar:	Kevin Li, Sandon Scott, Edwin Qiu, Yiyang “Reus” Zhu; Paris VII intern: Clarisse Dumont</td>
  </tr>
</table>


## Administrative Support
<a href="mailto:iwarren@stowers.org">Indigo Warren</a> is helping us (and other groups) with administration.
