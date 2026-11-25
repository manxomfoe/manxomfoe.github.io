---
layout: default
title: "Case Study: Automating Figma AI Credit Triage"
---

# Automating Figma AI Credit Triage via Admin Email Workflows

Reading Time: **2 minutes**

<details markdown="1">
  <summary>Overview</summary>

<br>

> Docusign transformed how it handled Figma AI credit requests by replacing a sluggish, manual email process with an **intelligent triage system**. The case study outlines the original hurdles of unpredictable costs and constant back-and-forth communication, leading to the establishment of clear objectives focused on **speed, cost-efficiency, and automation**. To solve this, the author leveraged Gemini Studio alongside webhooks and Confluence to automate **email parsing, offer calendar-aware spending advice, and integrate smoothly into existing platforms like Jira and Slack**. Ultimately, this workflow successfully **balanced financial oversight with creative momentum**, ensuring credit approvals remained fast, traceable, and aligned with actual project needs.

</details>

---
# _Case Study_

## The Problem

Managing Figma AI token allocations at Docusign meant balancing active design and prototyping demand against billing groups, credit pricing and model math, and governance with DTS and Finance. Users rarely checked their remaining credit balance proactively, so running low or out triggered ad-hoc back-and-forth threads to establish what they needed the tokens for, how much they required, and which project, team, or pillar should own the request. The exact follow-up questions shifted depending on where the request landed in the monthly cycle, and final sizing still required a human decision grounded in the account's live credit balance.

## Goals

* **Avoid delays:** Respond quickly enough to match the pace of active AI work rather than stalling momentum in manual threads.
* **Actively manage costs:** Prompt requesters to wait when the monthly reset was only two days away instead of burning extra credits unnecessarily.
* **Automate the mundane:** Offload repetitive, rote triage steps to an agent-like workflow while keeping human judgment on final allocation decisions.

## Solution

### _Gemini Studio Triage & Webhook Enabled Workflows_

I used **Gemini Studio** to respond to system-generated emails arriving at Figma admins, turning a manual, inconsistent intake loop into a connected, agent-accelerated workflow:

- **Automated email triage:** Parsed incoming admin system emails to identify token and credit requests and structure the missing context—what the credits were needed for, how much was requested, and which project, team, or pillar applied.
- **Calendar-aware cost nudges:** Factored in proximity to the monthly reset—such as nudging users to wait when reset was two days away—to curb unnecessary mid-cycle spend while keeping urgent work moving.
- **Webhooks into existing tools (Jira & Slack):** Connected Gemini Studio to Jira and Slack via webhooks so triage and follow-ups met requesters and admins where they already worked instead of trapping decisions in email threads.
- **Lightweight traceability via forms and spreadsheets:** Used forms and spreadsheets to keep lightweight, auditable tracking of requests and agent activity without heavy overhead.
- **Visible instructions in Confluence:** Maintained the detailed agent rules and operating instructions in Confluence, a shared, accessible space the team already used—keeping operational knowledge visible and searchable.

## Operational Fit & Impact

This workflow fit directly into my DesignOps and tooling governance work at Docusign by pairing Figma governance, credit spend analysis, and billing oversight with practical automations that reduced routine manual effort. It kept credit decisions tied to real project context and account balances, protected inefficient spending around monthly reset boundaries, and maintained lightweight traceability without slowing down AI prototyping.
