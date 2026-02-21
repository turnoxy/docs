# Documentation TODO

Features and documentation items to add.

## SOCKS5 Protocol

SOCKS5 is now supported on port 1318 (same port, auto-detected by ProtocolDetector). Documentation needs updating.

**Endpoint**: `gate.turnoxy.com:1318` (shared with HTTP/HTTPS)

**Example**:
```bash
curl -x "socks5://sub_xxx:pass@gate.turnoxy.com:1318" https://example.com
```

**Files to update**:
- `proxies/connection.mdx` - Add SOCKS5 endpoint and Protocol Comparison table
- `examples/curl.mdx` - Add SOCKS5 example

---

## Pool Parameter (Archived)

> **Decision (2026-02)**: Pool is now bound at subscription level via `subscriptions.poolId`, not as a user parameter in the proxy username. The `pool` parameter is still parsed by the proxy for backwards compatibility but is **not used for routing**.

This TODO item is no longer applicable. Users select their pool type (res/dc/isp/mob) when creating a subscription, not per-request.
