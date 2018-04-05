---
title: Find a Shed
---
# Locations
The US Men's Shed Community currently has three Sheds in operation in the United States, and another four being formed. Below are the locations of the three Men's Sheds, along with a link to each Shed's web site and the email address of the primary contact for each Shed.

{% for location in site.data.locations %}
  *  [{{ location.name }}]({{ location.web }})
{% endfor %}

{% for location in site.data.locations %}
  <div>
    <iframe width="350" height="350" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="https://www.openstreetmap.org/?mlat={{ location.lat }}&amp;mlon={{ location.long }}#map=12/{{ location.lat }}/{{ location.long }}" style="border: 1px solid black"></iframe><br/><small><a href="https://www.openstreetmap.org/?mlat={{ location.lat }}&amp;mlon={{ location.long }}#map=12/{{ location.lat }}/{{ location.long }}">View Larger Map</a></small>
    <a href="{{ location.web }}">{{ location.name }}</a><br />
    email: <a href="mailto:{{ location.email }}">{{ location.email }}</a><br />
  </div>
{% endfor %}
