# [EyalSec status](https://eyalsec.github.io/status/): <!--live status--> **All systems operational**

[![Uptime CI](https://github.com/EyalSec/status/workflows/Uptime%20CI/badge.svg)](https://github.com/EyalSec/status/actions/workflows/uptime.yml)
[![Response Time CI](https://github.com/EyalSec/status/workflows/Response%20Time%20CI/badge.svg)](https://github.com/EyalSec/status/actions/workflows/response-time.yml?query=workflow%3A%22Response+Time+CI%22)
[![Graphs CI](https://github.com/EyalSec/status/workflows/Graphs%20CI/badge.svg)](https://github.com/EyalSec/status/actions/workflows/graphs.yml?query=workflow%3A%22Graphs+CI%22)
[![Static Site CI](https://github.com/EyalSec/status/workflows/Static%20Site%20CI/badge.svg)](https://github.com/EyalSec/status/actions/workflows/site.yml?query=workflow%3A%22Static+Site+CI%22)
[![Summary CI](https://github.com/EyalSec/status/workflows/Summary%20CI/badge.svg)](https://github.com/EyalSec/status/actions/workflows/summary.yml?query=workflow%3A%22Summary+CI%22)

If something in EyalSec is not working for you, this page tells you within
about five minutes whether the problem is on our side. It shows the live state
of the website, the dashboard and API, and the documentation, with response
times and the history of every incident.

- **Status page:** https://eyalsec.github.io/status/
- **Help with your account or a machine:** support@eyalsec.com
- **Security reports:** security@eyalsec.com

## What is checked

| Service | Check |
| --- | --- |
| Website | `GET https://eyalsec.com` answers with a success status |
| Dashboard and API | `GET https://eyalsec.com/healthz` answers and its body reads `ok` |
| Documentation | `GET https://eyalsec.com/docs` answers with a success status |

Each check runs every five minutes from GitHub's hosted runners. When one
fails, an [issue](https://github.com/EyalSec/status/issues) opens with the
`status` label, and the same issue closes on its own when the service answers
again, so the issue list doubles as the incident history. GitHub can start a
scheduled run a few minutes late when it is busy, so read the times as close,
not exact.

## Current numbers

<!--start: status pages-->
<!--end: status pages-->

## How it works

This page runs on [Upptime](https://upptime.js.org) by
[Anand Chowdhary](https://anandchowdhary.com) and its contributors, an uptime
monitor built entirely from GitHub Actions, Issues and Pages. Thank you to
them: it lets us publish our availability in the open without running another
server. The checks live in [`.upptimerc.yml`](.upptimerc.yml), and every
result is committed to [`history/`](history), so the record can be audited
line by line.

## About EyalSec

EyalSec is a secure Python that catches injection as your app runs: es-python
runs your Python app unchanged and follows untrusted input to the SQL query,
shell command or file path that uses it, then reports each flow or stops it.
See [eyalsec.com](https://eyalsec.com), or
[book a live demo](https://eyalsec.com/contact).

## License

- Code: [MIT](LICENSE)
- Data in [`history/`](history): [Open Database License](https://opendatacommons.org/licenses/odbl/1-0/)
