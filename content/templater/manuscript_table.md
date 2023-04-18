```
const table = dv.markdownTable(["Arquivo", "Última atualização, status"], dv.pages('"manuscrito"').sort(p => p.file.mtime, 'asc').map(p =>[p.file.link, p.file.mtime]))
dv.paragraph(table)
```