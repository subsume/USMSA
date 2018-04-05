---
title: Find a Shed
---
# Locations
The US Men's Shed Community currently has three Sheds in operation in the United States, and another four being formed. Below are the locations of the three Men's Sheds, along with a link to each Shed's web site and the email address of the primary contact for each Shed.

* [Minneapolis, Minnesota](Minneapolis,%20Minnesota.yaml)
* [Traverse City, Michigan](Traverse%20City,%20Michigan.yaml)
* [Honolulu, Hawaii](Honolulu,%20CHawaii.yaml)

<ul>
  {% for location in site.data.locations %}
    <li>
      <a href="{{ location.web }}">{{ location.name }}</a>
    </li>
  {% endfor %}
</ul>
