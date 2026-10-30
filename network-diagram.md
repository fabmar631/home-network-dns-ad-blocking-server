# Network diagram

This diagram records the current router-forwarded DNS path for other home devices. The Windows client address is documented separately because its exact resolver path was not recorded.

```mermaid
flowchart LR
    Devices["Other home devices"] -->|DNS requests forwarded by router| Router["Vodafone Power Hub<br/>Router: 192.168.1.1"]
    Router -->|DNS forwarding| Server["AdGuard Home<br/>Lenovo ThinkCentre M73<br/>Server: 192.168.1.90"]
    Server --- Filters["Enabled filters<br/>AdGuard DNS Filter<br/>HaGeZi Multi Normal"]
    Client["Windows client<br/>192.168.1.18<br/>DNS route not recorded"]
```

The diagram does not specify an upstream DNS provider because that detail was not recorded. It also does not imply that every device or application has been tested against the filtering server.

