---
layout: none
---
[{% for organization in site.data.organizations.index %}{
    "id": "{{ organization.id }}",
    "accreditations": "{{ organization.accreditations }}",
    "alternate_name": "{{ organization.alternate_name }}",
    "date_incorporated": "{{ organization.date_incorporated }}",
    "description": "{{ organization.description }}",
    "email": "{{ organization.email }}",
    "funding_sources": [],
    "licenses": [],
    "name": "{{ organization.name }}",
    "website": "{{ organization.website }}",
    "slug": "{{ organization.slug }}",
    "url": "{{ organization.url }}",
    "locations_url": "{{ organization.locations_url }}",
    "contacts": [],
    "phones": []}{% if forloop.last == false %},{% endif %}{% endfor %}]
