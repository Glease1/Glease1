# Ryan Glease

I'm a junior software developer in Hartlepool. I work mainly in Python and SQL, with a bit of Linux, Docker and C# when a project needs it.

I'm looking for a junior Python, backend or application-support role. I'm happy on-site around the North East, hybrid, or remote in the UK.

The projects below are mostly about the unglamorous parts: checking the data is real, making sure a job actually ran, and not letting a failed step disappear.

## Projects

- **[Smoth Labs Terminal](https://github.com/Glease1/smoth-labs-terminal)** — a local-first terminal for crypto derivatives. It pulls data from several venues, stores it in SQLite, and puts 17 views on one screen. There is no order execution path, and that's enforced in code. The research side keeps the ideas that didn't work as well as the ones that did.
- **[Brand Finder Case Study](https://github.com/Glease1/brandfinder-case-study)** — what happened when a small real-money execution system had to handle ownership, pending exits, failed sells and valuation. It includes the measurement that says the strategy has no edge. The source is private.
- **[Odjob Launcher](https://github.com/Glease1/odjob-launcher)** — a C#/.NET WPF launcher for three Bond game ports. It validates discs and ROMs, supervises processes, and uses a small TCP room protocol with IPv4 join codes.
- **[EnterpriseCloudAdmin](https://github.com/Glease1/enterprise-cloud-admin)** — a Linux and Ansible lab: a four-role baseline over SSH, UFW and SSH hardening, plus a few small .NET tools, including a user-account CLI with an audit trail. Source included.
- **[Web-Development](https://github.com/Glease1/Web-Development)** — a PHP 8 and SQLite travel booking app. No framework: front controller, session basket, CSRF protection and a role-gated admin area. Source included.

## How I work

I usually start with the failure cases. The bugs worth remembering are the boring ones: a sweep that closes a position that was still open, a sell that fails after the decision to sell, a feed that connects and then sends nothing.

When something goes wrong, I write it up: what happened, what it affected, and what changed so it can't happen the same way again.

I try not to claim more than the evidence supports. The trading work ended with 171 closed trades, a profit factor of 1.22, and the top three trades making 154% of the profit. Without those three it lost money, so I don't call it an edge. That result is in the write-up.

## Tools

Python, asyncio, FastAPI, SQLite, SQL, Linux, SSH, Ansible, systemd, Docker Compose, Git, pytest, C#/.NET, HTML/CSS, PowerShell.

I also use Microsoft Entra ID, Entra PIM, Duo MFA and audit trails in my day job in IT support. That comes in handy when the thing I'm debugging turns out to be an identity problem.

## Currently

I'm finishing the public write-up for Smoth: architecture, research results and a walkthrough of the main views. Every repo here is meant to say what it does and what it still doesn't do.

**Contact:** [ryanglease1@protonmail.com](mailto:ryanglease1@protonmail.com). CV available on request.

<sub>I use AI coding tools heavily for implementation. The requirements, failure analysis and acceptance are mine, and each project says where the line is.</sub>
