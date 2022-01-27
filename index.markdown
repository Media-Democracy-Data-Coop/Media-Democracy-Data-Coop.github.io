---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

{:refdef: style="text-align: center;"}
![MDDC Logo](/assets/images/mddc_logo.png)
{: refdef}

Welcome to the home page of the Media & Democracy Data Cooperative (MDDC). 	

The Media and Democracy Data Cooperative (MDDC, pronounced "medic") is a collaborative effort across multiple research centers to advance research using digital data, particularly in the areas of political media and communication. MDDC's mission has two pillars: (1) to advance digital data collection efforts and (2) to provide opportunities for collaborative research across our members.

{% assign sorted_pages = site.pages | sort:"order" %}
{% for node in sorted_pages %}
  <li><a href="{{node.url}}">{{node.title}}</a></li>
{% endfor %}