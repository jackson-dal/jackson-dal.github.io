---
layout: home
---

Hi, I'm Jackson, an electrical engineering student focused on power electronics and embedded systems.

## Projects

{% assign projects = site.projects | sort: "date" | reverse %}
{% for project in projects %}
### [{{ project.title }}]({{ project.url | relative_url }})
![{{ project.title }}]({{ project.image | relative_url }})

{{ project.summary }}

*{{ project.tools | join: " · " }}*
{% endfor %}
