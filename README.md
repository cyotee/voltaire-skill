# voltaire-effect

Progressive disclosure skills for [voltaire-effect](https://voltaire-effect.tevm.sh) - Effect.ts integration for Voltaire Ethereum primitives.

## Skills

| Skill | Topic |
|-------|-------|
| `voltaire-effect-architecture` | Three-layer model, Decode→Use→Provide pattern, comparison with viem/ethers |
| `voltaire-effect-schemas` | Branded types, Effect Schema validation, ParseError handling |
| `voltaire-effect-services` | Provider, Signer, Transport services, layer composition, multicall |
| `voltaire-effect-error-handling` | Typed errors, catchTag patterns, Either for partial failures, retry/timeout |
| `voltaire-effect-crypto` | Keccak256, Secp256k1, BLS, AES-GCM, HDWallet, BIP-39, CryptoLive/Test |
| `voltaire-effect-contracts` | Contract factory, type-safe read/write/simulate, events, multicall batching |
| `voltaire-effect-testing` | TestTransport, CryptoTest, layer swapping, mock patterns |
| `voltaire-effect-streaming` | Block/event streaming, reorg detection, WebSocket subscriptions |

## Installation

```bash
# Claude Code
/plugin install voltaire-effect@cyotee
```

## About voltaire-effect

voltaire-effect integrates Voltaire Ethereum primitives with Effect.ts, providing:
- **Typed errors** visible in function signatures (not hidden exceptions)
- **Service dependency injection** via Effect layers (swap production for test)
- **Composable workflows** with retry, timeout, and fallback
- **150+ Effect Schema wrappers** for Ethereum data types
- **WASM-compiled crypto** (9.2x faster keccak256 vs viem)

Requirements: Effect 3.x, Voltaire 0.x, TypeScript 5.4+

```bash
pnpm add voltaire-effect @tevm/voltaire effect
```

## License

MIT
