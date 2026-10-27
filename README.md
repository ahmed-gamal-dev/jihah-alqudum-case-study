# Jihah Al Qudum (جهة القدوم)

> Saudi recruitment and domestic-worker rental platform.

**Live:** [jihahalqudum-co.com](https://jihahalqudum-co.com/) · **Role:** Technical lead & developer · **Period:** 2026 · **For:** Al Shohab Al Aliyah

![Laravel 12](https://img.shields.io/badge/Laravel_12-2E2A8C?style=flat-square) ![PHP](https://img.shields.io/badge/PHP-2E2A8C?style=flat-square) ![Modular architecture](https://img.shields.io/badge/Modular_architecture-2E2A8C?style=flat-square) ![MySQL](https://img.shields.io/badge/MySQL-2E2A8C?style=flat-square) ![Paymob KSA](https://img.shields.io/badge/Paymob_KSA-2E2A8C?style=flat-square) ![Firebase](https://img.shields.io/badge/Firebase-2E2A8C?style=flat-square) ![Flutter](https://img.shields.io/badge/Flutter-2E2A8C?style=flat-square)

![Jihah Al Qudum (جهة القدوم) — home page](screenshots/desktop.png)

## Overview

A platform for direct recruitment through Musaned and for monthly, yearly and hourly worker rental: clients browse workers, request them, sign contracts, pay in installments and follow everything online or from the mobile app.

## What it does

- Worker catalog by nationality, skills and experience
- Recruitment requests and rental contracts
- Installment plans and online payment
- Renewals, cancellations, refunds and worker replacement
- Contract PDF based on the Musaned unified contract
- Admin back office with branches, reports and WhatsApp booking

## Engineering highlights

- Contract state machine (13 states) with an immutable audit trail
- No double booking: date-range reservations under database row locks, proven by a concurrency test
- Signature-verified, idempotent payment webhooks
- Rule-based pricing snapshotted onto each contract
- ~300 commits, pull-request workflow, CI/CD to Hostinger

## Screenshots (live site)

<p>
  <img src="screenshots/mobile.png" width="260" alt="Mobile">
  <img src="screenshots/page1.png" width="520" alt="Page">
  <img src="screenshots/page2.png" width="520" alt="Page">
</p>

<details>
<summary>Full home page</summary>

![Full page](screenshots/long.png)

</details>

## Mobile app (Flutter)

| Home | Catalog | Worker | Contracts | Contract |
|---|---|---|---|---|
| <img src="screenshots/app/01-home.png" width="160"> | <img src="screenshots/app/04-catalog.png" width="160"> | <img src="screenshots/app/05-worker-detail.png" width="160"> | <img src="screenshots/app/06-contracts.png" width="160"> | <img src="screenshots/app/07-contract-detail.png" width="160"> |

---

Source code is private (client / commercial project). This repository documents the work only.

Built by **Ahmed Gamal** — Senior Laravel Developer · [LinkedIn](https://www.linkedin.com/in/wzcoder/) · [GitHub](https://github.com/ahmed-gamal-dev)
