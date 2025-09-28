# DeFi (Crypto) Papers

Below are all PDFs in this folder:

{% assign pdfs = site.static_files | where_exp: "f", "f.path contains '/Crypto/DeFi/'" | where: "extname", ".pdf" %}
{% if pdfs.size > 0 %}
{% for f in pdfs %}
- [{{ f.name }}]({{ f.path | relative_url }})
{% endfor %}
{% else %}
- (No PDFs yet)
{% endif %}
