# SeaFlow V3.6 vs BM25

## Source record and public edition

- **Original title:** `SeaFlow V3.6 冻结内部合成探索研究` (original Chinese title)
- **English navigation label:** SeaFlow V3.6 vs BM25
- **Author/byline:** Not stated in the original report.
- **Version:** V3.6, five-arm exploratory execution, Run_001; sealed manifest status `HISTORICAL_SEALED_EXECUTION_COMPLETE_INTERPRETATION_PARTIAL`.
- **Execution/seal date:** 2026-10-23, per the project timeline; the run manifest records execution complete with interpretation PARTIAL.
- **Scope:** Internal synthetic exploratory comparison of the real SeaFlow evidence condition E with an independent BM25 downstream baseline, alongside three other conditions. This is not an external or third-party benchmark.
- **Sealed primary paired result:** For E vs B-downstream, 34 pairs were complete and currently judgeable: 0 improvements, 0 degradations, 30 were both acceptable and 4 were both errors; 12 pairs remain under review and 2 are incomplete. The original report preserves all 48 episodes.
- **Execution completeness:** 180 model requests; 178 completed and 2 ended at the output limit. Both truncated responses remain in the record.
- **Resource cost:** E used more input resources and had longer cumulative latency than B-downstream. Exact resource totals are omitted from this Public Edition; actual monetary cost was not exposed.
- **Interpretation:** Internal scoring is provisional and the report's overall interpretation is PARTIAL. It establishes neither statistical significance, equivalence, a zero effect nor an external benchmark pass. Negative findings, reviews, truncations and resource disadvantages are retained.
- **Public date:** 2026-10-26.
- **Preparation date:** 2026-10-26.

## Source and integrity

- **Original source path (private workspace):** `Exam_Field/Active/V3_6/FiveArm_Exploratory_Execution/Run_001/FIVE_ARM_RESEARCH_REPORT.md`
- **Archived file:** [`FIVE_ARM_RESEARCH_REPORT_PUBLIC_EDITION.md`](FIVE_ARM_RESEARCH_REPORT_PUBLIC_EDITION.md)
- **Public-edition SHA-256:** `3fa749a1c799ec37cff66ea9fed88562e0d5e5964201eace530e40f3381eda39`
- **Original source SHA-256 (withheld):** `6bef44162e168338e31aa00689caa4309d2fd6f8a199fee5ce357acb1d3c0e7f`
- **Edition status:** Aggregate English public summary; not an original copy or translation. The sealed Chinese source remains internal pending separate release review.

## Separate owner-reported expert re-review

The project owner reports a later review, separate from Run_001: machine review approved 1 improvement, and two human experts jointly approved 3 improvements. This suggests a slight edge among those reviewed cases only. The note was supplied in the owner’s 2026-10-26 direction; no separate source file, denominator, or protocol record was attached. It does not replace or alter the sealed report’s primary paired result and does not establish an overall PASS.

## Scope boundary

The original episode scorecards and execution logs were checked for consistency but are not included. The four-arm retriever-governance development work is a separate experiment. V3.6.1 follow-up records are also separate; their PARTIAL/HOLD states do not make this V3.6 report an overall PASS. No private Core, source snapshots, credentials, raw datasets or legal-source full text are included.

The original report does not state a separate reuse license. This archive adds no license grant; preserve the original report's attribution and rights.
