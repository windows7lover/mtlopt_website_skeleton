---
layout: page
title: Talks schedule
description: Montreal Machine Learning and Optimization (MTL MLOpt) is a group of researchers living and working in Montréal.
hero_height: is-fullwidth
---


{% assign sortedtalks = site.talks_entries | sort: 'date' | reverse %}

{%  assign current_year = 0  %}

{% for talk in sortedtalks %} {% assign talk_year = talk.date | date: "%Y" %} {% if current_year != talk_year %}  {% assign current_year=talk.date | date: "%Y" %} 
| {{current_year}} | | | | 
|:--- |:--- |:--- | ---:|  
{% endif %} | {{ talk.date | date: "%B %d at %H:%M" }}| {{ talk.author }} | [{{talk.title}}]({{talk.url}})  |  {{ talk.room }}  | 
{% endfor %}




