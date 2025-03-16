# Turborepo react-native starter

- https://github.com/ansemb/deno-install-peer-deps/tree/main
- https://github.com/ansemb/deno-install-peer-deps/tree/test-with-lock
- https://github.com/ansemb/deno-install-peer-deps/tree/test-no-peers

## main

setup before each command:
```bash
rm -rf ./node_modules deno.lock pnpm-lock.yaml
deno clean
pnpm store prune
```

```bash
time deno install
```

```
❯ time deno install
//...
________________________________________________________
Executed in  352.56 secs    fish           external
   usr time  607.77 secs    0.08 millis  607.77 secs
   sys time  104.72 secs    2.81 millis  104.72 secs
```

---

```bash
time pnpm install
```

```
❯ time pnpm install
//...
________________________________________________________
Executed in   23.16 secs    fish           external
   usr time   12.26 secs    0.09 millis   12.26 secs
   sys time   78.50 secs    3.33 millis   78.49 secs
```


## test-with-lock

- https://github.com/ansemb/deno-install-peer-deps/tree/test-with-lock

```
❯ time deno install
//...
________________________________________________________
Executed in   17.53 secs    fish           external
   usr time    7.59 secs    0.11 millis    7.59 secs
   sys time   59.51 secs    3.68 millis   59.50 secs
```

cached:
```
❯ time deno install
________________________________________________________
Executed in    1.20 secs    fish           external
   usr time    1.01 secs    0.09 millis    1.01 secs
   sys time    0.14 secs    2.25 millis    0.13 secs
```

---

```bash
time pnpm install
```

```
❯ time pnpm install
//...
________________________________________________________
Executed in   20.61 secs    fish           external
   usr time   10.26 secs    0.08 millis   10.26 secs
   sys time   73.42 secs    2.66 millis   73.42 secs
```

cached:

```
❯ time pnpm install

---

Executed in 868.30 millis fish external
usr time 1.07 secs 0.12 millis 1.07 secs
sys time 0.79 secs 3.24 millis 0.79 secs
```

## test-no-peers

- https://github.com/ansemb/deno-install-peer-deps/tree/test-no-peers

```bash
time deno install
```

```
❯ time deno install
//...
________________________________________________________
Executed in  342.35 secs    fish           external
   usr time  608.49 secs    0.13 millis  608.49 secs
   sys time   76.27 secs    3.48 millis   76.26 secs
```

---

```bash
time pnpm install
```

```
❯ time pnpm install
//...
________________________________________________________
Executed in   23.01 secs    fish           external
   usr time   12.42 secs    0.10 millis   12.42 secs
   sys time   79.10 secs    3.48 millis   79.10 secs
```


