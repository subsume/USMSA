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
    <iframe width="350" height="350" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="https://www.openstreetmap.org/export/embed.html?mlat={{ location.lat }}&amp;mlon={{ location.long }}#map=12/{{ location.lat }}/{{ location.long }}" style="border: 1px solid black"></iframe><br/><small><a href="https://www.openstreetmap.org/?mlat={{ location.lat }}&amp;mlon={{ location.long }}#map=12/{{ location.lat }}/{{ location.long }}">View Larger Map</a></small>
    <iframe width="425" height="350" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="https://www.openstreetmap.org/export/embed.html?bbox=-85.86021423339845%2C44.62199845891659%2C-85.59791564941408%2C44.84588953618059&amp;layer=mapnik&amp;marker={{ location.lat }}%2C{{ location.long }}" style="border: 1px solid black"></iframe><br/><small><a href="https://www.openstreetmap.org/?mlat=44.7341&amp;mlon=-85.7291#map=12/44.7341/-85.7291">View Larger Map</a></small>
    <iframe src="http://maps.google.co.uk/maps?q={{ location.lat }},{{ location.long }}&output=embed" width="300" height="300"></iframe>
    <br>
    <a href="{{ location.web }}">{{ location.name }}</a>
    <br>
    email: <a href="mailto:{{ location.email }}">{{ location.email }}</a>
  </div>
{% endfor %}
