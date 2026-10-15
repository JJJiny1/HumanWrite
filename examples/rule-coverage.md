# Rule coverage and validation status

This map connects writing-quality checks to skill instructions and behavioral scenarios. Coverage means explicit instructions exist; it does not establish stable model behavior.

| # | Writing-quality check | Instruction location | Behavioral scenario |
|---|---|---|---|
| 1 | Excessively long, nested sentences | ai-writing-patterns: Sentence load | N1 |
| 2 | Uniform paragraph lengths | ai-writing-patterns: Whole-text rhythm | N2 |
| 3 | Excessive dashes, colons, semicolons, parentheses | ai-writing-patterns: Punctuation | N3 |
| 4 | Padded lists of three | ai-writing-patterns: Parallelism | N1, N3 |
| 5 | Vague claims without examples | ai-writing-patterns: Specificity | N1, N2 |
| 6 | Stock phrases and ornamental vocabulary | ai-writing-patterns: Vocabulary | N1 |
| 7 | Inconsistent key concepts | academic-writing: Terminology | N4 |
| 8 | Circular, superficially complete arguments | academic-writing: Substantive argument | N2, N10 |
| 9 | Inappropriate language level | ai-writing-patterns; personal-writing-profile | N1, N11 |
| 10 | Repeated negation and mirrored structures | ai-writing-patterns: Parallelism | N1, N12 |
| 11 | Repeated paragraph development | ai-writing-patterns: Whole-text rhythm | N2 |
| 12 | Sources do not support claims | academic-writing: Sources; essay-consistency | N5 |
| 13 | Mechanical narration of table cells | academic-writing: Empirical results | N6 |
| 14 | Invented explanations for non-significance | academic-writing: Empirical results | N6 |
| 15 | Generic reflection without an episode | reflection-writing: Develop reflection | N7, N8 |
| 16 | Missing authentic thought and self-criticism | reflection-writing: Develop reflection | N7, N8 |
| 17 | Theory added without a concrete connection | academic-writing; reflection-writing: Theory | N7 |
| 18 | Slogan-like conclusions | academic-writing: Conclusions; reflection-writing: Action | N7, N10 |

Additional concerns: source overlap and the limits of an eight-character threshold appear in academic-writing and chinese-writing (N5, N9). Repetitive defensive caveats appear in ai-writing-patterns and academic-writing (N6). Natural drafting is routed before composition in SKILL.md (N12). Existing intent, profile, and contradiction scenarios remain in acceptance-scenarios.md.

All reference paths in this table refer to files under skills/humanwrite/references/. Existing essay-consistency.md is preserved without modification. Instructions do not guarantee automatic host invocation; see README for discovery limits.

## Validation record

Version 0.2.0: frontmatter, YAML metadata, relative links, unchanged essay-consistency resource, and archive contents receive local structural checks. The natural-writing scenarios are supplied for manual execution; they have not received an independent model behavior evaluation in this release.
