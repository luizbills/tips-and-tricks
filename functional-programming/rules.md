```js
compose(f, g) == f(g)
```

```js
// head :: [a] -> a
compose(f, head) == compose(head, map(f));
```
```js
// filter :: (a -> Bool) -> [a] -> [a]
compose(map(f), filter(compose(p, f))) == compose(filter(p), map(f));
```

```js
// id :: a -> a
// for every unary (one argument function) function f
compose(id, f) == compose(f, id) == f;
```
