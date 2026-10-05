t1_bug_report (1/1) — Correctly withheld the tool call and asked for missing environment/steps instead of guessing. Confirms the "don't infer missing fields" fix is working.

t2_faq_return_policy (1/1) — Answer matches FAQ almost verbatim; reasoning trace shows it quoted the FAQ rather than using general knowledge.

t3_faq_shipping (1/1) — Accurate, FAQ-attributed.

t4_faq_not_covered (1/1, flag) — Correct hand-off text, but the reasoning says "FAQ document could not be accessed due to an error" — it got the right answer for the wrong reason (a retrieval failure, not a scope judgment).

t5_other_request (1/1) — Exact redirect text, correctly classified as OTHER.

t6_bug_report_detailed — missing from this results set. Confirm output_eval_dataset.jsonl has all 6 lines and re-run the eval job if it was dropped — this is your only full-tool-call test, and the rubric needs it covered.