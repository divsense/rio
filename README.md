# Rio
## Functional Programming Language that compiles to Javascript

Generates ES2016 compatible AST.
Assumes Ramda.js as a 'standard' library.

Rio           | Javascript       | Why?                                 | Notes
------------- | ---------------- | -------------------------------------- | ------- 
m = 1         | const m = 1      | 'const' is the only type in Rio        |
`n/a`         | var x = 2        | Rio does not allow mutations           |
`n/a`         | let x = 3        | same as above                          |
f = x -> !x   | const f = x => !x | The thin arrow reminds that in Rio there is no access to 'this' | ... as well as to 'arguments'
c = f . g . h     | const c = f(g(h))  |                                | 
p = resolve(1) >>> delay   | const p = Promise.resolve(1).then(delay)   |   | requires: import 'promise'






