# Trustskill — Portal Submission

Category: Builder → Intelligent Contracts

One-liner: Consensus-reviewed admission of immutable agent skills against onchain capability and domain policies.

Description: Trustskill is a reusable GenLayer contract primitive for reviewing agent skills before installation. A policy owner records allowed runtime capabilities, exact outbound domains, and prohibited behavior. A reviewer submits a full-commit GitHub URL for a manifest containing SKILL.md and up to four additional files with exact SHA-256 digests. Validators fetch and hash the same locked bytes independently, inspect capabilities and missing references, and compare the substance of their policy judgments. The contract stores a nonce-bound ALLOW, REVIEW, BLOCK, or INSUFFICIENT_EVIDENCE receipt, including file hashes and specific findings. It fails closed on missing or tampered evidence and prevents nonce replay. ALLOW is a review aid, not a sandbox, authorization, or proof that unlisted runtime dependencies are safe.

Public repository: https://github.com/Dark-Brain07/trustskill

StudioNet contract link: [https://explorer-studio.genlayer.com/address/0x577f37261B082C4cC460354c223961cD72655225](https://explorer-studio.genlayer.com/address/0x577f37261B082C4cC460354c223961cD72655225)

Deployment Transaction: [https://explorer-studio.genlayer.com/transactions/0x18bb43ca4703baafd325fd5e2868472d8d3d8b9decc6839a3d6088b848d55029](https://explorer-studio.genlayer.com/transactions/0x18bb43ca4703baafd325fd5e2868472d8d3d8b9decc6839a3d6088b848d55029)

Reviewer verification: Open the StudioNet contract, call `get_counts`, then `get_policy("1")` and `get_review("1")`.
