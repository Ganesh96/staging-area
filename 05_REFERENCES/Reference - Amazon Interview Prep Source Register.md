---
id: ref-20260504-amazon-source-register
type: reference
status: reference
created: 2026-05-04
updated: 2026-05-04
source_type: mixed
source_link: ""
source_path: "01_STAGING/01_LONG_FORM/STUDY_MATERIAL/Amazon"
tags: [#status/reference, #domain/job-search]
---
# Reference - Amazon Interview Prep Source Register

## Inventory and triage matrix
| File path | Type | Content role | Status | Reason | Extraction priority | Downstream notes |
|---|---|---|---|---|---|---|
| Amazon SDE Prep Guide.md | md | core prep scaffold | core | concise prep structure | high | Amazon project, Amazon prep stack |
| Final Plan.md | md | integrated plan | core | actionable schedule and focus areas | high | Amazon project, technical register |
| Ultimate Software Engineer Interview Prep Plan.md | md | broad prep architecture | supporting | overlaps with Final Plan, still useful | medium | Amazon prep stack |
| study plans.md | md | planning variants | supporting | schedule alternatives | medium | Amazon project |
| amazon 6  month.md | md | long-horizon planning | supporting | timeline/constraint source | medium | Amazon project |
| Monday Quick.md | md | short-cycle execution | supporting | quick sprint structure | medium | Amazon project |
| constraint.md | md | prep constraints | supporting | boundary conditions and limits | medium | Amazon project |
| LeetCode Problem List for Interview Preparation.md | md | coding backlog | core | explicit coding inventory | high | technical topics register |
| Amazon LPs Prep.docx | docx | LP behavioral examples | core | readable STAR-style behavioral content | high | LP behavioral mapping model |
| SDE2 PS prep document -2023.docx | docx | phone-screen scoring rubric | core | readable competency rubric | high | Amazon prep stack, technical register |
| SDE Amazon.docx | docx | behavioral + project examples | supporting | readable but narrower | medium | LP behavioral mapping model |
| Chime Instructions.docx | docx | logistics | low-signal | operational setup, not prep content | low | none |
| LPs.md | md | empty placeholder | superseded | zero content | none | none |
| Ace Amazon SDE - 1.pdf | pdf | potential prep deck | unreadable | text extraction unavailable in environment | needs-review | none |
| Ace Amazon SDE - 2.pdf | pdf | potential prep deck | unreadable | text extraction unavailable in environment | needs-review | none |
| Amazon LPs Prep.pdf | pdf | LP material duplicate candidate | duplicate | mirrors LPs Prep source family | low | none |
| Amazon SDE Interview Prep.pdf | pdf | prep guide | unreadable | text extraction unavailable in environment | needs-review | none |
| Amazon SDE prep.pdf | pdf | prep guide | unreadable | text extraction unavailable in environment | needs-review | none |
| Amazon Systems Design Preparation.pdf | pdf | system design guide | unreadable | text extraction unavailable in environment | needs-review | none |
| Candidate Phone Interview Prep.pdf | pdf | phone screen guide | unreadable | text extraction unavailable in environment | needs-review | none |
| Fortify-Experts-Behavioral-Questions-Based-on-Amazon-Principles.pdf | pdf | behavioral bank | unreadable | text extraction unavailable in environment | needs-review | none |
| Gmail - SDE Prep Docs.pdf | pdf | exported prep notes | unreadable | image-heavy/metadata-only extraction | needs-review | none |
| Medium - Behavioral Interview Questions.pdf | pdf | behavioral bank | duplicate | exact duplicate exists in `Amazon/pdfs/` | low | none |
| SDE Interview Prep Guide 1.pdf | pdf | prep guide | unreadable | text extraction unavailable in environment | needs-review | none |
| SDE Interview Prep Guide 2.pdf | pdf | prep guide | unreadable | text extraction unavailable in environment | needs-review | none |
| SDE Interview Prep Guide 3.pdf | pdf | prep guide | unreadable | text extraction unavailable in environment | needs-review | none |
| SDE Onsite Competency Prep Guide.pdf | pdf | onsite competency guide | unreadable | text extraction unavailable in environment | needs-review | none |
| SDE+II+Phone+Screen+Prep+Guide.pdf | pdf | phone screen guide | unreadable | text extraction unavailable in environment | needs-review | none |
| STAR Leadership Principals.pdf | pdf | LP/STAR content | unreadable | text extraction unavailable in environment | needs-review | none |
| pdfs/12 Week Programme - Leetcode.pdf | pdf | coding plan | unreadable | text extraction unavailable in environment | needs-review | none |
| pdfs/ASP NET MVC.pdf | pdf | unrelated tech stack doc | excluded | not Amazon interview-specific | none | none |
| pdfs/Competitive Programmer’s Handbook.pdf | pdf | generic CP book | excluded | broad reference, not Amazon-specific | none | none |
| pdfs/Design Pattern.pdf | pdf | generic design ref | supporting | useful technical support | low | technical topics register |
| pdfs/Java .pdf | pdf | generic language notes | excluded | broad language reference | none | none |
| pdfs/Java Backend Developer Interview Questions .pdf | pdf | generic backend questions | supporting | relevant but non-Amazon-specific | low | technical topics register |
| pdfs/LeetCode Notes.docx | docx | coding notes | supporting | readable and coding-relevant | medium | technical topics register |
| pdfs/Leetcode Quick.pdf | pdf | coding quick list | unreadable | extraction unavailable | needs-review | none |
| pdfs/Medium - Behavioral Interview Questions.pdf | pdf | behavioral bank | duplicate | exact duplicate of root PDF | low | none |
| pdfs/RabbitMQ_vs_Kafka_vs_ActiveMQ_Comparison_Guide.pdf | pdf | system design support | supporting | relevant distributed systems theme | low | technical topics register |
| pdfs/RedisUsecases.pdf | pdf | system design support | supporting | relevant caching/data-store theme | low | technical topics register |
| pdfs/authentication_features_guide.pdf | pdf | system design support | supporting | security/auth topic relevance | low | technical topics register |
| pdfs/Youtube - recommendation engine.docx | docx | system design case notes | supporting | readable design-oriented content | medium | technical topics register |
| pdfs/recommendation engine  - Key Components.docx | docx | system design architecture notes | supporting | readable components summary | medium | technical topics register |
| pdfs/recommendation engine - Question.docx | docx | system design Q&A | supporting | readable interview framing | medium | technical topics register |

## Notes
- Multiple PDFs are classified `unreadable` due current environment extraction limits; marked `needs-review` rather than guessed.
- Behavioral PDF duplicate detected (`Medium - Behavioral Interview Questions.pdf` in two locations).
- `LPs.md` is empty and treated as superseded by richer LP sources.

## High-priority PDF resolution (2026-05-04 follow-up)
| File path | Status | Extraction result | Reason | Downstream output affected | Manual review |
|---|---|---|---|---|---|
| SDE+II+Phone+Screen+Prep+Guide.pdf | needs-manual-review | no reliable text extracted | PDF extraction tooling unavailable in environment (`pdftotext`, `pdfinfo`, PyPDF libs missing) | Project, Amazon prep stack | yes |
| SDE Onsite Competency Prep Guide.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | Project, Amazon prep stack | yes |
| Candidate Phone Interview Prep.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | Project | yes |
| Amazon Systems Design Preparation.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | System Design atomic, technical register | yes |
| STAR Leadership Principals.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | LP behavioral mapping model | yes |
| Fortify-Experts-Behavioral-Questions-Based-on-Amazon-Principles.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | LP behavioral mapping model | yes |
| Amazon SDE Interview Prep.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | Project, MOC | yes |
| Amazon SDE prep.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | Project, MOC | yes |
| SDE Interview Prep Guide 1.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | Project, technical register | yes |
| SDE Interview Prep Guide 2.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | Project, technical register | yes |
| SDE Interview Prep Guide 3.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | Project, technical register | yes |
| pdfs/12 Week Programme - Leetcode.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | technical register | yes |
| pdfs/Leetcode Quick.pdf | needs-manual-review | no reliable text extracted | same tooling limitation | technical register | yes |

