---
layout: home
title: Tools
---

Open-source tools developed by researchers at the
[Co-Centre for Sustainable Food Systems](https://foodcocentre.org).
Each tool lists a **stable release** (hosted here) and a link to the
**latest development version** in the maintainer's repository.

{% for tool in site.data.tools %}
### {{ tool.name }}

{{ tool.description }}

- **Maintainer:** {{ tool.maintainer }}
- **Stable version:** [{{ tool.stable_version }}]({{ tool.stable_repo }}/releases)
- **Latest development version:** [GitHub]({{ tool.latest_repo }})
{% if tool.app_url %}- **Live app:** [Open]({{ tool.app_url }}){% endif %}
{% if tool.doi %}- **Cite:** [{{ tool.doi }}](https://doi.org/{{ tool.doi }}){% endif %}

{% endfor %}
