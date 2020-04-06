---

title: Trainers
layout: event_noheader
permalink: /trainers/

---

<link rel="stylesheet" type="text/css" href="/assets/css/training.css">

# {{page.title}}
<br>

{% for trainer in site.data.trainings %}
<section id="{{trainer.SectionId}}">
<hr>
<ul><li><div class="training-header"><div class="training-container no-margin"><div class="training-image" style="background-image:url('{{trainer.Image}}');"></div>
<div class="trainer-header"><h2>{{ trainer.Name }}</h2><br>
             <div class="info-container">
             <a href="mailto:{{trainer.Email}}">{{ trainer.Email }}</a><br>
             <a href="https://www.twitter.com/{{trainer.Twitter}}">@{{ trainer.Twitter }}</a><br>
             <strong>Class:</strong><a href="/trainings/#{{trainer.SectionId}}">{{ trainer.Title }}</a>
             </div>
</div></div></div></li>
<li class='bio-container'><strong>Bio:</strong>{{trainer.Biography}}</li>
</ul>
</section>
{% endfor %}


