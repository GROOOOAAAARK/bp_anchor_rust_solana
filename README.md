# GM Solana

Boilerplate using the Anchor template, Anchor SDK and TS for unit testing

## Build

```bash
anchor build
```

## Obtain address for Smart Contract

```bash
solana address -k target/deploy/<programName>-keypair.json
```

Copy this address as `declare_id` macro inside your program, in the Anchor.toml

## Deploy on local net

```bash
solana config set --url localhost && solana-test-validator
```

```bash
anchor deploy --program-name <yourProgramId>
```
