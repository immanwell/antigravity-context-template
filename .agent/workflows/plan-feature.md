---
name: Generate Feature PRP
command: /plan-feature [FEATURE_NAME]
---
**GOAL:** Generate a structured Product Requirements Plan (PRP) for a new feature.
1.  READ `memory-bank/systemPatterns.md` for architectural constraints.
2.  ASK the user: "Please provide a brief description and any relevant API documentation for the feature: $[FEATURE\_NAME]."
3.  GENERATE a detailed Implementation Plan artifact including: Data Model changes, File Modification List, and a Step-by-Step Task List.
4.  APPEND the generated plan to `memory-bank/activeContext.md` under a "PROPOSED PLAN" header.
5.  NOTIFY the user the plan is ready for review.
