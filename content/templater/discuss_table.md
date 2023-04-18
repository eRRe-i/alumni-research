

```
const table = dv.markdownTable(["Arquivo", "Última atualização"], dv.pages('"discussoes"').sort(p => p.file.mtime, 'asc').map(p =>[p.file.link, p.file.mtime]))
dv.paragraph(table)
```


