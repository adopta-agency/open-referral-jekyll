---
layout: none
---
[{% for organization in site.data.organizations.index %}
  {
    "id": "{{ organization.id }}",
    "accreditations": "{{ organization.id }}",
    "alternate_name": "{{ organization.id }}",
    "date_incorporated": "{{ organization.id }}",
    "description": "{{ organization.id }}",
    "email": "{{ organization.id }}",
    "funding_sources": [],
    "licenses": [],
    "name": "{{ organization.id }}",
    "website": "{{ organization.id }}",
    "slug": "{{ organization.id }}",
    "url": "{{ organization.id }}",
    "locations_url": "{{ organization.id }}",
    "contacts": [],
    "phones": []
  }{% if forloop.last == false %},{% endif %}
{% endfor %}]
