- 定义make-cycle过程、
```
(define (make-cycle x)
    (set-cdr! (last-pair x) x)
    x)
```
`从代码中可以知道它将x的最后一个序对的cdr指向了x本身，这将形成一个环。`

`(define z (make-cycle (list 'a 'b 'c)))`

![](a.jpg)