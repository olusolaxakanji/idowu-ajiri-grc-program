# Templates

Blank, version-controlled templates for every document type in this GRC program. Always copy a template when creating a new record rather than building from scratch — this ensures consistency and that no required fields are accidentally omitted.

## Available Templates

| Template file | Used for | Current version |
|---|---|---|
| `control-record-v1.md` | New control entries in `controls/` | v1 |
| `risk-entry-v1.md` | New risk entries in `risk-register/` | v1 |
| `policy-v1.md` | New policy documents in `policies/` | v1 |
| `evidence-record-v1.md` | New evidence files in `evidence/` | v1 |
| `screening-record-v1.md` | Individual screening records in `screening/records/` | v1 |
| `screening-log-v1.md` | Running screening logs in `screening/logs/` | v1 |
| `board-report-v1.md` | Quarterly board compliance reports in `reports/board/` | v1 |
| `exception-record-v1.md` | Screening or control exceptions | v1 |

## Versioning

Template filenames include a version suffix (`-v1`, `-v2`, etc.). When a template is updated:

1. The new version is added as a new file (e.g., `policy-v2.md`).
2. The old version is retained so that existing documents that reference it remain valid.
3. The table above is updated to point new documents at the latest version.
4. A note is added to the old template file indicating it has been superseded and naming the replacement.

## How to Use

```
cp templates/policy-v1.md policies/global/POL-GL-006-new-policy.md
```

Then fill in all fields marked `[REQUIRED]`. Fields marked `[OPTIONAL]` may be left blank if not applicable, but do not delete them — leave the label in place so reviewers know the field was considered.
