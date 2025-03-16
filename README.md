# Turborepo react-native starter

```bash
rm -rf ./node_modules deno.lock pnpm-lock.yaml
deno clean
pnpm store prune
```

```bash
time deno install
```

````
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
````

````
❯ time pnpm install
//...
________________________________________________________
Executed in   20.61 secs    fish           external
   usr time   10.26 secs    0.08 millis   10.26 secs
   sys time   73.42 secs    2.66 millis   73.42 secs
```

cached:

````

❯ time pnpm install

---

Executed in 868.30 millis fish external
usr time 1.07 secs 0.12 millis 1.07 secs
sys time 0.79 secs 3.24 millis 0.79 secs

```

```
