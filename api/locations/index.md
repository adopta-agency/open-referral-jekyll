---
layout: none
---
[{% for location in site.data.locations.index %}{
    "id": {{ location.id }},
    "active": {{ location.active }},
    "admin_emails": [
      "admin@example.com"
    ],
    "alternate_name": "{{ location.alternate_name }}",
    "coordinates": [],
    "description": "{{ location.description }}",
    "latitude": "{{ location.latitude }}",
    "longitude": "{{ location.longitude }}",
    "name": "{{ location.name }}",
    "short_desc": "{{ location.short_desc }}",
    "slug": "{{ location.slug }}",
    "website": "{{ location.website }}",
    "updated_at": "{{ location.updated_at }}",
    "url": "{{ location.url }}",
    "address": "{{ location.address }}",,
    "organization": {
      "id": 1,
      "accreditations": [],
      "alternate_name": "An Alternate name",
      "date_incorporated": null,
      "description": "This is a description of the organization, providing details about what it does.",
      "email": "info@example.com",
      "funding_sources": [],
      "licenses": [],
      "name": "First Organization",
      "website": "https://example.com",
      "slug": "first-organization",
      "url": "https://example.org",
      "locations_url": "https://example.com"
    },
    "phones": []}{% if forloop.last == false %},{% endif %}{% endfor %}]
