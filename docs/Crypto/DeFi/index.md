---
title: DeFi (Crypto) Papers
layout: page
---

Below are all PDFs in this folder:

{% assign pdfs = site.static_files | where: "extname", ".pdf" %}
{% for f in pdfs %}
{% if f.path contains '/Crypto/DeFi/' %}
- [{{ f.name }}]({{ f.path | relative_url }})
{% endif %}
{% endfor %}
