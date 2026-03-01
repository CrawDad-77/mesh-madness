What This Covers
	•	IP Passthrough configuration (single NAT architecture)
  •	Wi-Fi extender replacement with true mesh topology
	•	5 GHz optimization (80 MHz channel width)
	•	Roaming behavior correction
	•	QoS configuration using real-world throughput measurements
	•	Latency-focused performance validation

###############################################################

Topology (Post-Optimization)

                 ┌──────────────────────────┐
Fiber → ONT →    │  AT&T BGW320 Gateway     │
                 │  (IP Passthrough + Wi-Fi │
                 │   radios disabled)       │
                 └───────────┬──────────────┘
                             │ Ethernet
                             ▼
                 ┌──────────────────────────┐
                 │  Deco Node #1 (Upstairs) │
                 │  Primary Router + DHCP   │
                 └───────────┬──────────────┘
                             │ 5 GHz Mesh Backhaul
                             ▼
                 ┌──────────────────────────┐
                 │  Deco Node #2 (Downstairs│
                 │  Coverage Node           │
                 └───────────┬──────────────┘
                             │ 5 GHz Client
                             ▼
                 ┌──────────────────────────┐
                 │  Fire TV (Amazon Luna)   │
                 │  High Priority (QoS)     │
                 └──────────────────────────┘
