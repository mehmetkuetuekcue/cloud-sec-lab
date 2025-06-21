# Cloud-Sec-Lab

Personal sandbox to learn **Cloud Security & DevSecOps**  
*Perth (AU), started **21 Jun 2025**.*

---

## Roadmap (2025)

| Week | Milestone                                  | Status   |
| ---- | ------------------------------------------ | -------- |
| 01   | ✔ GitHub + AWS Free-Tier set-up            | Complete |
| 02   | GitHub supply-chain lab (Dependabot, SBOM) | *Next*   |
| 03   | PortSwigger first 5 labs                   |          |
| 04   | Deploy OWASP Juice Shop to AWS             |          |
| …    | …                                          |          |

> *Update this table each Sunday so progress stays visible.*

---

## Lab structure

```text
/
├── docs/            # blog drafts, slides, research notes
├── terraform/       # Infrastructure-as-Code (*.tf) for AWS lab
├── pipelines/       # GitHub Actions workflow YAML files
├── scripts/         # helper Bash/Python scripts (e.g. Trivy filter)
├── juice-shop/      # forked OWASP Juice Shop source & Dockerfile
├── opa/             # Rego policies + unit tests
└── images/          # screenshots & diagrams referenced in README
```

### Folder purpose quick-ref

- **docs/** – long-form write-ups, slide decks, raw lab notes.  
- **terraform/** – reproducible AWS environment definitions; run `terraform init && terraform apply` here.  
- **pipelines/** – version-controlled CI/CD definitions (GitHub Actions). Each file mirrors one security gate or deployment flow.  
- **scripts/** – automation (≤ 50 LOC) used by pipelines or during manual testing.  
- **juice-shop/** – self-contained vulnerable app, includes a `Dockerfile` and `docker-compose.yml` for local runs.  
- **opa/** – policy-as-code: `.rego` rules + tests; executed via Conftest in CI.  
- **images/** – PNGs/GIFs for README and blog posts. Name with ISO date + short slug.

---

## Useful links

- **GitHub profile** → <https://github.com/mehmetkuetuekcue>  
- **AWS Free-Tier Console** → <https://console.aws.amazon.com/>  
- **PortSwigger Academy** → <https://portswigger.net/web-security>

Happy hacking ! 🛡️
