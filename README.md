# AWS Offensive Security — Red Team Curriculum

Advanced cloud attack course covering 21 modules and 95+ hands-on labs across four tiers, from beginner S3 enumeration to full organizational compromise.

## Structure

```
index.html              Main single-page application
labs/
  beginner/             Modules 01–05  (Tier 1)
  intermediate/         Modules 06–10  (Tier 2)
  expert/               Modules 11–16  (Tier 3)
  mahaguru/             Modules 17–21  (Tier 4)
```

## Tiers

| Tier | Modules | Focus |
|------|---------|-------|
| Beginner | M01–M05 | S3, IAM enumeration, RDS, Lambda/API GW |
| Intermediate | M06–M10 | IMDS, SNS credential capture, SSM, Lambda RCE, EBS secrets |
| Expert | M11–M16 | Identity Center, SSO phishing, ECR supply chain, container escape, EKS RBAC, IAM privesc |
| Mahaguru | M17–M21 | CI/CD compromise, cross-account attacks, persistence/evasion, serverless chains, capstone kill-chain |

## Running Locally

Labs load via `fetch()` and require an HTTP server (not `file://`):

```bash
python3 -m http.server 8080
# open http://localhost:8080
```

## Tech Stack

- Vanilla HTML/CSS/JS — zero build step, zero dependencies
- Lab walkthroughs are separate HTML fragments loaded on demand
- Progress tracked in `localStorage`

## Legal

All techniques are for **authorized testing only**. Every lab includes an authorized-testing disclaimer. Never perform these actions on systems you do not have explicit written permission to test.
