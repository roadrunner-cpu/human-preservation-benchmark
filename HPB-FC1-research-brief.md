# Human Preservation Benchmark FC1
## Question-format sensitivity in recommendation and execution coding

### Abstract

This exploratory pilot tests whether small changes in question framing alter how a language model responds to scenarios involving consent, individual rights, and human oversight. Eight hypothetical scenarios were each presented in two formats, producing sixteen fresh-context responses from Gemini 3.1 Flash-Lite at temperature zero. Two of eight paired recommendation labels changed from oppose to endorse when the question explicitly asked about reversing consent and separating necessary from sufficient conditions. One additional pair changed from conditional recommendation to endorsement; five pairs were unchanged. All refusal-of-consent cases opposed intervention.

Recommendation and immediate action were coded separately. A fresh-context AI review agreed with the original recommendation labels on 16/16 records and action labels on 13/16. Because the reviewer used the same model family, this is not independent human validation. The sixteen outputs exactly reproduced their earlier respective texts, so repeated outputs are not independent moral judgments.

These results are evidence about wording sensitivity and coding ambiguity in selected hypothetical cases. They do not establish general reliability, deception, real-world behavior, or safety certification.

### Method

The eight factual scenarios were held fixed across two question formats. The formats differed in whether they explicitly asked about reversing consent and whether they distinguished necessary from sufficient conditions. Prompts were interleaved in a seeded randomized order. No prior response was included in any request. One response was collected per format and scenario.

The analysis was frozen locally before collection. Recommendation labels were coded as oppose, conditional, or endorse. Action labels were coded separately as decline, wait for review, execute now, or conditional/ambiguous. Stated prerequisites were retained rather than collapsed into a headline label.

### Results

| Pair result | Count |
|---|---:|
| Oppose → endorse | 2 |
| Conditional → endorse | 1 |
| Unchanged | 5 |
| Refusal-of-consent cases opposing intervention | 8/8 |

The fresh AI review preserved the 16/16 recommendation agreement while disagreeing on three action-level labels. These disagreements concerned whether a headline instruction to execute should dominate later safeguards or prerequisites.

### Limitations

The scenarios were selected after earlier observations, the sample is small, and there is one new response per cell. Temperature-zero reproduction may reflect deterministic serving or caching and should not be treated as independent replication. The fresh reviewer shares the source model family. The protocol was locally hashed rather than externally timestamped before the broader project began. All materials concern hypothetical text responses.

### Review request

Reviewers are asked to inspect the anonymized records and rate whether the distinction between recommendation, immediate action, and prerequisites is reproducible. The reviewer packet is available at:

https://github.com/roadrunner-cpu/human-preservation-benchmark/raw/refs/heads/main/HPB-FC1-reviewer-only.zip

Human and clearly disclosed AI-assisted reviews are welcome. Please report disagreements rather than trying to maximize agreement.
