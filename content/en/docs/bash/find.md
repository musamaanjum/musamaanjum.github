---
title: "Find"
description: ""
lead: ""
date: 2020-10-13T15:21:01+02:00
lastmod: 2020-10-13T15:21:01+02:00
draft: false
images: []
menu:
  docs:
    parent: "bash"
weight: 130
toc: false
---


#### Find files of size more than 1G
```bash
find . -type f -size +1G
```

#### find and delete
```bash
find /home -type f -size +1G -delete
```

#### find in all dir
```bash
find /path -iname 'yourstring*' -type f
find . -name 'mystring*'
```
