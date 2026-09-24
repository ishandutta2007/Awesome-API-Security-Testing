# Awesome-API-Security-Testing

# Top API Security Testing Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on API Vulnerability Scanning, OpenAPI/GraphQL Security Testing, BOLA/BFLA Detection, DAST for APIs & Continuous API Security*  
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **API Security Testing**. These tools discover APIs, test against the OWASP API Security Top 10, fuzz OpenAPI/GraphQL contracts, find broken object/function level authorization, and integrate into CI/CD for continuous protection.

**Examples** include 42Crunch, Traceable AI, Salt Security, Noname Security, Escape, Wallarm, Cequence Security, Data Theorem, Akto, Probely, StackHawk, FireTail, and related API security platforms (the category leaders).

**Open-source emphasis**: API security testing has excellent open tooling. **OWASP ZAP**, **Nuclei**, **Schemathesis**, the **OWASP API Security Testing Framework**, and related projects provide production-usable testing. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[42Crunch](https://42crunch.com/)**  
  API security platform centered on OpenAPI contract security audit, conformance, and runtime protection aligned with API design-time and runtime controls.

- **[Salt Security, Noname Security, Traceable AI](https://salt.security/)**  
  API security and discovery platforms providing continuous testing, posture, and threat detection across API estates.

- **[Escape, Wallarm, Cequence Security](https://escape.tech/)**  
  Platforms combining API discovery, DAST-style testing, and runtime or WAF-adjacent protection for APIs and GraphQL.

- **[Data Theorem, Probely, StackHawk, Akto, FireTail](https://www.datatheorem.com/)**  
  API and application security testing tools focused on automated scanning, CI integration, and developer-friendly API security workflows.

- **[Other commercial API security platforms](https://42crunch.com/)**  
  Additional solutions for inventory, testing, and protection of REST, GraphQL, and microservice APIs.

## Open-Source GitHub Projects

- **[OWASP ZAP (Zed Attack Proxy)](https://github.com/zaproxy/zaproxy)**  
  Leading open-source DAST tool with strong API support—imports OpenAPI/Swagger and GraphQL, actively tests for common and API-specific vulnerabilities, and runs headlessly in CI/CD.

- **[Nuclei (ProjectDiscovery)](https://github.com/projectdiscovery/nuclei)**  
  Template-based scanner with a large community library covering API issues (BOLA/IDOR patterns, JWT weaknesses, GraphQL exposure, SSRF, auth bypass, and more)—ideal for continuous API security checks.

- **[Schemathesis](https://github.com/schemathesis/schemathesis)**  
  Property-based testing for OpenAPI and GraphQL APIs—generates inputs from the schema, finds contract violations, stateful bugs, and edge cases that manual tests miss.

- **[OWASP API Security Testing Framework](https://github.com/OWASP/www-project-api-security-testing-framework)**  
  Specialized open framework targeting OWASP API Security Top 10 coverage with automated test cases for REST and related API styles.

- **[Wallarm API Firewall (open)](https://github.com/wallarm/api-firewall)**  
  Open-source API proxy firewall that validates requests/responses against OpenAPI specs (positive security model) for REST and GraphQL.

- **[RESTler & Microsoft API fuzzing research](https://github.com/microsoft/restler-fuzzer)**  
  Stateful REST API fuzzing that learns producer-consumer dependencies from OpenAPI specs to find deeper logic bugs.

- **[mitmproxy, Postman/Newman, Insomnia automation](https://github.com/mitmproxy/mitmproxy)**  
  Open proxies and collection runners used to capture and replay API traffic for security review and regression testing.

- **[k6, artillery & load tools with security checks](https://github.com/grafana/k6)**  
  Open performance tools often extended with security assertions for API resilience and abuse testing.

### Additional Strong Open-Source Options

- **DAST workhorses**: OWASP ZAP for broad API DAST; Nuclei for fast, template-driven coverage.
- **Contract-driven testing**: Schemathesis and RESTler for schema-based and stateful fuzzing.
- **Positive security / gateway**: Wallarm API Firewall for OpenAPI-enforced request validation.
- **CI/CD pipelines**: ZAP + Nuclei + Schemathesis in GitHub Actions or similar for continuous API security.
- **Composable stacks**: Spec audit → dynamic scan → fuzz → runtime OpenAPI validation.
- Commercial platforms still lead in automatic API discovery, inventory, and business-logic attack coverage at scale.

**Frameworks for building custom systems**:  
**OWASP ZAP**, **Nuclei**, and **Schemathesis** form a powerful open API security testing stack.  
Add **RESTler** for deeper stateful fuzzing and **Wallarm API Firewall** for runtime contract enforcement.  
Commercial platforms (42Crunch, Salt, Noname, Traceable, Escape, Wallarm, StackHawk, etc.) add discovery, continuous posture, and managed findings workflows.  
Many teams run open tools in CI for every PR and use commercial API security platforms for estate-wide visibility and runtime protection. Fully open pipelines are production-viable for testing; discovery and runtime often benefit from commercial or hybrid approaches.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- API security testing can generate traffic that looks like attacks. Only test systems you own or have explicit permission to test. Coordinate with operations to avoid availability impact.
- Open-source scanners require tuning to reduce false positives and to cover auth, rate limits, and business logic. Commercial platforms often provide richer discovery and prioritization. Combine automated testing with manual review for critical APIs.

---

**Made for AppSec engineers, API developers, and DevSecOps teams securing modern APIs.**  
Let's keep API security testing open and continuous—through excellent open scanners and complementary commercial platforms.
