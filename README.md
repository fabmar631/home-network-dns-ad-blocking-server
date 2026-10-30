# Home Network DNS Ad-Blocking Server

A home-network DNS filtering project built on a Lenovo ThinkCentre M73 running Debian 13 and AdGuard Home. The server provides DNS filtering for devices that use the Vodafone Power Hub's DNS forwarding path.

## Project overview

The aim is to use existing hardware to run a dedicated DNS filtering service and make its activity visible through AdGuard Home. The current setup has two enabled filters: **AdGuard DNS Filter** and **HaGeZi Multi Normal**.

The figures in this repository are a record of the initial dashboard snapshot. They are point-in-time results, not a long-term average or a guarantee that every device or application is filtered.

## Hardware and software

| Component | Recorded details |
| --- | --- |
| Server | Lenovo ThinkCentre M73 |
| Processor | Intel Pentium (exact model not recorded) |
| Memory | 16 GB RAM |
| Storage | 1 TB HDD |
| Operating system | Debian 13 |
| DNS filtering | AdGuard Home v0.107.79 |
| Router | Vodafone Power Hub |
| AdGuard server address | `192.168.1.90` |
| Router address | `192.168.1.1` |
| Windows client address | `192.168.1.18` |

## Current network behavior

Other devices currently use DNS forwarded by the router. This documents the configured route; it does not claim that every device has been individually tested or that every DNS request is blocked. See the [network diagram](network-diagram.md) and [testing results](testing-results.md).

## Initial dashboard snapshot

| Dashboard measure | Initial value |
| --- | ---: |
| Queries | 827 |
| Blocked | 352 |
| Blocked share | 43% |
| Average processing time | 4 ms |

The date, time, and measurement window for this initial snapshot were not recorded. The values should be treated as a baseline only. More context and limitations are in [testing results](testing-results.md).

## Repository contents

- [Network diagram](network-diagram.md) — Mermaid diagram of the documented DNS forwarding path.
- [Testing results](testing-results.md) — recorded dashboard values and what they do and do not establish.
- [Lessons learned](lessons-learned.md) — practical conclusions based on the documented setup and its current evidence.
- [Screenshots](screenshots/) — reserved for sanitized project screenshots. No screenshots were available in the workspace when this repository was prepared.

## Privacy

Only the local network addresses already used in the project documentation are included. Router passwords, Wi-Fi credentials, MAC addresses, serial numbers, public IP addresses, and secrets visible in photographs are intentionally excluded. Review and redact screenshots before adding them.

