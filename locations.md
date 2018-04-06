---
title: Find a Shed
---
# Locations
The US Men's Shed Community currently has three Sheds in operation in the United States, and another four being formed. Below are the locations of the three Men's Sheds, along with a link to each Shed's web site and the email address of the primary contact for each Shed.

{% for location in site.data.locations %}
  <div>
    <h2><a href="{{ location.web }}">{{ location.name }}</a></h2>
    email: <a href="mailto:{{ location.email }}">{{ location.email }}</a>
    <iframe src="https://maps.google.co.uk/maps?q={{ location.lat }},{{ location.long }}&output=embed" width="300" height="300"></iframe>
    <hr>
  </div>
{% endfor %}
