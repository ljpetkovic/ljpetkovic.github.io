---
layout: single
title: "DEBUG TALKS"
permalink: /debug-talks/
---

# site.talks size
Nombre d’items : {{ site.talks | size }}

# List of items:
{% for t in site.talks %}
- **{{ t.title }}**  
  path = {{ t.path }}  
  category = {{ t.category }}  
  date = {{ t.date }}  
{% endfor %}

--- RAW DUMP ---
<pre>
{{ site.talks | jsonify }}
</pre>
