# Screening Records

Individual screening records for each screen performed. One file per screen, named using the screen ID from the relevant log.

Records containing PII (passport numbers, addresses, identification details) are maintained in secure storage and referenced by URL in the evidence field of each record file.

## Directory Structure

```
records/
├── donors/       # Individual donor screening records (SCR-YYYY-NNNN.md)
├── vendors/      # Individual vendor screening records
└── grantees/     # Individual grantee and partner screening records
```

## File Naming

```
SCR-YYYY-NNNN.md
```

Matches the Screen ID in the corresponding screening log row.

## Related

- [Donor Screening Log](../logs/donor-screening-log.md)
- [Vendor Screening Log](../logs/vendor-screening-log.md)
- [Grantee Screening Log](../logs/grantee-screening-log.md)
- [Exception Log](../exceptions/exception-log.md)
