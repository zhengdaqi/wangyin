---
layout: default
title: Markdown Test
---

Just A Test
-----------


* time
* space
* energy

1. wind
2. fire
3. earth
4. water


---------------------------------------

Some *Scheme* code:

    (define value?
      (lambda (exp)
        (pmatch exp
          [,x (guard (atom? x)) #t]
          [((lambda (,x) ,e) ,env) #t]
          [else #f])))

--------------------------

[I'm an inline-style link](https://www.google.com)

--------------------------

Picture:
![dog](https://encrypted-tbn1.gstatic.com/images?q=tbn:ANd9GcTVZdc4qJd7an7I87cwFr_jum3bD8kululFx0YU8SgSw6Qne4A1)

