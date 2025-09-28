---
title: Crypto Research
layout: page
---

Curated papers and notes.

## Subfolders
- [DeFi](./DeFi/)

## PDFs in this folder
{% assign pdfs = site.static_files | where: "extname", ".pdf" %}
{% for f in pdfs %}
{% if f.path contains '/Crypto/' and f.path contains '/Crypto/DeFi/' == false %}
- [{{ f.name }}]({{ f.path | relative_url }})
{% endif %}
{% endfor %}
