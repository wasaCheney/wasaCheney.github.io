---
title: 'PDF compressing and splitting'
date: 2021-03-11
collection: posts
permalink: /posts/2021/03/pdf-compressing-and-splitting/
tags:
  - pdf
  - compress
  - split
---
<!-- Description for link -->
Uploading files might encount size limitation, in which case
files need to be compressed and/or split. Here is an 
effective and easy way in Fedora.

`pdfinfo <pdf_file>` is a built-in command Fedora, and it
will show several information about an pdf file, such as
creator, date, pages, page size, file size, etc.

`pdfjam <pdf_file> begin-end` will extract the specific
pages with page number from `begin` to `end`.
