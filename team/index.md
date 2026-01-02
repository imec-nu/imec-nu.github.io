---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team


{% include list.html data="members" component="portrait" filters="role: pi" %}
{% include list.html data="members" component="portrait" filters="role: ^(phd$)" %}
{% include list.html data="members" component="portrait" filters="role: visitingphd" %}
{% include list.html data="members" component="portrait" filters="role: ^(ms$)" %}
{% include list.html data="members" component="portrait" filters="role: undergrad" %}

{% include section.html %}

# {% include icon.html icon="fa-solid fa-users" %}Alumni

{% include list.html data="members" component="portrait" filters="role: ^(alum_ms$)" %}


