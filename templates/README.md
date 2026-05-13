# Templates

Consistency is the foundation of audit readiness. If every risk entry uses a different field structure, if every screening record captures different data, if every policy is formatted differently: comparing records is harder, aggregating findings is harder, and demonstrating to a regulator that the programme operates systematically becomes much harder.

Templates solve that problem by establishing the required structure before any document is created. Every substantive record in this programme is produced from one of these templates.

---

## Available Templates

| Template | Used for | Version |
|---|---|---|
| `policy-v1.md` | New policy documents in `policies/` | v1 |
| `control-record-v1.md` | New control entries in `controls/` | v1 |
| `risk-entry-v1.md` | New risk entries in `risk-register/` | v1 |
| `evidence-record-v1.md` | New evidence files in `evidence/` | v1 |
| `screening-record-v1.md` | Individual screening records in `screening/records/` | v1 |
| `board-report-v1.md` | Quarterly board compliance reports in `reports/board/` | v1 |
| `exception-record-v1.md` | Screening or control exceptions in `screening/exceptions/` | v1 |

---

## How to Use

Copy the relevant template to the appropriate folder, rename it following the programme naming convention, and fill in all fields marked `[REQUIRED]`. Fields marked `[OPTIONAL]` may be left blank if not applicable, but do not delete the field label: leave it in place so reviewers know it was considered.

```bash
cp templates/policy-v1.md policies/global/POL-GL-006-new-policy.md
```

Remove the template usage notes section at the bottom before publishing or merging to `main`.

---

## Template Versioning

Template filenames include a version suffix (`-v1`, `-v2`). When a template is updated:

1. The new version is added as a new file (e.g., `policy-v2.md`).
2. The old version is retained: existing documents that reference it remain valid.
3. The table above is updated to point new documents to the latest version.
4. A superseded notice is added to the old template file naming the replacement.

Never delete a template version that has existing documents built from it.

---

## Related Documentation

| Document | Description |
|---|---|
| [Policies](../policies/README.md) | Documents produced using `policy-v1.md` |
| [Controls](../controls/README.md) | Records produced using `control-record-v1.md` |
| [Risk Register](../risk-register/README.md) | Entries produced using `risk-entry-v1.md` |
| [Screening](../screening/README.md) | Records produced using `screening-record-v1.md` |
| [Evidence](../evidence/README.md) | Records produced using `evidence-record-v1.md` |
| [Reports](../reports/README.md) | Reports produced using `board-report-v1.md` |
