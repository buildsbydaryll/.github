# Daryll's Beehive

The projects of Daryllson Jumaoas ([@22104323](https://github.com/22104323) on GitHub): backends, servers and deployments. Each public repo says what it does, how to run it, and what I ran to check it. Where a project grew out of client or team work, the write-up keeps the problem and the approach and leaves out the client's name, code and hosts.

## Start here

| Repo | What it shows |
|---|---|
| [server-hardening](https://github.com/buildsbydaryll/server-hardening) | Two Ansible playbooks for a fresh Ubuntu or Debian VPS: one locks it down (key-only SSH, a deny-by-default firewall, automatic security updates, safer kernel and Docker settings), the other verifies every change on the server without changing anything. Its test runs both on a throwaway virtual machine. |
| [case-studies](https://github.com/buildsbydaryll/case-studies) | Write-ups of real problems from production work: what went wrong, what I chose and why, how I tested it, and what I traded away. |
| [reliability-labs](https://github.com/buildsbydaryll/reliability-labs) | Runnable labs that start from a backend defect, show it with a failing test, and fix it. The first is a FastAPI booking adapter that double-booked when the provider timed out, fixed with an idempotency key in PostgreSQL. One command runs it, and CI runs it on every push. |

## How I work

- **Tested, not claimed.** A change is finished when a test or check shows it works, and each write-up says which tests ran and what they required.
- **No secrets in Git.** Every push is scanned with gitleaks first, and real values live only in each host's secret store.
- **The smallest change that fully solves it.** Each case study ends with the trade-offs I accepted and why.

## Contact

Open to backend, platform and DevOps roles. Reach me through my GitHub profile, [@22104323](https://github.com/22104323).
