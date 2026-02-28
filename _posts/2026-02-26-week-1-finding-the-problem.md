---
title: "Week 1: Cleo & You"
date: 2026-02-27
author: Melanie & Ernest
image: /assets/images/week-1-finding-the-problem.png
---

# Cleo & You

**Your AI Onboarding & Sales Enablement Assistant**
Week 1 Discovery Deliverable • ProductBC Build-a-Thon 2026

---

## 1. Problem Statement

> *Sales and customer-facing teams at growing companies lose weeks of productivity during onboarding and product updates because institutional knowledge lives inside specific people and static documents — not in a system that is always available, interactive, and adaptable to how each person learns.*

This problem was identified through direct experience at two different companies:

| **VoPay (Fintech)** | **Fresh Tracks (Travel)** |
|---|---|
| A fast-growing fintech startup managing multiple high-priority projects simultaneously. Sales onboarding relied on whiteboard sessions and one-on-one demos from a few key people. New hires had access to dozens of documents and SOPs but still couldn't retain product knowledge effectively without live interaction. | A travel company where sales reps engage customers in live phone conversations about travel experiences. Onboarding is slow and dependent on shadowing experienced reps — an approach that does not scale and limits how much new hires can practice before speaking with real customers. |

While the context differs, the root problem is identical: knowledge is locked in people and static documents, and new team members cannot learn, practice, or get answers independently.

---

## 2. User Segments

| **Primary: New Sales Hires** | **Primary: Existing Sales Team** | **Secondary: Sales Managers / Admins** |
|---|---|---|
| Joining a company with complex products or services. Needs to get up to speed fast. Learns best through interaction, not passive reading. Frustrated by waiting for an available trainer. | Preparing for product launches, events, or new service lines. Wants to practice pitch variations without consuming a colleague's time. Needs quick refreshers on product details before calls. | Responsible for keeping knowledge current. Currently the bottleneck for all training. Wants to offload repetitive onboarding tasks and ensure consistency across the team. |

---

## 3. Initial Hypothesis

> *"We believe that new sales hires and existing sales team members at growing companies experience slow ramp-up, inconsistent product knowledge, and lack of independent practice opportunities when onboarding or preparing for product updates, because institutional knowledge is locked inside specific people and static documents that cannot be accessed on-demand, do not adapt to individual learning styles, and do not allow safe, independent practice."*

| **Specific** | **Falsifiable** | **Consequential** |
|---|---|---|
| Named user segments, clear context (onboarding + product updates), and identified root cause. | If interviews show teams don't actually feel this pain, or if they have adequate solutions already, this hypothesis is wrong. | If wrong, the entire product direction changes — making this the most important assumption to test first. |

![Laptop with finger](assets/images/week-1/laptop-finger.HEIC)
---

## 4. Opportunity Solution Tree

The OST maps the path from our desired outcome to testable experiments. We start with the outcome, then identify the user pain points (opportunities) that, if addressed, would achieve it.

---

**DESIRED OUTCOME**

Sales and customer-facing team members reach full productivity and confidence in their role in 50% less time, without depending on a specific person being available to train them.

---

**OPPORTUNITIES (User Pain Points & Needs)**

| **Opportunity 1: Knowledge locked in people** | **Opportunity 2: No safe space to practice** | **Opportunity 3: Content goes stale fast** |
|---|---|---|
| New hires can only learn from specific people who are not always available. When that person is busy or leaves, knowledge disappears. | Sales reps have no way to rehearse calls or test product knowledge independently without consuming a colleague's or manager's time. | Existing documentation (SOPs, product guides, decks) becomes outdated and requires someone to manually update and re-communicate changes. |

---

**SOLUTIONS (Ideas to Address Opportunities)**

| **Solution A: AI Knowledge Base** | **Solution B: AI Call Simulator** | **Solution C: Living Knowledge Hub** |
|---|---|---|
| Cleo ingests company documents, SOPs, product guides, and call recordings. Team members can ask questions in natural language and get instant, accurate answers in their preferred format. | Cleo simulates real customer calls using the company's actual customer profiles, tone, and objection patterns learned from past recordings. Reps can practice anytime without needing a colleague. | Any team member can upload new documents, recordings, or updates to Cleo. The knowledge base stays current automatically, removing the single point of failure for knowledge transfer. |

