---
title: "iPhone 15 Pro battery replacement with linked pack - EN note"
date: 2025-12-01
layout: note
lang: "en"
tags:
  - "repair"
  - "iPhone 15 Pro"
  - "battery replacement"
  - "Service36"
---

## Summary
An iPhone 15 Pro came in with around 87 percent reported battery health and roughly 500 charge cycles. The owner wanted to pass the phone to another family member and expected it to behave like a device with a fresh battery. We decided to install a JCID zx linked battery instead of a more expensive AASP pack, and configured it through Apple's repair assistant.

## Key symptoms
- noticeable battery drain by the end of a regular day
- more frequent charging compared to the first year of use
- battery health reported in the low 80s range
- cycle count already in the several hundred range
- no obvious reboots or instability from the logic board

## Diagnostics highlights
- verified stable power rails and no board level faults related to power
- matched the client's complaints with normal lithium cell wear for iPhone 15 Pro
- considered that iOS 26.1 can optimize behavior, but cannot undo physical degradation
- discussed future usage pattern, since the phone is being handed down in the family
- compared three battery options: AASP pack, JCID zx linked pack, and "orig" packs that do not pass authenticity checks

## Technical notes
- for iPhone 15 Pro, 80–85 percent health plus several hundred cycles already means reduced runtime for active users
- JCID zx linked packs, once configured via repair assistant, show up as genuine used Apple parts with a repair date
- controller level manufacture dates can be synthetic and not match the actual cell production date
- from the user's perspective, having 100 percent health and no constant authenticity warnings in settings is a big quality of life factor
- realistic lifespan for such linked batteries under active daily use is about one and a half years

## Practical conclusion
When an iPhone 15 Pro still behaves well on the logic board side but clearly suffers from battery wear, a linked JCID zx pack can be a sensible middle ground. It integrates cleanly into iOS, keeps the service history consistent and restores predictable battery life, without the full cost of an AASP battery. For family hand me downs this is often the most rational mix of cost, behavior and expected lifetime.

Full RU case in the Service36 blog:  
👉 https://service36.ru/blog/0112-iphone15pro-zamena-akkumulyatora-voronezh/
