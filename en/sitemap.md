---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: page
---
{% assign sorted_pages = site.pages | sort:"order" %}

Welcome! We are exciated that you want to learn more about Aerondo and the features of the platform. On the following sites you find helpful information about each single feature offered by Aerondo and hints how to use them. 

> Please be aware that further development of Aerondo is driven by the community. If you are missing any features or you have ideas for improvements don't hesitate to let us know. In the case you want to send us a Feature request or a proposal for an improvement have a look to our issues on GitHub. If there is no issue describing your request there, just create a new one.ne.

### Getting started

### For Pilots
{% for page in sorted_pages %}
{% if page.section == 'pilots' %}
[{{page.title}}]({{page.url}})
{% endif %}
{% endfor %}