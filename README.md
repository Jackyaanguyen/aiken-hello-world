# Aiken hello_world contract

How to run this project:

Step 1: Download dependencies

```
aiken check
```

Step 2:  Build contract

```
aiken build
```

Step 3: Generate a private key and an address using Lucid

```
deno run --allow-net --allow-write generate-credentials.ts
```

Step 4: Run lock scripts
```
deno run --allow-net --allow-read --allow-env hello_world-lock.ts
```

Step 5: Run unlocking scripts
```
deno run --allow-net --allow-read --allow-env hello_world-unlock.ts <TX_HASH_OF_LOCK_TRANSACTION>
```