# Lessons Learned

1. **Verify the pipeline before trusting silence.** During a multi-hour quiet window I tested port reachability, made my own failed logins, and checked overall event volume. That turned "maybe it's broken" into "it works, nobody's attacking right now."
2. **Exposure gets noticed fast.** Automated scanners found and hammered an open RDP port within hours.
3. **Know your tooling's defaults.** Incidents existed but were hidden by a default Defender portal filter.
4. **Geo-IP ≠ attacker location.** It shows where the infrastructure is hosted, often a VPS or a compromised host.
5. **Documentation is part of the work.** I captured results but not every config step. Next time I'll screenshot each step as I go and keep a running notes file with timestamps.
6. **Watch cloud costs.** "Stop (deallocate)" is different from shutting down inside the OS, and storage and log ingestion still cost money until resources are deleted.
