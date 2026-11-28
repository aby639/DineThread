# DineThread experimental records

The five directories hold the component studies and the recorded accessibility retest. The integration directory holds the merged-build observations and the later release checks. Each study's results or protocol identifies its build and workload. Compressed JSON, JSONL and text files use gzip. SHA256SUMS lists the checksums of the archived files, including the current study summaries.

| Directory | Evidence |
|---|---|
| [Order recovery](order-recovery/) | November 23 API and browser comparison, CSV, logs and receipts |
| [Catalogue](catalogue/) | Matched rounds, fixture checks, price-confirmation screenshots |
| [Theme preview](theme/) | Correctness, delivery timing and React profiling |
| [Accessibility](accessibility/retest-2026-11-28/) | Bibek Rai’s 28 November keyboard, NVDA Speech Viewer and 200% Chrome zoom recordings, frame excerpts and checksums |
| [Kitchen workflow](workflow/) | History checker, browser observations and read-back-to-screen timings |
| [Integration and release](integration/) | Cross-strand checks, screenshots and native speech observations |

Bibek's three recordings cover one version of the customer menu. The [original team research archive](https://github.com/Talha49/DineThread/tree/cf67404a5663baf844b479f939f4bfc78c45f574/research-records) holds the earlier component studies.

The original implementation commits are [catalogue](https://github.com/Talha49/DineThread/commit/3611db71be54230b8e0892fc756e051331078085), [theme preview](https://github.com/Talha49/DineThread/commit/69149a5079a2e01b95a424c3bd914b4005821353) and [kitchen workflow](https://github.com/Talha49/DineThread/commit/5d4422f57a9b4bdab2c662bc80ac9233453a605e). This branch preserves their original history. The group's application is on main. Earlier protocols in this archive describe the experiments as recorded. Current release protocols are maintained in the application repository.
