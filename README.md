# Ryan Glease

I'm a junior software developer in Hartlepool. I work mainly in Python and SQL, with a bit of Linux, Docker and C# when a project needs it.

I'm looking for a junior Python, backend or application-support role. I'm happy on-site around the North East, hybrid, or remote in the UK.

The projects below are mostly about the unglamorous parts: checking the data is real, making sure a job actually ran, and not letting a failed step disappear.

If you only click one, make it **Brand Finder**. It is the most complete example of how I work.

## Projects

### [Smoth Labs Terminal](https://github.com/Glease1/smoth-labs-terminal)

A crypto derivatives terminal that pulls data from Binance, Bybit, Hyperliquid, Kraken and Deribit into SQLite, scores the market and puts 17 views on one screen.

There is no order endpoint and no key custody. The execution guard is enforced in code and covered by tests. The research side keeps the ideas that didn't work as well as the ones that did.

Start with the [architecture](https://github.com/Glease1/smoth-labs-terminal/blob/main/docs/ARCHITECTURE.md), then the [research results](https://github.com/Glease1/smoth-labs-terminal/blob/main/docs/RESEARCH.md).

### [Brand Finder Case Study](https://github.com/Glease1/brandfinder-case-study)

A Solana memecoin system built around execution control, not a trading signal. It watches nine live data sources, runs each candidate through fail-closed safety gates, and records every rejection with the reason it failed.

The part I find most useful is how the decisions are separated: a paper arena asks what a rule would have done, a shadow ledger checks whether a real quote actually existed, and a 0.01 SOL canary proves the real execution path works. Several strategy variants are scored side by side, and the result is not a win: 171 closed rows, a profit factor of 1.22, the top three trades making 154% of the profit, and no edge once those are removed.

If you read one section, read the [failure taxonomy](https://github.com/Glease1/brandfinder-case-study/blob/main/docs/FAILURE-TAXONOMY.md). The [evidence](https://github.com/Glease1/brandfinder-case-study/blob/main/EVIDENCE.md) explains what was tested and what was not.

### [Odjob Launcher](https://github.com/Glease1/odjob-launcher)

A C#/.NET WPF launcher for three Bond game ports. It detects an install, checks the user's own disc or ROM, builds the port when needed, launches it, and opens a small TCP room so two people can start the same game together.

It ships no game code and no assets. The interesting bits are the media validation, process supervision, single-instance handling, and the UPnP/SSDP work needed to make the room reachable.

### [EnterpriseCloudAdmin](https://github.com/Glease1/enterprise-cloud-admin)

A Linux and Ansible lab I built to practise the things an infrastructure or application-support job actually involves.

Four Ansible roles set up a default-deny UFW firewall, SSH with no password login and no root login, and a small set of admin tools. The C# `UserAdminTool` handles local account create/delete/lock/reset and writes every action to an audit log.

The [README](https://github.com/Glease1/enterprise-cloud-admin) covers the roles, the tools and the limitations, including the broad sudo rule I would not use on a shared host.

### [Web-Development](https://github.com/Glease1/Web-Development)

A PHP 8 and SQLite travel booking application with no framework. Front controller, session basket, CSRF protection, role-gated admin area and a small schema.

It is the least exotic project here, but it is a complete small application: routing, sessions, validation, database access and an admin surface all in one place.

## How I work

I usually start with the failure cases. The bugs worth remembering are the boring ones: a sweep that closes a position that was still open, a sell that fails after the decision to sell, a feed that connects and then sends nothing.

When something goes wrong, I write it up: what happened, what it affected, and what changed so it can't happen the same way again.

I try not to claim more than the evidence supports. The trading work has a profit factor above 1, but once the top three trades are removed it loses money. That's not an edge, and the write-up says so.

## Tools

Python, asyncio, FastAPI, SQLite, SQL, Linux, SSH, Ansible, systemd, Docker Compose, Git, pytest, C#/.NET, HTML/CSS, PowerShell.

I also use Microsoft Entra ID, Entra PIM, Duo MFA and audit trails in my day job in IT support. That comes in handy when the thing I'm debugging turns out to be an identity problem.

## Currently

I'm finishing the public write-up for Smoth: architecture, research results and a walkthrough of the main views. Every repo here is meant to say what it does and what it still doesn't do.

**Contact:** [ryanglease1@protonmail.com](mailto:ryanglease1@protonmail.com). CV available on request.

<sub>I use AI coding tools heavily for implementation. The requirements, failure analysis and acceptance are mine, and each project says where the line is.</sub>
