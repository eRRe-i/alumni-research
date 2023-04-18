---
title: "Discussão"
enableToc: false
---
# Discussões

Discussões são ideias mais ou menos inacabadas que podem ou não tornarem-se parte de um capítulo ou subcapítulo do [Manuscrito](main_pages/manuscrito.md) e possui, sempre que possível, apontando uma ou mais [Referências](main_pages/referencias.md)

```dataviewjs
const table = dv.markdownTable(["Arquivo", "Última atualização"], dv.pages('"discussoes"').sort(p => p.file.mtime, 'desc').map(p =>[p.file.link, p.file.mtime]))
dv.paragraph(table)
```




















