# MetaPathways-Bookkeeping
For Filecoin Allocator
Take record of all the DataCap allocated to client   **updated 2025/9/1**
- **Pathway description**         

The MetaPathways-Bookkeeping allocator operates as a structured mechanism for managing Filecoin DataCap allocations, specifically focused on processing for the Fil+ ecosystem. It supports clients across diverse industries—including digital marketing, and other enterprise use cases—to onboard datasets onto the Filecoin network.

- **Contact information**

Github: @Destore2023
Slack: @Eric
Email: eric@bingta.net

- **Allocation policy**

Allocation will be 1st-5%,2nd-10%, 3rd-15%, 4th-20%, 5th-25%

On-Chain Requirements: Clients must provide a unique, existing Filecoin on-chain address  for Datacap delivery.

- **Risk mitigation approach**
1. Tracks total requested Datacap per application and validates alignment with dataset size and replica needs (e.g., 10PiB total for a 1.56PiB dataset with 6 replicas).
2. Requires clients to pre-list at least 3-5 unique SP IDs and their locations (e.g., f01234 in Singapore , f06789 in Hongkong) in applications, enabling future verification against Fil+’s ≤30% per SP rule.
3. Mandates written confirmation in applications that clients will engage ≥3 SPs, with non-compliance risking active status revocation  (tracked via [github bookkeeping](https://github.com/Destore2023/2024_DataCap_Bookkeeping)).
4. Validates on-chain addresses to ensure they exist on the Filecoin network (per application template instructions) and are not reused across multiple applications.
5. Verifies dataset legitimacy via sample submissions and source transparency ("My Own Storage Infra").

- **Dispute resolution process**
1. Dispute Filing: Clients, SPs file disputes via GitHub Issues in the MetaPathways-Bookkeeping repository, with clear documentation (e.g., on-chain transaction IDs, SP engagement records, application links).
2. Initial Review: The allocator (Destore2023) acknowledges the dispute within 3 business days and requests additional evidence if needed (e.g., client-SP deal records, dataset retrieval logs).
3. Verification: Cross-references dispute claims with application data , on-chain records  and Fil+ guidelines.
4. Decision & Communication: A written decision is published as a comment on the dispute issue within 7 business days, including:
    - Rationale (e.g., "Datacap denial upheld due to missing SP list").
    - Remediation steps (e.g., "Client must submit updated SP IDs to reactivate allocation").
5. Appeal:  Clients, SPs may appeal to Fil+ governance (via official Fil+ forums) if unsatisfied with the allocator’s decision, providing the dispute issue link for transparency.

- **Audit plan**
1. Review GitHub Actions logs to confirm automation (issue-to-PR conversion, PR updates) functions as intended.
2. Governance Sync: Share audit reports with Fil+ governance via official channels GitHub to align with ecosystem standards.
