# campus project notes

## check essays against records

Check the _histories to see how they match up with campus-buildings.csv:

```
---
---
filename,buildingid,title,length
{% for h in site.histories %}{{ h.name }},{{ h.buildingid }},"{{ h.title | escape }}",{{ h.content | size }}
{% endfor %}
```

## brinkandphinneyhalls note

old collection had brinkandphinneyhalls as a single combined record.
new collection adds separate records for carolryriebrinkhall and archiephinneyhall.
