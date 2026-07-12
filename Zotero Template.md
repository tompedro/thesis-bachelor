---
titolo: "{{title}}"
autori: {{authors}}
anno: {{date}}
chiave_bibliografica: {{citekey}}
tags: [letteratura/da_processare]
---

# {{title}}
[Apri in Zotero]({{pdfZoteroLink}})

## Abstract
{{abstractNote}}

## Derivazioni e Annotazioni

{% for annotation in annotations %}
{% if annotation.annotatedText %}
> {{annotation.annotatedText}}
{% endif %}
{% if annotation.imageRelativePath %}
![[{{annotation.imageRelativePath}}]]
{% endif %}
{% if annotation.comment %}
- *Osservazione:* {{annotation.comment}}
{% endif %}

{% endfor %}