# Testing results

## Initial dashboard snapshot

The initial AdGuard Home dashboard showed the following values:

| Measure | Recorded value |
| --- | ---: |
| Queries | 827 |
| Blocked queries | 352 |
| Blocked share | 43% |
| Average processing time | 4 ms |

The date, time, and measurement window were not captured. These are point-in-time dashboard values, not ongoing monitoring results. The 43% figure is the value shown on the dashboard; it should not be read as a measured block rate for every device, site, or time period.

## Configuration recorded alongside the snapshot

- AdGuard Home version: **v0.107.79**
- Enabled filters: **AdGuard DNS Filter** and **HaGeZi Multi Normal**
- AdGuard server: **192.168.1.90**
- Router: **Vodafone Power Hub**, **192.168.1.1**
- Other devices currently use DNS forwarded by the router.
- Windows client address recorded in the project: **192.168.1.18**

## Evidence limits

No individual query-log entries, DNS lookup transcripts, before-and-after comparison, or client-by-client test outcomes were included in the recorded facts used for this document. The dashboard snapshot confirms that AdGuard Home displayed query and blocking activity at that point; it does not independently verify which domains were blocked or whether all clients used this DNS path.

## Future test records

When further checks are performed, record the date and time, client used, resolver queried, test domain, observed response, and matching AdGuard Home query-log result. Do not add a result until it has been observed.

