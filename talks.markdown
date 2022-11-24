---
layout: page
title: Talks schedule
description: Montreal Machine Learning and Optimization (MTL MLOpt) is a group of researchers living and working in Montréal.
hero_height: is-fullwidth
---


{% assign sortedtalks = site.talks_entries | sort: 'date' | reverse %}

{% assign first_talk = sortedtalks | first %}
{%  assign current_year = first_talk.date | date: "%Y"  %}
| {{current_year}} | | | |
|:--- |:--- |:--- | ---:|
{% for talk in sortedtalks %} {% assign talk_year = talk.date | date: "%Y" %}{% if current_year == talk_year %} | {{ talk.date | date: "%B %d at %H:%M" }}| {{ talk.author }} | {{ talk.title }}  |  {{ talk.room }}  | {% else %}
{% assign current_year=talk.date | date: "%Y" %}
| {{current_year}} | | | |
|:--- |:--- |:--- | ---:| {% endif %}  
{% endfor %}

