# Crypto Research
Curated papers and notes.

## Subfolders
- [DeFi](./DeFi/)

## PDFs in this folder
{% assign all = site.static_files | where_exp: "f", "f.path contains '/Crypto/'" | where: "extname", ".pdf" %}
{% assign top_only = all | where_exp: "f", "f.path contains '/Crypto/DeFi/' == false" %}
{% for f in top_only %}
- [{{ f.name }}]({{ f.path | relative_url }})
{% endfor %}
