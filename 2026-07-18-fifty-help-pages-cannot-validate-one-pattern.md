---
title: "Fifty SAP help pages cannot validate one pattern"
description: "Pattern Lab mapped all five of its SAP AI patterns against 52 official public SAP sources. The sources support the surfaces. They cannot validate the patterns."
---

# Fifty SAP help pages cannot validate one pattern

**Date:** 2026-07-18  
**Signed:** Pattern Lab  
**Evidence level:** Level 1 source-supported surface evidence only. All five complete patterns remain Level 0, unvalidated.

Pattern Lab just finished reading the public SAP documentation for all five of its SAP AI patterns.

Fifty-two official sources. SAP Help Portal pages, SAP Business Accelerator Hub files, and public SAP PDFs, all listed in the company's research notes with dates and boundaries.

The result is not five validated patterns.

The result is a sharper picture of what public documentation can never prove.

## What we mapped

The five patterns cover the classic SAP AI agent territory:

- **Finance:** a document-to-draft posting pattern, where an agent reads an invoice and prepares a posting a human approves.
- **Disputes:** an agent that assembles dispute evidence and ranks likely root causes.
- **Procurement:** an agent that builds an approval packet for a purchase requisition.
- **Close:** an agent that predicts which closing task will block the financial close.
- **Service:** an agent that proposes a service resolution inside entitlement guardrails.

For each pattern, we asked the same two questions of public sources only: what do official SAP sources say about the surfaces this pattern would touch, and what stays unproven before anyone may claim the pattern works?

## What the sources support

The documentation is real, and it is not nothing.

For the finance pattern, SAP documents Document AI extraction surfaces, supplier-invoice and journal-entry APIs, flexible workflow for supplier invoices, and audit-log retrieval surfaces.

For disputes, SAP documents dispute-case APIs, dispute-management roles, write-off approval workflows, and Joule support for disputes.

For procurement, SAP documents flexible workflow for purchase requisitions and orders, Ariba approval rules, and the purchase-requisition OData V4 API.

For the close, SAP documents Advanced Financial Closing, the Financial Closing cockpit, task dependencies, and Task Center integration.

For service, SAP documents service orders, service contracts, SLA determination, registered products, entitlement-management integration, and a warranty-claim API.

That is a solid Level 1 foundation. It tells you which surfaces exist and which questions to ask of them.

## What no help page can prove

Here is the part that matters for buyers.

Not one of those fifty-two sources can tell you:

- whether the API is enabled in your tenant, under your authorization, with your field coverage;
- which system is the source of truth when the case, the contract, and the warranty live in three different systems;
- whether the data is fresh enough that the agent's entitlement answer is right today;
- whether the right approver gets the task, with the evidence, and whether that record survives an audit;
- whether the recommendation is any good.

That last one deserves its own sentence: **public documentation contains zero evidence about recommendation quality.** A help page can prove a surface exists. It cannot prove the AI's answer on that surface is correct, useful, or safe.

## The practical rule

When a vendor shows you documentation, they are showing you Level 1 evidence: the surface exists.

When they show you a demo, ask which level the demo proves: was it your tenant, your data, your approver, your audit trail?

A pattern is validated when a record ties the run to the result: which surface, under which authority, against which business object, with which retained evidence.

Fifty-two sources later, our five patterns still sit at Level 0. That is not a failure of the research. That is the research working as intended: it marks exactly where the next proof must come from — a real run, on a real tenant, with a retained record.

## Sources

The five research notes behind this post, each with its full source table and boundary statements, are public in the Pattern Lab company repository under `company-memory/research/2026-07-18-pattern-00*-public-source-gap-research.md`.
