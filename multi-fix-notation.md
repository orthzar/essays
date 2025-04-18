# Most Programming Languages Use Every Style of Notation

It is often claimed that popular programming languages use infix notation, but this is obviously false.

Consider this psuedo-code:

```
function foo:
  arguments:
    a
    b
  body:
    add(a, b) + add(a, b);
```

```+``` and ```add()``` do exactly the same thing.  The former is infix notation; the latter is prefix notation.  The keyword ```function``` precedes ```foo```,  ```arguments:```, and ```body:```, so this is indisputably prefix notation.  The keyword statement ends with a ```;```. So that's two forms of syntax in one language (```x```,```y``` are operators, ```a```,```b```,```c``` are operands):

- Infix: ```axb```, and
- Prefix: ```x a``` / ```x(a)```.

The only thing missing is two more forms of post-fix notation and we'll have every kind of notation:

- ```(a)x```, and
- ```ax``` (e.g. ...2;).

But wait, ```:``` and ```;``` are operators: the former is a psuedo-infix notation; the latter post-fix notation.  So the psuedo-code snippet actually contains all three kinds of notation!
- Infix: ```axb``` / ```ax b c```
- Prefix: ```x a``` / ```x(a)```, and
- Post-fix ```ax```.

The only thing missing is Forth-style post-fix notation (```a x```) and you'd have every kind and variation of notation.  (I am so close to making such a language.)

Most languages use this multi-fix notation, which is why metaprogramming is so uncommon; macros would require templates and pattern-matching, which are non-trivial to design and implement.  If such languages would use only one kind of notation, macros would be trivial to design/implement.

You wanted to avoid Lisp-like syntax, and you gave yourself every kind of notation instead, including two forms of prefix notation, one of which has parentheses!  Is there some obscure law that requires language designers be meth-heads?  Avoiding X by implementing everything else plus two alternative forms of X is not logical!