---

**ASSUMPTION TESTS (Experiments to Validate)**

| **Test 1: Desirability** | **Test 2: Feasibility** | **Test 3: Viability** |
|---|---|---|
| Interview 8–10 sales managers and new hires across 3+ industries: Would they trust and regularly use an AI system for onboarding? What would make them stop using it? | Build a prototype that ingests 2–3 real company documents and responds accurately to questions. Test: does Cleo answer correctly 80%+ of the time without hallucinating? | Run a pricing test with 5 companies: Would they pay $X/month per seat? What's the minimum viable feature set before they'd pay? Target CAC < 3 months of revenue. |

---

## 5. Assumption Mapping

**Solution being evaluated:** Cleo — an AI system that ingests company knowledge (documents, videos, call recordings) and enables team members to learn and practice independently through natural conversation and call simulation.

| **DESIRABILITY — Do users want this?** | **VIABILITY — Does the business model work?** |
|---|---|
| • Sales teams experience onboarding as a real, painful problem | • Companies will pay a monthly SaaS fee per seat or per team |
| • Teams will trust an AI system to teach product knowledge | • CAC will be low enough to reach profitability within 12 months |
| • Sales reps will actually use a simulator to practice (vs. skipping it) | • The problem is painful enough that churn will be low |
| • Managers will champion adoption of Cleo to their teams | • Market is large enough (any company with a sales team) |
| **FEASIBILITY — Can we build this?** | **USABILITY — Can users figure it out?** |
| • We can reliably ingest documents, videos, and audio recordings | • Non-technical users can upload content without IT help |
| • AI can accurately represent company tone from call recordings | • New hires can self-onboard with Cleo without a walkthrough |
| • System won't hallucinate or give dangerously wrong product info | • Sales reps understand how to start a practice call simulation |
| • Build is achievable within the 5-week buildathon timeline | • Admins can update the knowledge base in under 10 minutes |

### Riskiest Assumption to Test First

> **Assumption:** Sales teams will trust an AI system enough to actually use it for onboarding and practice — and won't just default back to asking a colleague.
>
> **Why it's riskiest:** If teams don't trust Cleo's accuracy or feel it's impersonal, adoption will fail regardless of how well we build it. Trust is the prerequisite for everything else.
>
> **How we'll test it:** Conduct 8–10 story-based interviews with sales managers and recent new hires across 3+ industries. Ask about the last time they onboarded someone or were onboarded. Listen for pain around availability, consistency, and knowledge gaps.

---

## 6. Interview Guide

**Methodology:** Story-based interviewing — asking about specific past experiences, not hypotheticals. Conducted by both team members together where possible.

### Opening (set context)
- Tell me about your role and how long you've been at your current company.
- How many people have joined your sales team in the last 12 months?

### Story-Based Questions (core discovery)
- Tell me about the last time someone new joined your sales team. Walk me through what their first two weeks looked like.
- What was the hardest part of that onboarding process — for them, and for you?
- Tell me about a time when a new hire struggled with product knowledge during a real customer call. What happened?
- Think about the last product update or new service your team had to learn. How did that training happen? What worked and what didn't?
- Tell me about the last time a sales rep needed a quick answer during or before a call. Where did they go? How long did it take?

### Depth Questions (dig into the pain)
- How much time do you personally spend on onboarding or answering repetitive product questions each week?
- If you could wave a magic wand and fix one thing about how your team learns, what would it be?
- Have you tried any tools or systems to solve this? What happened?

### Solution Probing (test our hypothesis)
- If there was a system that could answer product questions instantly and let reps practice calls on their own — what would make you trust it enough to actually use it?
- What would make you stop using it?

---

## 7. Next Steps — Week 2

- **Conduct 6–8 interviews with sales managers and new hires across at least 3 industries**
- Complete an Interview Snapshot within 15 minutes of each interview
- Begin synthesizing: Interviews → Insights → Clusters → Themes → Opportunities
- Update the Opportunity Solution Tree based on what we learn
- Identify and prioritize the next riskiest assumption to test

> *Note: AI personas are for preparation only. Real human interviews are the source of truth — we will not skip them.*
