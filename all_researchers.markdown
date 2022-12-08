---
layout: page
title: Researchers
# hero_image: /site_images/Maths_banner.jpg
# hero_darken: true
hero_height: is-fullwidth
---


# Professors and Research Scientists #

{% for researcher in site.prof_and_industry %}
{{researcher.name}}
{% endfor %}

# Students and Postdocs #

{% for researcher in site.students_and_postdocs %}
	{{researcher.name}}
{% endfor %}


# Alumnis #
{% for researcher in site.alumnis %}
{{researcher.name}}
{% endfor %}