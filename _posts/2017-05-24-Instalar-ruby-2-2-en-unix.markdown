---
title:  "Instalar Ruby 2.2 en UNIX"
date:   2017-05-24 13:25:00
comments: true
categories: [ruby, unix]
tags: [ruby, unix]
---

Necesitamos instalar Ruby en nuestro sistema Unix local para poder realizar la instalación de `jekyll` y poder utilizarlo. El problema principal es que la instalación por defecto en `apt-get` es la versión 1.9.3 que es demasiado antigua.

Podemos superar dicho problema realizando lo siguiente en línea de comandos

```
$ sudo apt-add-repository ppa:brightbox/ruby-ng
$ sudo apt-get update
$ sudo apt-get install ruby2.2

$ ruby2.2 -v
ruby 2.2.0p0 (2014-12-25 revision 49005) [x86_64-linux-gnu]
```