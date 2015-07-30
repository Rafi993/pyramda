# pyramda [![Build Status](https://travis-ci.org/jackfirth/pyramda.svg?branch=master)](https://travis-ci.org/jackfirth/pyramda)
Python package supporting heavy functional programming through currying and function composition. Translation of the Ramda library from javascript to python. Currently only Python 3 is supported.

```python
>>> from pyramda import map, inc
>>> inc(1)
2
>>> map(inc, [1, 2, 3]
[2, 3, 4]
>>> incEach = map(inc)
>>> incEach([1, 2, 3])
[2, 3, 4]
```

### Provided functions

```
add :: Number -> Number -> Number
compose :: (y -> z) ... (a -> b) -> a -> z
curry :: (a b ... -> z) -> a -> b -> ... -> z
equal :: a -> b -> Boolean
filter :: (a -> Boolean) -> [a] -> [a]
getattr :: attr : String -> Object { attr :: a | * } -> a
getitem :: key : k -> Collection { key :: v | * } -> v
isinstance :: Class -> a -> Boolean
map :: (a -> b) -> [a] -> [b]
reduce :: (a -> b -> b) -> a -> [b] -> a
```
