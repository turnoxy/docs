# Documentation TODO

Features temporarily removed from documentation. Add back when supported.

## Pool Parameter

IP pool type selection parameter. Add when multiple pools are available.

**Parameter**: `pool`

**Values**:
| Value | Name | Best For |
|-------|------|----------|
| `res` | Residential | Social media, e-commerce, high anonymity |
| `dc` | Datacenter | High-volume scraping, speed priority |
| `isp` | ISP | Long-term tasks, balanced needs |
| `mob` | Mobile | Mobile simulation, highest security |

**Example**:
```bash
sub_xxx-pool-dc:pass@gate.turnoxy.com:1318
```

**Files to update**:
- `proxies/parameters.mdx` - Add pool section and Quick Reference table
- `examples/curl.mdx` - Add IP Pool Types examples
- `quickstart.mdx` - Add pool examples and Card link
- `authentication/password.mdx` - Update Multiple Parameters example
- `errors.mdx` - Add INVALID_POOL error

---

## SOCKS5 Protocol

SOCKS5 proxy protocol support. Add when SOCKS5 is available.

**Endpoint**: `gate.turnoxy.com:1319`

**Example**:
```bash
curl -x "socks5://sub_xxx:pass@gate.turnoxy.com:1319" https://example.com
```

**Files to update**:
- `proxies/connection.mdx` - Add SOCKS5 endpoint and Protocol Comparison table
- `examples/curl.mdx` - Add SOCKS5 example
