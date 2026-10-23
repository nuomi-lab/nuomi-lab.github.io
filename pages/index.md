---
layout: page
permalink: /
---


{% include masthead.html %}


<section id="about" markdown="1">
{% include content/about.md %}
</section>


<section id="research" markdown="1">
{% include content/research.md %}
</section>


{% if site.show_publications %}
<section id="publications" markdown="1">

# **Selected Publications**

The following is a short list of publications that represents our research vision and approaches. For a full list of publications, please see the [Google Scholar page](https://scholar.google.com/) for Weiwei Pan. <!-- TODO: replace with the full Google Scholar profile URL -->

<div class="publications">
{% bibliography -f selected_publications.md %}
</div>

</section>
{% endif %}


<section id="people" markdown="1">
{% include people.html %}
</section>


<section id="joining" markdown="1">
{% include content/joining.md %}
</section>


<section id="resources" markdown="1">
{% include content/resources.md %}
</section>
