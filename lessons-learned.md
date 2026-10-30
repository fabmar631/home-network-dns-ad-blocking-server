# Lessons learned

These points are based on the configuration and evidence recorded for this project.

1. **Reuse can provide a dedicated service host.** The DNS filtering service runs on an existing Lenovo ThinkCentre M73 with 16 GB RAM and a 1 TB HDD.
2. **Router forwarding gives the documented devices a central DNS route.** Other devices currently use DNS forwarded by the Vodafone Power Hub to the AdGuard server. This should not be confused with proof that every device follows that route.
3. **A dashboard snapshot needs its measurement window.** The initial values—827 queries, 352 blocked, 43%, and 4 ms—are useful as a baseline, but the date and time were not captured, so they cannot support a time-based comparison.
4. **Service-level counts and client-level checks answer different questions.** The dashboard shows aggregate activity. No individual DNS lookup result or per-device validation outcome was included in the available project record.
5. **Screenshots need a privacy review.** Add images only after checking for router and Wi-Fi credentials, MAC addresses, serial numbers, public IP addresses, and other secrets.

