# Ryan Glease

**Junior software developer in Hartlepool, UK.** Python services, SQL, Linux — and a habit of documenting what went wrong.

I build systems that collect data, make decisions and have to survive being wrong. Most of what is here is about the gap between a **decision** and an **action**: who owns a job, whether a decision was executed, whether a number came from a real source, and what happens when a step fails silently.

I am looking for a **junior Python, backend or application-support role**, on-site in the North East, hybrid, or remote in the UK.

---

## What's here

| Repository | What it is |
|---|---|
| **[smoth-terminal](https://github.com/Glease1/smoth-terminal)** | A local-first terminal for crypto derivatives: 46 FastAPI/SQLite service modules, 17 views, a research harness with pre-registration and a rejection archive. No execution path, enforced in code. |
| **[brandfinder-case-study](https://github.com/Glease1/brandfinder-case-study)** | The engineering story of a small real-money execution system: ownership, pending exits, valuation tiers, exit attribution, and the measurement that says the strategy has no edge. The source is private; this is the part worth reading. |
| **[odjob-launcher](https://github.com/Glease1/odjob-launcher)** | A C#/.NET WPF launcher and session coordinator for three Bond game ports: disc/ROM validation, process supervision, a TCP room protocol and IPv4 join codes. |

---

## How I work

- **I test the failure path first.** The regression tests worth keeping came from incidents: an orphan sweep closing a live position, a sell that failed after the decision to sell, a venue feed that connected and sent nothing.
- **I write the incident up.** Root cause, blast radius, a prevention rule — one page, kept beside the code.
- **I say what is not proven.** The trading work ends with 171 closed trades, a profit factor of 1.22, and the top three trades accounting for 154% of the profit. Excluding those three it loses money. So I do not claim an edge, and I keep the negative results in the archive.

---

## Tools I actually use

`Python` · `asyncio` · `FastAPI` · `SQLite` (WAL, migrations, retention) · `SQL` · `Linux` · `SSH` · `Ansible` · `systemd` · `Docker Compose` · `Git` · `pytest` · `C#/.NET` · `HTML/CSS` · `PowerShell`

Also: Microsoft Entra ID, Entra PIM, Duo MFA and audit-trail work from my day job in IT support — useful when the thing I am debugging is an identity problem.

---

## Currently

- Building out the Smoth publication: architecture, research results and a screenshot tour.
- Every repository here states its limitations, including the ones I have not fixed.
- Open to junior developer and application-support roles.

**Contact:** [ryangleas1@protonmail.com](mailto:ryangleas1@protonmail.com) — CV available on request.

---

<sub>Everything here is my own work or an integration layer over other people's work, and I say which is which. AI coding tools were used heavily for implementation; the requirements, the failure analysis and the acceptance were mine, and that is documented in each project.</sub>
