# SeaFlow V3.6 Five-Arm Exploratory Evaluation — Public Edition

> **Public Edition.** This separately prepared aggregate summary is not the original Chinese Run_001 report. The original remains internal; this file is labeled so it cannot be mistaken for an unmodified source copy.

## Record and provenance

- **Original title:** `SeaFlow V3.6 冻结内部合成探索研究`
- **Public-edition title:** *SeaFlow V3.6 Five-Arm Exploratory Evaluation — Public Edition*
- **Author/byline in original:** Not stated.
- **Version and status:** V3.6, five-arm Run_001; execution sealed, interpretation PARTIAL.
- **Execution/seal date:** 2026-10-23 per the project timeline.
- **Original source path:** `Exam_Field/Active/V3_6/FiveArm_Exploratory_Execution/Run_001/FIVE_ARM_RESEARCH_REPORT.md (private workspace source)`
- **Original source SHA-256:** `6bef44162e168338e31aa00689caa4309d2fd6f8a199fee5ce357acb1d3c0e7f`
- **Public date:** Pending final approval and GitHub publication.
- **Preparation date:** 2026-10-26.

## Scope and findings

This was an internal synthetic five-arm exploratory evaluation comparing the SeaFlow evidence condition E with an independent BM25 downstream baseline among other conditions. It is not an external or third-party benchmark.

Under the report-defined bounded-answer paired outcome, 34 E vs B-downstream pairs were complete and currently judgeable: 0 improvements and 0 degradations; 30 pairs were both acceptable and 4 were both errors. Twelve pairs remain under review and two are incomplete. These results show matching outcomes on that judgeable subset; they do not establish equivalence, a true zero effect, or a general retrieval gain.

The run records 180 model requests, with 178 completed and two truncated at the output limit. Both truncations and all unresolved cases remain part of the finding. In the evaluated configuration E required more input resources and longer cumulative model latency than B-downstream. Exact token and timing totals, provider and route identifiers, item-level examples and execution logs are intentionally omitted from this Public Edition. Actual monetary cost was not exposed.

## Separate owner-reported expert re-review

The project owner reports a later review, separate from Run_001: machine review approved one improvement, and two human experts jointly approved three improvements. This suggests a slight edge among those reviewed cases only. This post-seal note is not part of the original report or its primary paired endpoint; no separate source file, denominator, or protocol record was supplied. It does not establish an overall PASS or replace the sealed result.

## Limits and separation

- The original study used internal synthetic references and provisional internal scoring; it did not have an independent expert gold set. The separate owner-reported review above is not represented as an independent benchmark or validated adjudication protocol.
- V3.6.1 follow-up evidence remains separate, with PARTIAL/HOLD states; neither is an overall PASS.
- The four-arm retriever-governance development experiment is separate and is not combined with Run_001.
- This summary does not establish statistical significance, equivalence, third-party benchmark acceptance, legal correctness, or production readiness.
- No scorecards, raw episode data, model credentials, provider routes, private Core, datasets, execution logs or legal-source full text are included.

No license grant is added by this Public Edition; rights remain with the original author or rights holder.
