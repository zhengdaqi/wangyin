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


---------------------------------------

Some code:

    (define value?
      (lambda (exp)
        (pmatch exp
          [,x (guard (atom? x)) #t]
          [((lambda (,x) ,e) ,env) #t]
          [else #f])))

--------------------------

Muahahahahhaha
