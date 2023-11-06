---
layout: page
title: Organizers
hero_height: is-fullwidth
---

<style>

table {
  border-spacing: 30px;
}

#profile {
  font-family: Helvetica, sans-serif;
  width: 100%;
  max-width: 75em
}

#profile td, #profile th {
  border: 0px solid #ddd;
  padding: 3%;
}

#profile tr {
  background-color: #ffffff;
  text-align: center;
}

#profile td:hover {
background-color: #ddd;
border-radius: 5%;
}
</style>

# Current #

<table id="profile">
{% tablerow researcher in site.current_organizers cols:4 %}
  {% include researcher_profile.html %}
{% endtablerow %}
</table>

# Alumnis #

<table id="profile">
{% tablerow researcher in site.alumnis cols:4 %}
  {% include researcher_profile.html %}
{% endtablerow %}
</table>