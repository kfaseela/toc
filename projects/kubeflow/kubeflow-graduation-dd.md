# Kubeflow Graduation Due Diligence

- Link to [Graduation Application: Kubeflow](https://github.com/cncf/toc/issues/1861)

## Graduation Evaluation Summary for Kubeflow

### Criteria Evaluation

[Faseela K](https://github.com/kfaseela) conducted the due diligence for Kubeflow, which applied for Graduation from Incubating status (accepted 2023-07-23).

The following criteria implementations are noteworthy:

- [Kubeflow](https://www.kubeflow.org/) is a modular, Kubernetes-native AI/ML platform that provides a foundation of composable tools for building and operating AI/ML workloads at scale. This graduation covers **6 subprojects**: Kubeflow Trainer, Kubeflow Pipelines, Kubeflow Katib, Kubeflow Notebooks, Kubeflow Spark Operator, and Kubeflow Hub (repo: kubeflow/hub). Each subproject satisfies the graduation criteria independently.
- The project's governance is multi-layered, with a Kubeflow Steering Committee (KSC, 5 seats, max 1 per organization) for strategic decisions, the Kubeflow Outreach Committee for community-facing coordination, the Kubeflow Distribution Committee (KDC) for release coordination, and Working Groups owning each subproject. The 2026 KSC election completed on schedule, with all seats filled and no organization holding more than 1 seat.
- Strong contributor health per [LF Insights](https://insights.lfx.linuxfoundation.org/foundation/cncf/overview/github?project=kubeflow&routedFrom=Github&bestPractice=false&repository=all&dateFilters=Last%20365%20Days&dateRange=custom&startDate=2025-06-17&endDate=2026-06-17): active contributors from a wide range of organizations, with positive YoY growth.
- A [General Technical Review (GTR)](https://github.com/kubeflow/community/blob/master/KUBEFLOW-GENERAL-TECHNICAL-REVIEW.md) was completed in September 2025, providing comprehensive architecture, design, and engineering documentation that satisfies several DD criteria. GTR snapshot is merged into cncf/toc via [Add Kubeflow GTR snapshot (toc#2180)](https://github.com/cncf/toc/pull/2180).
- All 6 graduation subprojects hold at least an OpenSSF Best Practices Passing badge; Kubeflow Trainer and Kubeflow Katib have achieved Gold.
- The Kubeflow Ecosystem page and process were established during this review in response to DD findings, clarifying the boundary between core subprojects and ecosystem partners (KServe, Feast, Elyra). KServe, previously presented under the Kubeflow brand, is now clearly identified as an independent CNCF Incubating project.
- Kubeflow demonstrates broad adoption spanning scientific research, financial services, logistics, and AI/ML platform industries, with production deployments ranging from hundreds to tens of thousands of daily active users and hundreds of thousands of indirect business end users. Four adopter interviews were conducted, collectively covering all 6 graduation subprojects across diverse industries and deployment scales.
- The Kubeflow maintainers and community have been exceptionally responsive throughout this review - PRs were merged, issues filed and assigned, and maintainers engaged constructively on all feedback.

The following blocking items were identified during the review and must be resolved before a graduation vote:

- **Adopter interview publication approval**: All 4 planned adopter interviews have been conducted (CERN, and three additional adopters from financial services, logistics, and AI/ML platform sectors). CERN and one additional adopter (financial services, published anonymously) have approved their interviews for publication. The remaining 2 interviews are pending formal publication approval from the respective adopters before they can be cited publicly in the DD. Interview reports cover all 6 graduation subprojects and are available for TOC review pending approval.

The following items were raised and resolved during the review:

- **[kubeflow/community#992](https://github.com/kubeflow/community/issues/992) - Track and resolve third-party security audit findings**: The Ada Logics audit report (Sept 2025) is published at [security/Ada_Logics-Kubeflow-security-audit-2025.pdf](https://github.com/kubeflow/community/blob/master/security/Ada_Logics-Kubeflow-security-audit-2025.pdf). All in-scope findings are resolved or tracked with linked PRs/issues. KServe findings are out of scope as KServe is an independent CNCF project. Full tracking details are in [kubeflow/community#992](https://github.com/kubeflow/community/issues/992). Resolved.

- **[kubeflow/community#972](https://github.com/kubeflow/community/issues/972) - Document contributor progression to WG Lead/Chair roles**: WG governance refactored via [Refactor WG governance and Chair requirements (community#989)](https://github.com/kubeflow/community/pull/989): WGs now have clearly documented Chair requirements (must be a community Member, hold a subproject role, sustained contributions, sponsored by a member + super-majority vote), responsibilities/privileges, 2+ Chairs minimum, and all private Google Doc links removed.
- **[kubeflow/community#988](https://github.com/kubeflow/community/issues/988) - Fix roadmap gaps**: ROADMAP.md added to kubeflow/notebooks ([Add ROADMAP.md (notebooks#1188)](https://github.com/kubeflow/notebooks/pull/1188)); kubeflow/kubeflow README and platform roadmap updated ([Update kubeflow README (kubeflow#7790)](https://github.com/kubeflow/kubeflow/pull/7790), [Update platform roadmap (kubeflow#7788)](https://github.com/kubeflow/kubeflow/pull/7788)); website subproject table updated ([Update website subproject table (website#4409)](https://github.com/kubeflow/website/pull/4409)).
- **[kubeflow/community#990](https://github.com/kubeflow/community/issues/990) - Add notebooks release process documentation**: `RELEASE.md` added to `kubeflow/notebooks` main branch via [Add RELEASE.md (notebooks#1189)](https://github.com/kubeflow/notebooks/pull/1189), pointing to detailed step-by-step release docs in `releasing/README.md` on both `notebooks-v1` and `notebooks-v2` branches.
- **[kubeflow/community#955](https://github.com/kubeflow/community/issues/955) - KSC vendor-neutrality language and election status**: Stale KEP-645 org-limit language and overdue election state. Resolved via [Add 2026 KSC election results (community#956)](https://github.com/kubeflow/community/pull/956) and [Consolidate KSC org-limit rule (community#957)](https://github.com/kubeflow/community/pull/957).
- **[kubeflow/community#961](https://github.com/kubeflow/community/issues/961)/[community#962: KServe subproject status](https://github.com/kubeflow/community/issues/962) - KServe ecosystem categorization**: KServe was presented as a Kubeflow subproject without indicating its independent CNCF Incubating status. Resolved via merged PRs: [Add ecosystem join process (community#963)](https://github.com/kubeflow/community/pull/963), [Add Kubeflow Ecosystem page (website#4384)](https://github.com/kubeflow/website/pull/4384), [Add subproject maturity levels (community#965)](https://github.com/kubeflow/community/pull/965). *Note*: Adopter interviews further validated this finding - production adopters continue to reference KServe as part of their Kubeflow deployment, reflecting the tight historical association. This reinforces the importance of the ecosystem boundary clarification work completed above.

The following non-blocking recommendations were provided:

- **[kubeflow/community#964](https://github.com/kubeflow/community/issues/964) - Submit Kubeflow GTR snapshot to cncf/toc**: Merged via [Add Kubeflow GTR snapshot (toc#2180)](https://github.com/cncf/toc/pull/2180). Resolved.
- **[kubeflow/community#996](https://github.com/kubeflow/community/pull/996) - Security self-assessment submission to cncf/toc**: Merged via [Kubeflow Security Self-Assessment (toc#2201)](https://github.com/cncf/toc/pull/2201). Resolved.
- **[kubeflow/community#976](https://github.com/kubeflow/community/issues/976) - Add `CODE_OF_CONDUCT.md` files to subproject repos**: All graduation subproject repos now have `CODE_OF_CONDUCT.md`.
- **[kubeflow/community#991](https://github.com/kubeflow/community/issues/991) - Security self-assessment enhancements**: Broken Trainer release link fixed and stale vulnerability-status wording updated via [Fix self-assessment links and stale wording (community#996)](https://github.com/kubeflow/community/pull/996).
- **Community/ADOPTERS.md listed KServe in the "Adopters of Kubeflow Projects" table**: KServe removed from the subprojects adopters table; only the 6 graduation subprojects are listed.
- **[kubeflow/community#967: WG docs subproject ownership](https://github.com/kubeflow/community/issues/967)/[community#969: WG README stale links](https://github.com/kubeflow/community/issues/969) - WG-level meeting docs had stale/broken links**: Outdated WGs/SIGs removed via [Remove outdated WGs/SIGs (community#974)](https://github.com/kubeflow/community/pull/974); WG docs updated across multiple PRs: [Update WG Training charter, remove WG AutoML (#981)](https://github.com/kubeflow/community/pull/981), [Update WG Notebooks docs (#983)](https://github.com/kubeflow/community/pull/983), [Update WG ML Experience subprojects and meetings (#984)](https://github.com/kubeflow/community/pull/984), [Fix WG Data broken link and organizer list (#985)](https://github.com/kubeflow/community/pull/985), [Update KFP WG and charter (#997)](https://github.com/kubeflow/community/pull/997); website governance page fixed via [Fix website governance page (website#4398)](https://github.com/kubeflow/website/pull/4398).

- **Enhancements requested by adopters during interviews (non-blocking)**: The following improvement areas were surfaced across the two completed adopter interviews. These are not graduation blockers but are noted here for project awareness and future roadmap consideration:
  - **Helm chart for installation**: Kustomize-based installation is complex for new operators; a Helm chart would significantly lower the adoption threshold. *Maintainer response*: Helm support has been in progress for 2-3 years. Trainer and Spark Operator already have Helm charts ([trainer/charts](https://github.com/kubeflow/trainer/tree/master/charts/kubeflow-trainer), [spark-operator/charts](https://github.com/kubeflow/spark-operator/tree/master/charts/spark-operator-chart)). A GSoC 2026 project is actively working toward Helm support in the Kubeflow Community Distribution: [GSoC 2026 Project 5](https://www.kubeflow.org/events/upcoming-events/gsoc-2026/#project-5-helm-charts).
  - **Service manager / operator documentation**: Upstream docs are adequate for end users but insufficient for operators managing multi-tenant production deployments.
  - **Security: inference endpoint multi-tenancy**: Cross-namespace authorization issue in KServe/Knative - upstream: [Cross-namespace inference endpoint auth issue (knative/serving#12533)](https://github.com/knative/serving/issues/12533).
  - **Pipeline artifact multi-tenancy**: [Pipeline artifact multi-tenancy (pipelines#11760)](https://github.com/kubeflow/pipelines/issues/11760).
  - **MLMD component maintenance**: MLMD is no longer actively maintained and depends on deprecated `mysql_native_password` auth, blocking MySQL backend upgrades.
  - **Security CVE response across interconnected components**: CVE in a dependency (e.g., KServe) can block the entire platform; a security best practices document for operators was requested.
  - **More frequent releases / faster security patching**: Current release cadence can be too slow for regulated environments with aggressive patching requirements.
  - **Maintainer growth, particularly for Pipelines**: Long-term sustainability risk noted; growing the maintainer base across subprojects is an active priority.
  - **UX for non-engineer users**: A simplified UX for data scientists and business analysts with no Kubernetes background would broaden adoption.

### Adoption Evaluation

> **Status: In Progress - adopter interviews ongoing.**

Kubeflow demonstrates wide adoption across large enterprise and research organizations. Public ADOPTERS.md files show 40+ production adopters for Spark Operator, ~20 for Trainer, and strong representation from organizations across enterprise, financial services, logistics, research, and cloud provider sectors.

All 4 adopter interviews have been completed. 2 have been approved for publication (CERN, and one financial services adopter published anonymously); the remaining 2 are pending formal publication approval. The approved interviews span multiple graduation subprojects including platform-level, pipeline, training, and data workload usage patterns. Adopter interview summaries for the remaining interviews will be added to this document once publication approval is received.

### Final Assessment

> **Status: Pending - first parse complete, iteration in progress.**

Pending DD evaluation.

---

## Criteria

## Application Process Principles

### Suggested

N/A

### Required

- [X] **Give a presentation and engage with the domain specific TAG(s) to increase awareness.**

Kubeflow has presented to TAG Runtime twice:
- TAG Runtime - January 2021: [https://youtu.be/S6N8ARZZcGs](https://youtu.be/S6N8ARZZcGs)
- TAG Runtime and TOC AI Initiatives - November 2024: [https://youtu.be/u4Mf3Jh8v2E?t=2243](https://youtu.be/u4Mf3Jh8v2E?t=2243)

The November 2024 presentation covered project overview, 2024 highlights, a live fine-tuning demo, and named graduation as a 2025/2026 goal. No concerns or action items were raised by TAG Runtime.

- [X] **TAG provides insight/recommendation of the project in the context of the landscape.**

TAG Runtime provided a positive recommendation for Kubeflow's graduation readiness based on the November 2024 presentation ([https://youtu.be/u4Mf3Jh8v2E?t=2243](https://youtu.be/u4Mf3Jh8v2E?t=2243)) and review of the application materials.

- [X] **All project metadata and resources are [vendor-neutral](https://contribute.cncf.io/maintainers/community/vendor-neutrality/).**

The KSC charter enforces a maximum of 1 seat per organization across all 5 KSC seats. Current KSC composition (verified 2026-06-11): Andrey Velichkevich (Apple), Chase Christensen (Wiz), Francisco Arceo (Red Hat), Julius von Kohout (DHL), Mathew Wicks (NVIDIA) - 5 seats, 5 unique organizations. The KOC (Outreach Committee) similarly enforces a maximum of 1 Chair per org. The 2026 election completed on schedule ([2026 KSC election issue (community#950)](https://github.com/kubeflow/community/issues/950)) with the previous Red Hat dual-seat and stale KEP language concerns resolved via [Add 2026 KSC election results (community#956)](https://github.com/kubeflow/community/pull/956) and [Consolidate KSC org-limit rule (community#957)](https://github.com/kubeflow/community/pull/957).

- [X] **Review and acknowledgement of expectations for sandbox projects and requirements for moving forward through the CNCF Maturity levels.**
  - [X] Acknowledged in the graduation application body (September 2025) per CNCF application requirements.

Completion of this due diligence document, resolution of concerns raised, and presentation for public comment satisfies the Due Diligence Review criterion.

- [X] **Additional documentation as appropriate for project type, e.g.: installation documentation, end user documentation, reference implementation and/or code samples.**

All 6 graduation subprojects have dedicated documentation pages on kubeflow.org with installation guides, user guides, operator guides, and reference documentation. The [kubeflow.org docs site](https://www.kubeflow.org/docs/) is actively maintained. The [General Technical Review](https://github.com/kubeflow/community/blob/master/KUBEFLOW-GENERAL-TECHNICAL-REVIEW.md) (GTR) provides an extensive technical reference. Kubeflow Notebooks has an architectural dependency on Kubeflow Central Dashboard and cannot be deployed standalone - this is a known design characteristic, not a documentation gap.

## Governance and Maintainers

### Suggested

- [X] **Governance has continuously been iterated upon by the project as a result of their experience applying it, with the governance history demonstrating evolution of maturity alongside the project's maturity evolution.**

The Kubeflow governance model has evolved alongside the project: from a single Google-donated project to a multi-org KSC structure, introduction of the KOC for outreach, introduction of formal WG lifecycle docs, KEP process for proposals, and most recently a formal subproject application process and ecosystem membership process. The history of governance PRs in kubeflow/community demonstrates ongoing iteration.

### Required

- [X] **Clear and discoverable project governance documentation.**

[GOVERNANCE.md](https://github.com/kubeflow/community/blob/master/GOVERNANCE.md) exists at the community repo root and links to all key governance documents: [KSC charter](https://github.com/kubeflow/community/blob/master/committee-steering/charter.md), [KOC charter](https://github.com/kubeflow/community/blob/master/committee-outreach/charter.md), [WG governance](https://github.com/kubeflow/community/blob/master/wg-governance.md), contributor ladder, and code of conduct. The kubeflow.org [governance page](https://www.kubeflow.org/docs/about/governance/) is linked from the website.

- [X] **Governance is up to date with actual project activities, including any meetings, elections, leadership, or approval processes.**

KSC elections and membership are current (2026 election completed). WG governance docs have been fully refreshed: defunct WGs (wg-deployment, wg-serving, wg-manifests, sig-feature-store, sig-onprem) removed via [Remove outdated WGs/SIGs (community#974)](https://github.com/kubeflow/community/pull/974); WG READMEs, charters, and wgs.yaml updated with current meetings, organizers, and CNCF Slack links across multiple PRs ([Update WG Training charter, remove WG AutoML (#981)](https://github.com/kubeflow/community/pull/981), [Update WG Notebooks docs (#983)](https://github.com/kubeflow/community/pull/983), [Update WG ML Experience subprojects and meetings (#984)](https://github.com/kubeflow/community/pull/984), [Fix WG Data broken link and organizer list (#985)](https://github.com/kubeflow/community/pull/985), [Update KFP WG and charter (#997)](https://github.com/kubeflow/community/pull/997)); website governance page synced via [Fix website governance page (website#4398)](https://github.com/kubeflow/website/pull/4398). Resolved via [WG docs need to reflect current subproject ownership (community#967)](https://github.com/kubeflow/community/issues/967) and [WG README files have stale and broken links (community#969)](https://github.com/kubeflow/community/issues/969).

- [X] **Governance clearly documents [vendor-neutral](https://contribute.cncf.io/maintainers/community/vendor-neutrality/) of project direction.**

The KSC charter documents an explicit 1-seat-per-organization cap for all 5 KSC seats, enforced at election time. Current composition: 5 seats, 5 unique organizations (Apple, Wiz, Red Hat, DHL, NVIDIA). The KOC charter similarly caps Chair representation. Note: LF Insights shows Red Hat as the top contributor by commit volume - notable technical concentration, but governance capture is structurally prevented by the representation rules.

- [X] **Document how the project makes decisions on leadership, contribution acceptance, requests to the CNCF, and changes to governance or project goals.**

Decision-making is documented across three processes: (1) KSC decisions ([committee-steering/charter.md](https://github.com/kubeflow/community/blob/master/committee-steering/charter.md)) - Normal Decisions (quorum + majority) and Special Decisions (70% threshold) for governance/charter changes; (2) [KEP process](https://github.com/kubeflow/community/tree/master/proposals) for user/operator-facing or major architectural changes; (3) [Ecosystem join process](https://github.com/kubeflow/community/tree/master/ecosystem) for external project partnerships (KSC vote required).

- [X] **Document how role, function-based members, or sub-teams are assigned, onboarded, and removed for specific teams (example: Security Response Committee).**

The [Kubeflow community page](https://www.kubeflow.org/docs/about/community/) and [Contributing](https://www.kubeflow.org/docs/about/contributing/) page provide the public entry point, while the [Kubeflow contributor ladder](https://github.com/kubeflow/community/blob/master/community-membership.md) defines how Members, Reviewers, and Approvers are onboarded and removed. The [Kubeflow governance page](https://www.kubeflow.org/docs/about/governance/) and refactored [wg-governance.md](https://github.com/kubeflow/community/blob/master/committee-steering/wg-governance.md) document WG Chair selection, responsibilities, privileges, and inactive Chair removal. Chairs must be at least a community Member, hold a documented subproject role, have sustained contributions, be sponsored by a member, and be confirmed by super-majority vote of existing Chairs. All private Google Doc references removed. Resolved via [Refactor WG governance and Chair requirements (community#989)](https://github.com/kubeflow/community/pull/989).

- [X] **Document complete list of current maintainers, including names, contact information, domain of responsibility, and affiliation.**

[MAINTAINERS.md](https://github.com/kubeflow/community/blob/master/MAINTAINERS.md) links to the KSC member list, KOC member list, WG chairs/leads in `wgs.yaml`, and per-subproject OWNERS files. The KSC and KOC lists include names, GitHub handles, organizations, and terms. Staleness in `wgs.yaml` is being addressed by [Remove outdated WGs/SIGs (community#974)](https://github.com/kubeflow/community/pull/974).

- [X] **A number of active maintainers which is appropriate to the size and scope of the project.**

[MAINTAINERS.md](https://github.com/kubeflow/community/blob/master/MAINTAINERS.md) covers governance-level maintainers (KSC and KOC) and links to per-subproject OWNERS files for approver-level maintainers. All 6 graduation subprojects have active approvers listed in their respective OWNERS files. The maintainer count is appropriate for a project of Kubeflow's size and scope.

- [X] **Document a complete maintainer lifecycle process (including roles, onboarding, offboarding, and emeritus status).**

The [contributor ladder](https://github.com/kubeflow/community/blob/master/community-membership.md) defines the full lifecycle: onboarding criteria for each role (Member -> Reviewer -> Approver), offboarding (12-month inactivity -> org removal; `emeritus_approvers` for inactive approvers), and WG Lead/Chair removal via super-majority vote.

- [X] **Demonstrate usage of the maintainer lifecycle with outcomes, either through the addition or replacement of maintainers as project events have required.**

Addition examples (all verified merged 2025-2026):
- [Add @mprahl and @zazulam as KFP maintainers (pipelines#12059)](https://github.com/kubeflow/pipelines/pull/12059) - Added @mprahl + @zazulam as KFP maintainers with community announcement
- [Add @Electronic-Waste as approver, @astefanutti as reviewer (trainer#2659)](https://github.com/kubeflow/trainer/pull/2659) - Added with explicit criteria verification against the membership page
- [Add @Al-Pragliola as approver (hub#1153)](https://github.com/kubeflow/hub/pull/1153) - Added with full checklist verification and linked internal-acls PR

Removal example:
- [@zw0610 moves to emeritus_approvers (trainer#2343)](https://github.com/kubeflow/trainer/pull/2343) - @zw0610 self-removed to `emeritus_approvers`

- [X] **Project maintainers from at least 2 organizations that demonstrates survivability.**

Maintainer org diversity is broad across all graduation subprojects, with approvers spanning a wide range of organizations ([LFX Insights](https://insights.lfx.dev/foundation/cncf/overview/github?project=kubeflow)). Org affiliation for governance-level maintainers is documented in the KSC and KOC member lists linked from [MAINTAINERS.md](https://github.com/kubeflow/community/blob/master/MAINTAINERS.md), and for WG leads/chairs in [wgs.yaml](https://github.com/kubeflow/community/blob/master/wgs.yaml). No subproject is controlled by a single organization. WG Notebooks leadership was expanded via [Update WG Notebooks docs (community#983)](https://github.com/kubeflow/community/pull/983), resolving a prior single-org concern.

- [X] **Code and Doc ownership in Github and elsewhere matches documented governance roles.**

Kubeflow uses a GitOps ACL system ([kubeflow/internal-acls](https://github.com/kubeflow/internal-acls)) via Peribolos and Prow: org membership, team membership, and repo permissions are declared in `github-orgs/kubeflow/org.yaml` and reconciled against GitHub. The KSC team, WG lead teams, and security-team are declared in org.yaml and match governance documents. Per-repo code ownership is enforced via OWNERS files (Prow `lgtm` + `approve`). `default_repository_permission: read` enforces least privilege.

- [X] **Document agreement that project will adopt CNCF Code of Conduct.**

The CNCF Code of Conduct is adopted and documented at [kubeflow.org/docs/about/community/#code-of-conduct](https://www.kubeflow.org/docs/about/community/#code-of-conduct), and cross-linked from GOVERNANCE.md and WG governance docs.

- [X] **CNCF Code of Conduct is cross-linked from other governance documents.**

The CNCF CoC is referenced in GOVERNANCE.md, wg-governance.md, and individual WG charters. As of 2026-06-18, standalone `CODE_OF_CONDUCT.md` files are present in all 7 graduation subproject repos: community, spark-operator, trainer, katib, notebooks, hub, and pipelines. Resolved via [kubeflow/community#976](https://github.com/kubeflow/community/issues/976).

- [X] **All subprojects, if any, are listed.**

The 6 graduation subprojects are listed consistently across the graduation application, GTR, kubeflow.org architecture page, `wgs.yaml`, and `internal-acls/org.yaml`:
1. Kubeflow Trainer - [kubeflow/trainer](https://github.com/kubeflow/trainer)
2. Kubeflow Pipelines - [kubeflow/pipelines](https://github.com/kubeflow/pipelines)
3. Kubeflow Katib - [kubeflow/katib](https://github.com/kubeflow/katib)
4. Kubeflow Notebooks - [kubeflow/notebooks](https://github.com/kubeflow/notebooks)
5. Kubeflow Spark Operator - [kubeflow/spark-operator](https://github.com/kubeflow/spark-operator)
6. Kubeflow Hub - [kubeflow/hub](https://github.com/kubeflow/hub)

The subproject add/remove process is documented in [community/subprojects/README.md](https://github.com/kubeflow/community/tree/master/subprojects) and is directly linked from the [kubeflow.org introduction page](https://www.kubeflow.org/docs/started/introduction/#kubeflow-subprojects).

- [X] **If the project has subprojects: subproject leadership, contribution, maturity status documented, including add/remove process.**

**Add process:** Documented in [community/subprojects/README.md](https://github.com/kubeflow/community/tree/master/subprojects): GitHub issue -> proposal doc -> community call demo -> PR -> KSC vote -> repo transfer. Prior applications (spark-operator, model-registry) are archived there.

**Remove/retire process:** Documented in [wgs/wg-lifecycle.md](https://github.com/kubeflow/community/blob/master/wgs/wg-lifecycle.md): WG retirement triggers (3 months without quorum -> should retire; 6 months -> must retire), archiving steps, and KSC final vote.

**Contribution docs:** All 6 subprojects have `CONTRIBUTING.md` files (verified 2026-06-16).

**Maturity/roadmap:** All 6 subprojects have `ROADMAP.md`. Subproject maturity levels are being introduced via [Add subproject maturity levels (community#965)](https://github.com/kubeflow/community/pull/965).

## Contributors and Community

### Suggested

- [X] **Contributor ladder with multiple roles for contributors.**

The [contributor ladder](https://github.com/kubeflow/community/blob/master/community-membership.md) defines 4 levels: Member -> Reviewer -> Approver -> WG Lead/Chair, each with documented requirements, responsibilities, and privileges. Onboarding and offboarding at each step are described.

### Required

- [X] **Clearly defined and discoverable process to submit issues or changes.**

Issue submission guidance is at [kubeflow.org/docs/about/contributing/#starter-issues](https://www.kubeflow.org/docs/about/contributing/#starter-issues). Change proposals follow the [KEP process](https://github.com/kubeflow/community/tree/master/proposals) with a documented lifecycle (provisional -> implementable -> implemented) and PR template.

- [X] **Project must have, and document, at least one public communications channel for users and/or contributors.**

Kubeflow uses CNCF Slack with dedicated subproject channels. Channels and entry points are documented at [kubeflow.org/docs/about/community/#slack-channels](https://www.kubeflow.org/docs/about/community/#slack-channels). The [kubeflow-discuss mailing list](https://groups.google.com/g/kubeflow-discuss) is also documented.

- [X] **List and document all project communication channels, including subprojects (mail list/slack/etc.). List any non-public communications channels and what their special purpose is.**

The [community page](https://www.kubeflow.org/docs/about/community/) lists all public channels: CNCF Slack channels, kubeflow-discuss mailing list, YouTube channels, social media, and community meetings calendar. The non-public channel (KSC private mailing list: `ksc@kubeflow.org`) is documented with its purpose (private KSC deliberation and security escalation).

- [X] **Up-to-date public meeting schedulers and/or integration with CNCF calendar.**

Community-level meeting calendar is published and integrated with CNCF/LFX calendar at [kubeflow.org/docs/about/community/#list-of-available-meetings](https://www.kubeflow.org/docs/about/community/#list-of-available-meetings). WG-level meeting metadata was refreshed via [WG docs need to reflect current subproject ownership (community#967)](https://github.com/kubeflow/community/issues/967) and [WG README files have stale and broken links (community#969)](https://github.com/kubeflow/community/issues/969) - broken Zoom/calendar links, stale Slack workspace references, and stale organizer handles updated across all active WGs.

- [X] **Documentation of how to contribute, with increasing detail as the project matures.**

Central contributing guide at [kubeflow.org/docs/about/contributing/](https://www.kubeflow.org/docs/about/contributing/). All 6 graduation subprojects have `CONTRIBUTING.md` files in their repos with subproject-specific contribution guidance (verified 2026-06-17).

- [X] **Demonstrate contributor activity and recruitment.**

LF Insights shows strong contributor activity across a wide range of organizations, with positive YoY growth and healthy contributor retention. Recent maintainer additions across multiple subprojects demonstrate active recruitment (trainer#2659, pipelines#12059, hub#1153).

## Engineering Principles

### Suggested

N/A

### Required

- [X] **Document project goals and objectives that illustrate the project's differentiation in the Cloud Native landscape as well as outlines how this project fulfills an outstanding need and/or solves a problem differently.**

Addressed by the [GTR](https://github.com/kubeflow/community/blob/master/KUBEFLOW-GENERAL-TECHNICAL-REVIEW.md) (lines 13-152): Kubeflow is positioned as a "foundation of tools for AI Platforms on Kubernetes," differentiated by its composability, modularity, Kubernetes-native design, and support for the full ML lifecycle. Target personas (data scientists, ML engineers, platform engineers, vendors) and primary use cases (distributed training, fine-tuning, HPO, pipelines, serving) are explicitly documented, along with unsupported use cases (no GitOps implementation, no infrastructure beyond Kubernetes).

- [X] **Document what the project does, and why it does it - including viable cloud native use cases.**

Addressed by the [GTR](https://github.com/kubeflow/community/blob/master/KUBEFLOW-GENERAL-TECHNICAL-REVIEW.md) (lines 82-152): primary use cases include large-scale data processing, distributed pre-training of foundation models, LLM fine-tuning, hyperparameter optimization, end-to-end GenAI pipelines, interactive AI development, and multi-tenancy. The [kubeflow.org architecture page](https://www.kubeflow.org/docs/started/architecture/) with the AI lifecycle diagram provides the user-facing project overview.

- [X] **Document and maintain a public roadmap or other forward looking planning document or tracking mechanism.**

All 6 graduation subprojects now have `ROADMAP.md` files. `kubeflow/notebooks` ROADMAP.md was added via [Add ROADMAP.md to notebooks (notebooks#1188)](https://github.com/kubeflow/notebooks/pull/1188). Resolved via [kubeflow/community#988](https://github.com/kubeflow/community/issues/988).

- [X] **Roadmap change process is documented.**

Community-wide changes use the [KEP process](https://github.com/kubeflow/community/tree/master/proposals) (proposal -> community review -> implementation). Subproject-specific proposals are managed in subproject KEP directories (e.g., [trainer/docs/proposals](https://github.com/kubeflow/trainer/tree/master/docs/proposals)). The full KEP lifecycle (provisional -> implementable -> implemented) and template are documented.

- [X] **Document overview of project architecture and software design that demonstrates viable cloud native use cases, as part of the project's documentation.**

Architecture documentation is comprehensive: the [GTR](https://github.com/kubeflow/community/blob/master/KUBEFLOW-GENERAL-TECHNICAL-REVIEW.md) covers design principles, architecture requirements, service dependencies, IAM design, API topology, and release process. The [kubeflow.org architecture page](https://www.kubeflow.org/docs/started/architecture/) includes an AI lifecycle diagram and component descriptions. The [Kubeflow Community Distribution release pages](https://www.kubeflow.org/docs/kubeflow-distribution/releases/) provide per-release component version matrices.

- [ ] **Document the project's release process and guidelines publicly in a RELEASES.md or equivalent file that defines:**
  - [X] Release expectations (scheduled or based on feature implementation)
  - [X] Tagging as stable, unstable, and security related releases
  - [X] Information on branch and tag strategies
  - [X] Branch and platform support and length of support
  - [X] Artifacts included in the release.

All 6 graduation subprojects have `RELEASE.md` or equivalent. `kubeflow/notebooks` `RELEASE.md` was added via [Add RELEASE.md to notebooks (notebooks#1189)](https://github.com/kubeflow/notebooks/pull/1189); it points to detailed step-by-step release docs (minor/patch/RC/GA, signed tagging, artifact updates) in `releasing/README.md` on both `notebooks-v1` and `notebooks-v2` branches. Resolved via [kubeflow/community#990](https://github.com/kubeflow/community/issues/990).

- [X] **History of regular, quality releases.**

All 6 graduation subprojects have consistent release histories (verified 2026-06-17):
- Trainer: v2.2.1 (2026-06-17), v2.2.0 (2026-03-19), v2.1.0 (2025-11-07)
- Pipelines: 2.16.1 (2026-05-04), 2.16.0 (2026-02-25), 2.15.x (2025-11/12)
- Spark Operator: v2.5.1 (2026-06-14), v2.5.0 (2026-03-19), v2.4.0 (2025-11-17)
- Katib: v0.19.0 (2025-10-30), v0.18.0 (2025-03-25), v0.17.0 (2024-07-12)
- Hub: v0.3.10 (2026-06-15), v0.3.9 (2026-05-04), v0.3.8 (2026-04-03)
- Notebooks: v1.11.0 (2026-06-04) + active v2.0.0-alpha line (2026 Q2)

RC/pre-release tags are used before stable releases, and patch releases are present across subprojects, indicating quality-focused release practices. The [Kubeflow Community Distribution release history](https://www.kubeflow.org/docs/kubeflow-distribution/releases/) spans from v0.6 through the current 26.03 release with detailed per-release notes.

## Security

### Suggested

- [ ] **Achieving OpenSSF Best Practices silver or gold badge.**

[Trainer](https://www.bestpractices.dev/projects/10435) and [Katib](https://www.bestpractices.dev/projects/9941) have achieved Gold.

### Required

- [X] **Clearly defined and discoverable process to report security issues.**

All 6 graduation subprojects have `SECURITY.md` files documenting: supported versions, private vulnerability reporting via GitHub Security Advisories, escalation to `ksc@kubeflow.org`, a disclosure process (acknowledgment within 10 business days, assessment, resolution, public disclosure), and explicit guidance not to use public channels. Verified across kubeflow/trainer, pipelines, katib, notebooks, spark-operator, and hub (2026-06-17).

- [X] **Enforcing Access Control Rules to secure the code base against attacks (Example: two factor authentication enforcement, and/or use of ACL tools.)**

Kubeflow uses a GitOps ACL system via [kubeflow/internal-acls](https://github.com/kubeflow/internal-acls): org membership and repo permissions are declared in `github-orgs/kubeflow/org.yaml` and reconciled by Peribolos. 2FA is required for all GitHub org members. `default_repository_permission: read` enforces least privilege.

- [X] **Document assignment of security response roles and how reports are handled.**

Security response roles are documented in each subproject's security policy: reports handled by project owners, with KSC (`ksc@kubeflow.org`) as escalation. A dedicated `security-team` is declared in `internal-acls/org.yaml`. Disclosure process (acknowledgment, investigation, resolution, public disclosure) is documented consistently across all 6 subproject policies.

- [X] **Document Security Self-Assessment.**

The [Kubeflow Security Self-Assessment](https://github.com/kubeflow/community/blob/master/security/self-assessment.md) is published in kubeflow/community, actively maintained (updated 2026), and covers all 6 graduation subprojects. Content structure follows TAG Security guidance including metadata, security links, background, actors, goals, security functions, secure development practices, and security issue resolution. The self-assessment is also merged into cncf/toc via [Kubeflow Security Self-Assessment (toc#2201)](https://github.com/cncf/toc/pull/2201).

- [X] **Third Party Security Review.**
  - [X] Moderate and low findings from the Third Party Security Review are planned/tracked for resolution.

The Ada Logics security audit (Sept 2025) is publicly available: [security/Ada_Logics-Kubeflow-security-audit-2025.pdf](https://github.com/kubeflow/community/blob/master/security/Ada_Logics-Kubeflow-security-audit-2025.pdf), published via [Publish Ada Logics security audit (community#994)](https://github.com/kubeflow/community/pull/994). All in-scope findings are resolved or tracked with linked PRs/issues; KServe findings are out of scope as KServe is an independent CNCF project. Full tracking details are in [kubeflow/community#992](https://github.com/kubeflow/community/issues/992).

- [X] **Achieve the Open Source Security Foundation (OpenSSF) Best Practices passing badge.**

All 6 graduation subprojects hold at least Passing badge (verified via bestpractices.dev, 2026-06-17):
- [Katib](https://www.bestpractices.dev/projects/9941): **Gold**
- [Trainer](https://www.bestpractices.dev/projects/10435): **Gold**
- [Notebooks](https://www.bestpractices.dev/en/projects/9942): Passing
- [Pipelines](https://www.bestpractices.dev/en/projects/9938): Passing
- [Hub](https://www.bestpractices.dev/en/projects/9937): Passing
- [Spark Operator](https://www.bestpractices.dev/en/projects/10524): Passing

## Ecosystem

### Suggested

N/A

### Required

- [X] **Publicly documented list of adopters, which may indicate their adoption level (dev/trialing, prod, etc.)**

All 6 graduation subprojects maintain public `ADOPTERS.md` files:
- [community/ADOPTERS.md](https://github.com/kubeflow/community/blob/master/ADOPTERS.md): 7 platform adopters (AT&T, CERN, DHL, Jio, Slalom, Telia, RAICS.AI)
- [Spark Operator](https://github.com/kubeflow/spark-operator/blob/master/ADOPTERS.md): 40+ adopters, many in Production
- [Trainer](https://github.com/kubeflow/trainer/blob/master/ADOPTERS.md): ~20 adopters (AWS, Cisco, NVIDIA, Bloomberg, Red Hat, etc.)
- [Katib](https://github.com/kubeflow/katib/blob/master/ADOPTERS.md): ~12 adopters
- [Kubeflow Hub](https://github.com/kubeflow/hub/blob/main/ADOPTERS.md): 5 adopters
- [Pipelines](https://github.com/kubeflow/pipelines/blob/master/ADOPTERS.md): 4 adopters sparse for the most widely deployed subproject
- [Notebooks](https://github.com/kubeflow/notebooks/blob/main/ADOPTERS.md): 1 adopter (Red Hat only) very thin - CERN addition in progress: [Add CERN to Notebooks ADOPTERS.md (notebooks#1190)](https://github.com/kubeflow/notebooks/pull/1190)

Notebooks and Pipelines ADOPTERS.md files are sparse relative to actual deployment scale. Adopter interview evidence provides independent validation.

- [ ] **Used in appropriate capacity by at least 3 independent + indirect/direct adopters, (these are not required to be in the publicly documented list of adopters)**

> **Status: Pending - adopter interviews in progress.**

2 of 4 planned adopter interviews have been completed. Based on public ADOPTERS.md evidence alone (Spark Operator 40+, Trainer ~20, platform 7), broad production adoption is clearly evidenced in aggregate; formal TOC verification via adopter interviews is required to close this criterion. Remaining interviews are being scheduled.

- [ ] **TOC verification of adopters.**

> **Status: Pending - linked to the above criterion.**

Will be closed together with the previous item once all planned interviews are complete and TOC confirms at least 3 independent production adopters across the graduation subprojects.

#### Adoption

> 1 of 4 adopter interviews has been approved for publication. 1 additional completed interview is pending adopter approval. 2 further interviews are being scheduled. Full adoption details will be recorded in this section prior to the graduation vote.

##### Adopter 1 - CERN/Scientific research organization

This adopter interview was conducted in June 2026 and recorded a strong production adopter running Kubeflow at scale across Notebooks, KServe, Trainer, Katib, and Pipelines, with plans to expand to thousands of users as part of a 3-5 year AI strategy. Refer to the [interview summary](adopter-interviews/CERN-adopter-interview.md) for more details.

##### Adopter 2 - Pending adopter approval for publication

##### Adopter 3 - Pending scheduling

##### Adopter 4 - Pending scheduling

- [X] **Clearly documented integrations and/or compatibility with other CNCF projects as well as non-CNCF projects.**

Kubeflow's integration documentation is organized per subproject (each has dedicated integration guides) rather than a single consolidated page. Maintainer confirmation (Andrey Velichkevich, 2026-06-17): "every Kubeflow subproject has its own list of integrations with other CNCF projects." An [Ecosystem page](https://www.kubeflow.org/docs/ecosystem/) provides a top-level view of ecosystem partners.

Per-subproject integration evidence (verified 2026-06-17):

| Subproject | Integration documented | Link |
|---|---|---|
| **Trainer** | Volcano, Kueue (job scheduling) | [Job Scheduling guide](https://www.kubeflow.org/docs/components/trainer/operator-guides/job-scheduling/) |
| **Trainer** | PyTorch, DeepSpeed, JAX, HuggingFace, XGBoost, MLX, Arrow, DataFusion | [Overview](https://www.kubeflow.org/docs/components/trainer/overview/) |
| **Spark Operator** | YuniKorn | [YuniKorn integration](https://www.kubeflow.org/docs/components/spark-operator/user-guide/yunikorn-integration/) |
| **Notebooks** | Jupyter, TensorFlow | [Jupyter + TF examples](https://www.kubeflow.org/docs/components/notebooks/jupyter-tensorflow-examples/) |
| **Hub** | KServe (CNCF Incubating) | [Hub getting-started](https://www.kubeflow.org/docs/components/hub/getting-started/#using-model-registry-metadata) |
| **Pipelines** | SeaweedFS / S3-compatible stores | [Object store config](https://www.kubeflow.org/docs/components/pipelines/operator-guides/configure-object-store/) |
| **Katib** | Argo Workflows (CNCF Graduated) | [Trial template guide](https://www.kubeflow.org/docs/components/katib/user-guides/trial-template/) |

CNCF projects integrated across subprojects (non-exhaustive): Kubernetes, Argo Workflows, Istio, Cert-Manager, Knative, Kueue, JobSet, Volcano, OpenTelemetry, Envoy, Prometheus, KEDA.

Non-CNCF projects integrated across subprojects (non-exhaustive): PyTorch, DeepSpeed, JAX, Jupyter, Apache Spark, Apache Arrow, Apache DataFusion, Horovod, MLX, XGBoost, HuggingFace, SeaweedFS, YuniKorn, TensorFlow, vLLM.
