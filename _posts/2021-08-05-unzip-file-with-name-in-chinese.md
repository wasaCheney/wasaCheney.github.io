---
title: 'Unzip file with name in Chinese'
date: 2021-08-05
collection: posts
permalink: /posts/2021/08/unzip-file-with-name-in-chinese/
tags:
  - unzip
  - CP936
  - Chinese
  - unicode
---
<!-- Description for link -->
`unzip -O CP936 <my_zip_file>.zip`
this piece of code could unzip files with Chinese names,
and do not output a mess!

CP936 is a Microsoft's character encoding for simplified Chinese,
and more details in [wiki](https://en.wikipedia.org/wiki/Code_page_936_(Microsoft_Windows))
