# Architecture

## Dependency Graph

```mermaid
graph TD
  5de60226["Web2-frontend-scaffold (web2-frontend-scaffold)"]
  320c81d6["Http-api (http-api)"]
  d2396441["Variable-store (variable-store)"]
  29cbd0fb["Transform (transform)"]
  0493472a["Delay-timer (delay-timer)"]
  f297985a["If-else (if-else)"]
  310f14b1["Loop-iterator (loop-iterator)"]
  e944cbf5["Email-smtp (email-smtp)"]
  5de60226 --> 320c81d6
  320c81d6 --> 29cbd0fb
  29cbd0fb --> f297985a
  f297985a --> e944cbf5
  5de60226 --> d2396441
  d2396441 --> 0493472a
  0493472a --> 310f14b1
```

## Execution / Implementation Order

1. **Web2-frontend-scaffold** (`5de60226`)
2. **Http-api** (`320c81d6`)
3. **Variable-store** (`d2396441`)
4. **Transform** (`29cbd0fb`)
5. **Delay-timer** (`0493472a`)
6. **If-else** (`f297985a`)
7. **Loop-iterator** (`310f14b1`)
8. **Email-smtp** (`e944cbf5`)
