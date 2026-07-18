---
title: "Four records to demand before you buy an SAP AI agent story"
description: "Every SAP AI agent demo crosses the same four handoffs. Each one has a record. Ask for all four before you believe the story."
---

# Four records to demand before you buy an SAP AI agent story

**Date:** 2026-07-18  
**Signed:** Pattern Lab  
**Evidence level:** Level 1 — built only on documented, public SAP surfaces. No tenant test, no production claim, no vendor endorsement.

Here is a habit worth stealing.

The next time someone shows you an SAP AI agent — a finance posting assistant, a dispute copilot, a close orchestrator, a service resolution helper — do not ask what the model can do. Ask for four records. One for each handoff the agent has to cross before it changes anything in your SAP system.

## The four records

**1. The action record.** Which exact SAP surface does the agent act on? Not "SAP" — the named object. A journal-entry API. A dispute case. A workflow task. A service order. If the demo cannot name the surface, the agent is a chatbot with a SAP backdrop.

**2. The authorization record.** Under whose identity does the agent read, and under whose identity does it write? In a governed setup these are not the same identity, and there is a record that shows which permissions the acting identity actually held. If the answer is "it uses my login," you are looking at an ungoverned script wearing an AI badge.

**3. The approval record.** Before anything posts, writes back, or touches a customer, a named human decided — and there is a durable record of that decision, attached to the exact payload they approved. "The workflow handles approvals" is not a record. The record is: this person, this payload, this timestamp, this decision.

**4. The business-result record.** After the agent acted, which SAP object changed, and where is the log that proves it? If the story ends at "the AI recommended," nothing happened yet. Recommendations are free. Changed business objects are the bill.

## Why this works

These four records are not our invention. Each one lines up with a surface SAP documents publicly: extraction and finance APIs, workflow and approval tasks, audit-log retrieval, entitlement and service objects. The surfaces exist. The question is whether the agent story in front of you can produce all four records for *its* path through *your* tenant.

A vendor or integrator who can show all four is selling you a system. One who cannot is selling you a demo.

## The one-line version

Before you believe an SAP AI agent story, ask: **which record proves the agent ran, which proves it was allowed, which proves a human approved, and which proves the business object changed?**

If one of the four is missing, that is where your risk lives.

---

*What this post is not: it is not a validated implementation, a tenant test, or a claim that any specific SAP product passes or fails these four checks. It is a buyer's question set, built from public SAP documentation. Pattern Lab's own five patterns are held to the same bar — and today, none of them can produce all four records on a live tenant either.*
