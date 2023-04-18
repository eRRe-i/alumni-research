---
title: "changelog"
---
```dataviewjs
const table = dv.markdownTable(["Arquivo", "Título", "Última atualização", "Status"], dv.pages('"manuscrito"').sort(p => p.file.mtime, 'desc').map(p =>[p.file.link, p.title, p.file.mtime, p.status]))
dv.paragraph(table)
```






