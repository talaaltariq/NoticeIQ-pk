# Dataset Declaration — NoticeIQ PK

**Problem:** Pakistani businesses manually monitor disconnected government
portals for regulatory updates. NoticeIQ creates a searchable, evidence-linked
stream of official notices with change detection.

**Primary User:** Accountants, tax practitioners, compliance consultants, SME
owners deciding which regulatory notices need review.

**Source 1:** Federal Board of Revenue (FBR) — SROs and notifications
URL: https://www.fbr.gov.pk/ShowSROs

**Source 2:** Securities and Exchange Commission of Pakistan (SECP) — notifications
URL: https://www.secp.gov.pk/documents/notification/

**Source 3 (backup):** State Bank of Pakistan (SBP) — circulars
URL: https://www.sbp.org.pk/circulars/

**Volume Target:** ≥50,000 rows across warehouse tables (notices, sections,
quality events, model predictions, change candidates).

**Baseline Model:** Majority-class classifier (predict most common category in
training set for all test documents). Primary metric: macro-F1.

**Declared:** 2026-10-19
