---
title: "Awk"
description: ""
lead: "Awk is text-processing utility."
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

{{< alert icon="💡" text="The name of AWK is derived from the surnames of its authors: Alfred Aho, Peter Weinberger, and Brian Kernighan." />}}

#### Print Lines Containing tom, jerry AND vivek

```bash
awk '/tom|jerry|vivek/' /etc/passwd
```

#### Specify : as seperator

```bash
awk -F: '{print $1}' /etc/passwd
```

#### use of printf

```bash
awk '{printf "%s ",$2}' file
```

#### Command line on bash

```bash
awk '
  BEGIN { actions } 
  /pattern/ { actions }
  /pattern/ { actions }
      ……….
   END { actions } 
' filenames

Execute a awk script
awk -f mypgoram.awk input.txt

#### Process and print
echo 4000000 | awk '{print $1*10^-6 " Wh"}'
```
