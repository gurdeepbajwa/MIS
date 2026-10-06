# How to Design a Defence-in-Depth Strategy

Course: [[Cyber Security Management (ISYS90090)/Course Overview|Cyber Security Management (ISYS90090)]]
Week: 05
Type: How-to guide
Source: [[Cyber Security Management (ISYS90090)/Week 05/Lecture|Week 05 Lecture]]

## Purpose

Use this guide to turn a case into an exam-ready defence-in-depth design. It focuses on control choice and reasoning rather than technical product detail.

## Start-to-Finish Method

### 1. Define the Risk Scenario

State:

- the asset or business capability;
- the threat actor and motive;
- the vulnerability and attack route;
- the likely business and CIA impact.

Do not begin with a list of security products. Control choice depends on this scenario.

### 2. Separate

Create enforced boundaries between the actor and asset.

Ask:

- Which network or service boundaries exist?
- Can traffic bypass them?
- Should the asset sit in a more restricted segment?
- How will approved remote users cross the boundary?

Possible controls include firewalls, network segmentation, secure remote access, and VPNs.

### 3. Observe

Place monitoring where it can see attempted entry, traffic that passed a boundary, internal movement, and activity at the endpoint.

Possible controls include network IDS, host agents, central logs, behaviour monitoring, and an IDPS where safe blocking rules exist.

Explain who receives each alert and what they should do. Detection without response does not stop an attack.

### 4. Mediate

Control every approved request for the asset.

Use:

- authentication to check identity;
- authorisation to set allowed actions;
- least privilege and need-to-know access;
- encryption to protect the asset if another control fails;
- logging and review to find misuse of valid access.

### 5. Assess the Attack Surface

Check:

- exposed systems, services, ports, and devices;
- weak or changed configurations;
- public or wireless information leakage;
- gaps created since the last penetration test.

Treat a penetration test as a dated view, not proof of continuing security.

### 6. Add Management Support

State the formal and human controls that make the technology work:

- clear asset and control ownership;
- policy and operating rules;
- staff training and reporting;
- incident response and recovery;
- control tests and regular review;
- cloud-provider duties and assurance where relevant.

### 7. Show How the Layers Work Together

Finish by explaining the combined effect:

- separation delays and contains;
- observation detects and informs response;
- mediation limits each request;
- encryption protects content after another failure;
- management controls keep the design current.

## Quick Exam Template

> **[Asset]** faces **[actor and threat]** through **[vulnerability and vector]**. The organisation should separate the asset using **[controls]**, observe entry and movement using **[controls and vantage points]**, and mediate each request using **[identity, access, and encryption controls]**. These layers work together by **[delay, detection, containment, and response]**. **[Policy, ownership, staff practice, and review]** keep the controls aligned with the risk.

## Quality Check

Before finishing, confirm that the answer:

- names one exact risk scenario;
- uses at least the three functions of separate, observe, and mediate;
- links every control to a weakness or attack stage;
- includes both technological and managerial controls;
- addresses cloud or mobile use when the asset leaves the organisation's own network;
- explains the combined effect rather than listing controls.
