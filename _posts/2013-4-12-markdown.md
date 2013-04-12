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

> quote
> haha
> ok

- [ ] a task list item
- [ ] list syntax required
- [ ] normal **formatting**, @mentions, #1234 refs
- [ ] incomplete
- [x] completed

---------------------------------------

Some Scheme code:

    (define value?
      (lambda (exp)
        (pmatch exp
          [,x (guard (atom? x)) #t]
          [((lambda (,x) ,e) ,env) #t]
          [else #f])))

--------------------------

Muahahahahhaha
