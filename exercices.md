---
layout: page
title: Exercices
permalink: /exercices/
---


Voici les exercices et TP (<i class="fas fa-file-archive"></i>) : 
<ul id="archive">
{% for exercices in site.data.exercices %}
      <li class="archiveposturl">
        <span><a href="{{ site.url }}/{{ exercices.dirname }}/{{ exercices.filename }}.zip">{{ exercices.title }}</a></span><br>
        <span class = "postlower">
        <strong>Description : </strong> {{ exercices.tldr }}</span>
<!-- <strong style="font-size:100%; font-family: 'Titillium Web', sans-serif; float:right">
	<a href="https://github.com/{{ site.githubdir}}/tree/master/{{ lectures.dirname }}"><i class="fab fa-github"></i></a>&nbsp;&nbsp;
<a href="https://github.com/{{ site.githubdir}}/tree/master/{{ lectures.dirname }}/{{ lectures.filename}}.Rmd"><i class="fab fa-r-project"></i></a>&nbsp;&nbsp;
<a href="https://github.com/{{ site.githubdir}}/blob/master/{{ lectures.dirname }}/{{ lectures.filename}}.pdf"><i class="fas fa-file-pdf"></i></a>
</strong>  -->
      </li>
{% endfor %}
</ul>