# Buildpacks Graduation Due Diligence

- Link to [cncf/toc/issues#1538](https://github.com/cncf/toc/issues/1538)

<!-- This template provides the TOC with the outline for completing due diligence of a project to move levels. This universal template is designed to capture all criteria so the TOC may ensure prior level criteria do not regress. As part of completing the due diligence, the TOC member should update the template to convey the level the project applied for the criteria by bolding the level indicated where the criteria is relevant. -->

## Graduation Evaluation Summary for $PROJECT

### Criteria Evaluation

_$TOCMEMBER conducted the due diligence of $PROJECT who applied for $LEVEL. The project [has/has not] completed the criteria that show its maturity at $LEVEL. The following criteria implementations are noteworthy to call out... $NOTABLES. The following actions were provided to the project that were considered blocking but since resolved... $BLOCKERS. The following recommendations were provided to the project that are non-blocking in the TOC's assessment but should be completed by the project to ensure continued viability of the project... $RECOMMENDATIONS._

### Adoption Evaluation

_The adopter interviews reflect a project [in use/too early] for the level which the project applied. They show ... $INTERVIEWSUMMARY._

### Final Assessment

_[The TOC has found the project to have satisfied the criteria for $LEVEL/ The TOC's evaluation of the project shows a needed focus to complete the outstanding blockers and reapply when the following conditions are met ... $CONDITIONS]._

### Criteria

## Application Process Principles

### Suggested

N/A

### Required

- [x] **Engage with the domain specific TAG(s) to increase awareness through a presentation or completing a General Technical Review.**

<!-- (TOC Evaluation goes here) -->

  - Tech Review request: https://github.com/cncf/toc/issues/1983
  - Initial version of the graduation Tech Review (GTR): https://github.com/cncf/toc/pull/2047

- [ ]  **All project metadata and resources are [vendor-neutral](https://contribute.cncf.io/maintainers/community/vendor-neutrality/).**

<!-- (TOC Evaluation goes here) -->

Buildpacks operates under vendor-neutral governance guided by its Technical Oversight Committee, and project communication/messaging/collaboration and support resources are vendor-neutral, with the following references:
- https://github.com/buildpacks/community/blob/main/TEAMS.md#technical-oversight-committee
- GitHub org(s): https://github.com/buildpacks, https://github.com/buildpacks-community
- Website: https://buildpacks.io/
- Slack: https://slack.buildpacks.io/

- Vendor-neutrality concern being tracked publicly: https://github.com/buildpacks/community/issues/281

- [x] **Review and acknowledgement of expectations for [Sandbox](sandbox.cncf.io) projects and requirements for moving forward through the CNCF Maturity levels.**		

<!-- (TOC Evaluation goes here) -->

   - Met during initial application on 31-08-2018.
   - Additional review/acknowledgement: TOC sponsor kickoff meeting with Buildpacks maintainers on 2025-12-16 to set Graduation expectations.

Acknowledgement evidence against prior CNCF TOC artifacts:
- Sandbox proposal PR: https://github.com/cncf/toc/pull/150
- Incubation review PR: https://github.com/cncf/toc/pull/338
- Process / criteria references:
  - https://github.com/cncf/toc/blob/main/process/README.md
  - https://github.com/cncf/toc/blob/main/process/graduation_criteria.md

- [ ] **Due Diligence Review.**

<!-- (TOC Evaluation goes here) -->

Completion of this due diligence document, resolution of concerns raised, and presented for public comment satisfies the Due Diligence Review criteria.

- [x] **Additional documentation as appropriate for project type, e.g.: installation documentation, end user documentation, reference implementation and/or code samples.**

<!-- (TOC Evaluation goes here) -->

Documentation links for this criterion:
- Installation documentation: https://buildpacks.io/docs/app-journey/
- Contributing/community documentation: https://buildpacks.io/community/#contributing
- “Cloud Native Buildpacks Incubation Due Diligence” (Google Doc): https://docs.google.com/document/d/1tb3mK5cJmaQLO8xR__9NaH2GMrdn3WPjAZFBJYsXrxY/edit?usp=sharing

## Governance and Maintainers

Note: this section may be augmented by the completion of a Governance Review from the Project Reviews subproject.

### Suggested

- [x]  **Governance has continuously been iterated upon by the project as a result of their experience applying it, with the governance history demonstrating evolution of maturity alongside the project's maturity evolution.**

<!-- (TOC Evaluation goes here) -->

  - [GOVERNANCE.md in buildpacks/community](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md) documents formal governance structure including teams, roles, voting, RFC process, and vendor-neutrality commitments.
  - [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) and emeritus status demonstrate active evolution; substantial emeritus membership indicates role transitions and project maturation over time.

Governance structure is documented and has evolved to include Team Leads, Special Teams (Security Response), and explicit role definitions. Project demonstrates iterative governance through RFC process and role transitions/promotions. SATISFIED.

### Required

- [x] **Clear and discoverable project governance documentation.**

<!-- (TOC Evaluation goes here) -->

  - [GOVERNANCE.md in buildpacks/community](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md) provides comprehensive governance documentation (repositories, TOC, teams, roles, voting, RFC process, emergencies, vendor-neutrality, security, updating governance).
  - [README.md](https://github.com/buildpacks/community/blob/main/README.md) links to [GOVERNANCE.md](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md), making it highly discoverable.

[GOVERNANCE.md](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md) is comprehensive, well-organized, and clearly linked from community [README.md](https://github.com/buildpacks/community/blob/main/README.md). SATISFIED.

- [x] **Governance is up to date with actual project activities, including any meetings, elections, leadership, or approval processes.**

<!-- (TOC Evaluation goes here) -->

  - Technical Oversight Committee details documented in [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md#technical-oversight-committee) with current member list and GitHub handles.
  - Committee activities tracked in [buildpacks/community Issues](https://github.com/buildpacks/community/issues), [Discussions](https://github.com/buildpacks/community/discussions), and [RFCs](https://github.com/buildpacks/rfcs).
  - TOC meetings are public with notes documented; [community calendar](https://buildpacks.io/community/) lists meeting times.
  - Team Leads, maintainers, and component maintainers documented in [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) with current membership and contact information.

[TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) and public issue/RFC tracking confirm governance structures are actively used and documented with current practices and personnel. SATISFIED.

- [ ] **Governance clearly documents [vendor-neutrality](https://contribute.cncf.io/maintainers/community/vendor-neutrality/) of project direction.**

<!-- (TOC Evaluation goes here) -->

  - [GOVERNANCE.md#vendor-neutrality](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md#vendor-neutrality) documents vendor-neutrality commitment: "No company may hold a majority of TOC seats" with max 2 seats from any one organization.
  - [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) displays TOC with explicit affiliation table: 3 active members (Heroku/Salesforce, Salesforce, Bloomberg) + 2 vacant seats ([buildpacks/community/pull#288](https://github.com/buildpacks/community/pull/288), [buildpacks/community/pull#290](https://github.com/buildpacks/community/pull/290) merged 2 days ago).
  - **Critical Gap:** TOC seat structure increased to 5, but **no documented process or timeline for filling vacant seats from new organizations**. Heroku/Salesforce are related companies per CNCF charter; genuine vendor-neutrality improvement requires seats filled by distinct organizations with transparent community engagement.

Vendor-neutrality rule is documented (satisfies transparency requirement), but vacant seats remain unfilled with no recruitment process documented. **BLOCKING**: Project must provide documented TOC recruitment process and timeline for filling seats from additional organizations to demonstrate genuine vendor-neutral governance. NOT SATISFIED pending recruitment process and seat filling.

- [ ] **Document how the project makes decisions on leadership, contribution acceptance, requests to the CNCF, and changes to governance or project goals.**

<!-- (TOC Evaluation goes here) -->

  - Changes to leadership roles, contribution acceptance, and governance follow the [RFC process](https://github.com/buildpacks/rfcs#rfc-process) per [GOVERNANCE.md#rfc-process](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md#rfc-process).
  - Voting rules are documented in multiple sections: [lazy consensus model](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md#voting-rules) (no votes against + at least one vote in favor = passes) and a separate governance-update rule: "All substantive changes in Governance require a supermajority agreement by the TOC."
  - TOC nomination and election process for leadership: "New TOC members must be nominated by an existing TOC member and elected by a super-majority of the TOC."
  - Maintainer nomination/election process documented: "New maintainers must already be contributors, must be nominated by an existing maintainer, and must be elected by a supermajority of CNB Team Leads and the TOC."
  - RFC process for major governance changes: "All substantive changes in Governance require a supermajority agreement by the TOC."

Decision-making mechanisms exist, but they are fragmented across sections and create ambiguity (for example, lazy consensus vs supermajority for governance changes). The project should consolidate and cross-link a single decision matrix clarifying: (1) which actions use lazy consensus, (2) which require supermajority, (3) who has binding vote authority, and (4) where outcomes are recorded. PARTIALLY SATISFIED / NOT FULLY SATISFIED pending consolidation.

- [ ] **Document how role, function-based members, or sub-teams are assigned, onboarded, and removed for specific teams (example: Security Response Committee).**

<!-- (TOC Evaluation goes here) -->

  - Roles documented: Team Lead, Maintainer, Component Maintainer, Contributor, TOC member; nomination and election processes defined for each.
  - All team roles described in [GOVERNANCE.md#teams](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md#teams) and [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md).
  - Security Response Team: [GOVERNANCE.md#security](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md#security) documents that it "is composed of all members of the Technical Oversight Committee and all Team Leads" and is "responsible for handling security vulnerabilities."
  - Resolution progress from [buildpacks/community/pull#291](https://github.com/buildpacks/community/pull/291) (linked from [buildpacks/community/issues#282](https://github.com/buildpacks/community/issues/282)):
    - Added explicit contributor ladder and role-summary matrix in [contributors/guide.md](https://github.com/buildpacks/community/blob/main/contributors/guide.md) (Contributor → Project Contributor → Maintainer → Team Lead → TOC).
    - Added Team Lead appointment and Release Manager responsibilities in [GOVERNANCE.md](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md).
    - Added Security section in [GOVERNANCE.md](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md), including Security Response Team composition and 2FA requirement for elevated permissions.
  - Remaining gap:
    - Role and sub-team lifecycle is clearer, but governance still lacks a single consolidated section that fully defines selection/removal/review cadence for all elevated roles and special teams in one authoritative place.

[buildpacks/community/issues#282](https://github.com/buildpacks/community/issues/282) is substantially addressed by [buildpacks/community/pull#291](https://github.com/buildpacks/community/pull/291) (ladder, role matrix, security-role documentation, and elevated-access expectations). Remaining concern is primarily consolidation/readability rather than absence of process. PARTIALLY SATISFIED with notable progress; acceptable to close once maintainers confirm final consolidation intent for role lifecycle references.

- [x] **Document a complete maintainer lifecycle process (including roles, onboarding, offboarding, and emeritus status).**

<!-- (TOC Evaluation goes here) -->

  - [GOVERNANCE.md#maintainers](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md#maintainers): "New maintainers must already be contributors, must be nominated by an existing maintainer, and must be elected by a supermajority of CNB Team Leads and the TOC. Likewise, maintainers may resign or be removed by a super-majority of Team Leads and the TOC."
  - Emeritus process: [GOVERNANCE.md#emeritus](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md#emeritus) documents self-nomination path, 3-month inactivity threshold, and reactivation process. "Out of courtesy, a notice for nomination should be given to members that fall under this category prior to being nominated."
  - Onboarding guidance: [contributors/guide.md](https://github.com/buildpacks/community/blob/main/contributors/guide.md) provides general contributor onboarding.

Maintainer lifecycle (nomination → election → removal → emeritus) is explicitly documented with clear thresholds and processes. SATISFIED.

- [x] **Demonstrate usage of the maintainer lifecycle with outcomes, either through the addition or replacement of maintainers as project events have required.**

<!-- (TOC Evaluation goes here) -->

  - [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) documents current active members and extensive emeritus lists across all teams (Implementation, Platform, Learning, Buildpack Authors' Tooling).
  - Git history examples: [buildpacks/community commit c837cd1](https://github.com/buildpacks/community/commit/c837cd15ce1e70f2a968be114b44e8f64d39a601#diff-7a8831df97c49707228dec1240256385588189e5e1bce211d5cdb23e7f94dfceR19) shows Natalieparellano progression from contributor → [commit 0fb5283](https://github.com/buildpacks/community/commit/0fb5283eb0458e655e8a65d1d6362c3d9be021c6) to maintainer → [commit ee0965f](https://github.com/buildpacks/community/commit/ee0965f6802f15e534060ba3909849d0a96b24dc) to TOC member.
  - [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) shows substantial emeritus membership, indicating the project actively uses role transitions and has experienced team evolution.

Extensive examples of role progression, role changes, and emeritus transitions are documented in [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) and git history. SATISFIED.

- [ ] **Document complete list of current maintainers, including names, contact information, domain of responsibility, and affiliation.**

<!-- (TOC Evaluation goes here) -->

  - [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) provides current TOC members, Team Leads, Maintainers, and Component Maintainers with GitHub handles and team assignments.
  - [GOVERNANCE.md#technical-oversight-committee](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md) describes TOC responsibilities and links to TEAMS.
  - Project contact is documented at [cncf-buildpacks-maintainers@lists.cncf.io](mailto:cncf-buildpacks-maintainers@lists.cncf.io).
  - **Gap:** affiliation is not presented in a complete, uniform format for all listed maintainer roles (it is explicit for TOC members, but not consistently for Team Leads/Maintainers/Component Maintainers).
  - Tracking issue: [buildpacks/community/issues#294](https://github.com/buildpacks/community/issues/294)

Names and role/domain ownership are mostly documented, but this criterion asks for complete maintainer listing including affiliation in a proper format. Current affiliation coverage is incomplete/inconsistent outside the TOC table in [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) (tracked in [buildpacks/community/issues#294](https://github.com/buildpacks/community/issues/294)). NOT YET SATISFIED until affiliation is consistently documented for all current maintainers.

- [x] **A number of active maintainers which is appropriate to the size and scope of the project.**

<!-- (TOC Evaluation goes here) -->

  - 4 active Technical Oversight Committee members (3 active; 2 vacant seats out of max 5).
  - 5 Team Leads across 5 functional teams.
  - Approximately 10+ active Maintainers across teams.
  - ~20+ Project Contributors and Component Maintainers listed in [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md).
  - Project scope: multi-component specification, reference implementation (pack, lifecycle, imgutil), registry ecosystem, documentation, and buildpack tooling. Leadership breadth (TOC, Team Leads, Maintainers across 5 teams) is appropriate to project scale and maturity.

Active maintainer count and team structure align with project scope (specification, implementations, tools, documentation, ecosystem). SATISFIED.

- [x] **Project maintainers from at least 2 organizations that demonstrates survivability.**

<!-- (TOC Evaluation goes here) -->

  - Minimum threshold is satisfied: TOC representation already spans at least 2 organizations (Heroku/Salesforce and Bloomberg) as listed in [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md#technical-oversight-committee).
  - Current TOC table also lists Salesforce separately, but related-company interpretation and broader maintainer affiliation formatting can be clarified further.
  - Additional affiliation/representation clarity is being tracked in [buildpacks/community/issues#294](https://github.com/buildpacks/community/issues/294).

Minimum survivability criterion (2 organizations) is satisfied based on current TOC composition. Additional representation/affiliation clarity can be incorporated after [buildpacks/community/issues#294](https://github.com/buildpacks/community/issues/294) is resolved.

- [x] **Code and Doc ownership in Github and elsewhere matches documented governance roles.**

<!-- (TOC Evaluation goes here) -->

  - [CODEOWNERS in buildpacks/community](https://github.com/buildpacks/community/blob/main/CODEOWNERS) assigns governance files ([GOVERNANCE.md](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md), [ROADMAP.md](https://github.com/buildpacks/community/blob/main/ROADMAP.md), OWNERS, [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md), [README.md](https://github.com/buildpacks/community/blob/main/README.md)) to @buildpacks/toc and @buildpacks/learning-maintainers.
  - All major component repositories include CODEOWNERS files (e.g., [pack](https://github.com/buildpacks/pack/blob/main/CODEOWNERS), [lifecycle](https://github.com/buildpacks/lifecycle/blob/main/CODEOWNERS)) defining ownership per documented teams.
  - GitHub Teams (e.g., @buildpacks/platform-maintainers, @buildpacks/toc) mirror documented roles in [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md).

CODEOWNERS and GitHub Teams alignment is comprehensive and matches documented governance roles. SATISFIED.

- [x] **Document adoption and adherence to the CNCF Code of Conduct or the project's CoC which is based off the CNCF CoC and not in conflict with it.**

<!-- (TOC Evaluation goes here) -->

  - [buildpacks/.github/CODE_OF_CONDUCT.md](https://github.com/buildpacks/.github/blob/main/CODE_OF_CONDUCT.md) explicitly states: "This project follows the CNCF Code of Conduct."
  - [GOVERNANCE.md](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md) references CoC: "fostering a healthy and welcoming community, including by defining and enforcing our [Code of Conduct](https://github.com/buildpacks/.github/blob/main/CODE_OF_CONDUCT.md)."
  - Remediation merged: [buildpacks/.github/pull#5](https://github.com/buildpacks/.github/pull/5) ("Fixes issue #285 update code of conduct"), updating org-level CoC to explicitly follow CNCF CoC.
  - Requested completion scope in [buildpacks/community/issues#285](https://github.com/buildpacks/community/issues/285):
    - Explicit adoption of and linkage to the CNCF Code of Conduct.
    - Ensure CNCF CoC is discoverable from root of core repositories (GitHub "Code of conduct" tab).
    - Cross-link CNCF CoC from governance and community docs.

Satisfied. Explicit CNCF CoC adoption language is now merged in [buildpacks/.github/pull#5](https://github.com/buildpacks/.github/pull/5), and governance/community docs link to this CoC. [buildpacks/community/issues#285](https://github.com/buildpacks/community/issues/285) may remain open administratively, but implementation evidence is present.

- [x] **CNCF Code of Conduct is cross-linked from other governance documents.**

<!-- (TOC Evaluation goes here) -->

  - [GOVERNANCE.md](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md) links to [buildpacks/.github/CODE_OF_CONDUCT.md](https://github.com/buildpacks/.github/blob/main/CODE_OF_CONDUCT.md).
  - [README.md](https://github.com/buildpacks/community/blob/main/README.md) also links to CoC.
  - Org-level CoC now explicitly links CNCF CoC via merged [buildpacks/.github/pull#5](https://github.com/buildpacks/.github/pull/5).
  - Related tracking context: [buildpacks/community/issues#285](https://github.com/buildpacks/community/issues/285).

Satisfied. Governance and README cross-link to project CoC, and project CoC now explicitly links CNCF CoC ([buildpacks/.github/pull#5](https://github.com/buildpacks/.github/pull/5)), establishing discoverable cross-link chain from governance documents to CNCF CoC.

- [x] **All subprojects, if any, are listed.**

<!-- (TOC Evaluation goes here) -->

  - Subprojects are organized through Teams and listed in [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md); each team documents its projects and responsibilities.
  - [buildpacks-community GitHub organization](https://github.com/buildpacks-community) hosts independent subprojects (e.g., kpack) with their own governance.
  - [GOVERNANCE.md](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md) states: "Repositories under the buildpacks organization are maintained and governed by the buildpacks project."

Subprojects are listed by team ownership in [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) and discoverable via team section in [GOVERNANCE.md](https://github.com/buildpacks/community/blob/main/GOVERNANCE.md). SATISFIED.

- [ ] **If the project has subprojects: subproject leadership, contribution, maturity status documented, including add/remove process.**

<!-- (TOC Evaluation goes here) -->

  - [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) documents team leadership and contributor roles; in practice, these teams appear to function as Buildpacks subprojects.
  - Team ownership is documented through [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) team sections and their listed projects/repositories, so subproject ownership and leadership are discoverable.
  - Formal subproject lifecycle and maturity status framework is not yet documented, including explicit add/remove workflow for subprojects.
  - No dedicated linked remediation issue/PR was identified for explicitly documenting subproject leadership model, maturity status taxonomy, and add/remove process as a single policy.

Not yet satisfied. Team ownership/leadership for subprojects is documented and discoverable, but documentation still lacks a consolidated subproject maturity framework and explicit add/remove workflow policy. [buildpacks/community/issues#282](https://github.com/buildpacks/community/issues/282) / [buildpacks/community/pull#291](https://github.com/buildpacks/community/pull/291) improved adjacent governance docs but did not fully close this specific requirement.

## Contributors and Community

Note: this section may be augmented by the completion of a Governance Review from the Project Reviews subproject.

### Suggested

- [x] **Contributor ladder with multiple roles for contributors.**

<!-- (TOC Evaluation goes here) -->

  - [contributors/guide.md](https://github.com/buildpacks/community/blob/main/contributors/guide.md) now includes an explicit contributor ladder diagram and progression path through Team Lead and TOC.
  - The same file includes a role-summary table that documents eligibility, selection, and lifecycle expectations for Project Contributor, Component Maintainer, Maintainer, Team Lead, and TOC Member.
  - This was added via [buildpacks/community/pull#291](https://github.com/buildpacks/community/pull/291), linked from [buildpacks/community/issues#282](https://github.com/buildpacks/community/issues/282).

Suggested criterion satisfied. The contributor ladder is now explicitly documented in one place with role progression and lifecycle summary.

### Required

- [x] **Clearly defined and discoverable process to submit issues or changes.**

<!-- (TOC Evaluation goes here) -->

  - [buildpacks/.github/CONTRIBUTING.md](https://github.com/buildpacks/.github/blob/main/CONTRIBUTING.md) provides a canonical pull-request process (fork, clone, branch, commit with sign-off, push, open PR) and sign-off requirements.
  - [buildpacks.io/community](https://buildpacks.io/community/) (Contributing → "How do I submit a pull request?") provides explicit pull-request submission steps (fork, clone, branch, commit sign-off, push, open PR).
  - The same guide documents multiple change paths: code, docs, RFCs, and triage; RFC change path is linked to [buildpacks/rfcs](https://github.com/buildpacks/rfcs).
  - [README.md](https://github.com/buildpacks/community/blob/main/README.md) is an entry point that links directly to the contributor guide and governance docs.

Satisfied. The process to propose and submit changes is discoverable from [README.md](https://github.com/buildpacks/community/blob/main/README.md) and documented through buildpacks.io/community contribution guidance plus [contributors/guide.md](https://github.com/buildpacks/community/blob/main/contributors/guide.md) RFC/contribution paths.

- [x] **Project must have, and document, at least one public communications channel for users and/or contributors.**

<!-- (TOC Evaluation goes here) -->

  - [buildpacks.io/community](https://buildpacks.io/community/) documents public channels including Slack (`#buildpacks`), GitHub Discussions, Mailing List, and StackOverflow.
  - [README.md](https://github.com/buildpacks/community/blob/main/README.md#meetings) documents public working-group meetings and links to attendance details.

Satisfied. Multiple public communication channels are clearly documented and discoverable.

- [ ] **List and document all project communication channels, including subprojects (mail list/slack/etc.).  List any non-public communications channels and what their special purpose is.**

<!-- (TOC Evaluation goes here) -->

  - Public channels are well documented on [buildpacks.io/community](https://buildpacks.io/community/): mailing list, GitHub discussions, StackOverflow, and multiple Slack channels (including team/scope-specific channels).
  - [README.md](https://github.com/buildpacks/community/blob/main/README.md) and the community page together cover primary working-group communication routes.
  - Private/special-purpose communication is documented for security handling in [buildpacks/.github/SECURITY.md](https://github.com/buildpacks/.github/blob/main/SECURITY.md) (private reporting and coordinated disclosure channels).
  - Remaining gap: there is no single canonical inventory that explicitly enumerates **all** channels across core/community subprojects and non-public channels with purpose in one place.

Partially satisfied / not yet fully satisfied. Public channels are documented, but a consolidated, explicit all-channels inventory (including non-public channel purpose and subproject-level mapping) is still missing.

- [x] **Up-to-date public meeting schedulers and/or integration with CNCF calendar.**

<!-- (TOC Evaluation goes here) -->

  - [buildpacks.io/community](https://buildpacks.io/community/) publishes recurring working-group meeting cadence, public Zoom links, agenda link, and a visible meeting schedule/calendar block.
  - [README.md#meetings](https://github.com/buildpacks/community/blob/main/README.md#meetings) points contributors to the public community meeting details.
  - Graduation tracking issue [buildpacks/community/issues#283](https://github.com/buildpacks/community/issues/283) was closed via [buildpacks/docs/pull#882](https://github.com/buildpacks/docs/pull/882), updating meeting-recording links to current YouTube channel and improving meeting-resource freshness.

Satisfied. Public meeting schedule and joining information are maintained on the community page, with recent graduation-tracking remediation ([buildpacks/community/issues#283](https://github.com/buildpacks/community/issues/283)) confirming active upkeep of meeting resources.

- [x] **Documentation of how to contribute, with increasing detail as the project matures.**

<!-- (TOC Evaluation goes here) -->

  - [buildpacks/.github/CONTRIBUTING.md](https://github.com/buildpacks/.github/blob/main/CONTRIBUTING.md) documents baseline contribution workflow and DCO sign-off expectations used across Buildpacks repositories.
  - [contributors/guide.md](https://github.com/buildpacks/community/blob/main/contributors/guide.md) provides structured contribution guidance across contribution types (code, docs, RFCs, triage), contributor ladder, role expectations, and FAQs.
  - Role progression and lifecycle detail was strengthened through [buildpacks/community/issues#282](https://github.com/buildpacks/community/issues/282) and [buildpacks/community/pull#291](https://github.com/buildpacks/community/pull/291).
  - [buildpacks.io/community](https://buildpacks.io/community/) provides newcomer-oriented paths (`good first issue` links, repository pointers, and contribution onboarding guidance), complementing the deeper governance/contributor docs.

Satisfied. Contribution documentation is discoverable and sufficiently detailed for multiple contributor levels, with recent graduation work (282/291) adding maturity and role clarity.

- [x] **Demonstrate contributor activity and recruitment.**

<!-- (TOC Evaluation goes here) -->

  - Recruitment pathways are actively documented: `good first issue` entry points and onboarding guidance on [buildpacks.io/community](https://buildpacks.io/community/), plus role progression in [contributors/guide.md](https://github.com/buildpacks/community/blob/main/contributors/guide.md).
  - Ongoing community activity is visible through recurring public working-group meetings and open discussion channels (Slack, mailing list, GitHub Discussions) on the community page.
  - Total developer activity momentum remains active across shorter windows using the same DevStats metric (`Contributions`, bots excluded): [Developer Activity Counts by Companies](https://buildpacks.devstats.cncf.io/d/66/developer-activity-counts-by-companies?orgId=1&var-metric=contributions) shows substantial non-zero activity in `Last year`, `Last 6 months`, and `Last month` (for example, visible top-contributor sums are at least 1,532, 475, and 127 respectively), indicating continued contribution throughput rather than a stalled project.
  - DevStats shows sustained project activity at meaningful scale: [Overall Project Statistics Table](https://buildpacks.devstats.cncf.io/d/18/overall-project-statistics-table?orgId=1) reports (bots excluded) 22,760 commits, 3,555 PRs, 3,941 issues, 948 contributors, and 70,533 contributions.
  - Recruitment signal (separate from total activity): [New Contributors Table](https://buildpacks.devstats.cncf.io/d/52/new-contributors-table?orgId=1&var-period_name=Last%20year&from=now-1y&to=now) shows 18 new contributor entries in the period (or 17 if excluding the `Copilot` entry as potential automation/service account).
  - Recent flow metrics remain active/positive: [Issues Opened/Closed by Repository Group](https://buildpacks.devstats.cncf.io/d/12/issues-opened-closed-by-repository-group?orgId=1) shows non-zero opened and closed issues/PRs with comparable opened vs closed values in the displayed 7-day moving-average view.
  - Team rosters in [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md) show active maintainers/contributors and continuing role transitions.

Satisfied. Contributor activity is positive and sustained, supported by DevStats scale metrics and ongoing opened/closed issue/PR flow, alongside explicit recruitment pathways and active community operations.

## Engineering Principles

### Suggested

N/A

### Required

**Note:** A General Technical Review was completed on 20-Feb-2026, and can be discovered at [cncf/toc/pull#2047](https://github.com/cncf/toc/pull/2047). The following criteria are satisfied through this review and supporting documentation.

- [x] **Document project goals and objectives that illustrate the project’s differentiation in the Cloud Native landscape as well as outlines how this project fulfills an outstanding need and/or solves a problem differently. _This requirement may also be satisfied by completing a General Technical Review._**

<!-- (TOC Evaluation goes here) -->

  - Satisfied via General Technical Review: [cncf/toc/pull#2047](https://github.com/cncf/toc/pull/2047).
  - The GTR captures CNB differentiation, project objectives, and why CNB addresses cloud-native build and supply-chain needs differently from Dockerfile-centric workflows.

Satisfied via GTR evidence in [cncf/toc/pull#2047](https://github.com/cncf/toc/pull/2047); technical differentiation and project objectives are documented there in detail.

- [x] **Document what the project does, and why it does it - including viable cloud native use cases. _This requirement may also be satisfied by completing a General Technical Review._**

<!-- (TOC Evaluation goes here) -->

  - Satisfied via General Technical Review: [cncf/toc/pull#2047](https://github.com/cncf/toc/pull/2047).
  - The GTR documents what CNB does, why it exists, and representative cloud-native use cases.

- [x] **Document and maintain a public roadmap or other forward looking planning document or tracking mechanism.**

<!-- (TOC Evaluation goes here) -->

  - Public Roadmap maintained at [buildpacks/community ROADMAP.md](https://github.com/buildpacks/community/blob/main/ROADMAP.md)
  - Recent planning documented in [buildpacks/rfcs/pull#325](https://github.com/buildpacks/rfcs/pull/325)
  - The Technical Oversight Committee (TOC) is explicitly responsible for roadmap direction, team leadership, and cross-cutting concerns as documented in [TEAMS.md](https://github.com/buildpacks/community/blob/main/TEAMS.md#technical-oversight-committee)
  - Discoverability gap noted in [buildpacks/community/issues#292](https://github.com/buildpacks/community/issues/292): roadmap history is not clearly presented for all expected periods (for example, 2024/2025 are not clearly discoverable from the current roadmap index/path).

Satisfied for existence of a public roadmap and ownership, with remaining discoverability gaps (including missing/unclear 2024/2025 roadmap visibility) tracked in [buildpacks/community/issues#292](https://github.com/buildpacks/community/issues/292).

- [ ] **Roadmap change process is documented.**

<!-- (TOC Evaluation goes here) -->

  - Primary gap: the end-to-end roadmap change process is not clearly documented (how changes are proposed, approved, and recorded).
  - Gap tracking issue raised: [buildpacks/community/issues#292](https://github.com/buildpacks/community/issues/292)
  - Secondary note: roadmap discoverability consistency (including 2024/2025 visibility) should be clarified as part of the same issue.
  - Expected outcome: document a clear roadmap change workflow (proposal path, approvers, decision policy, and where decisions are recorded).

Not yet satisfied. Primary blocker is lack of a directly traceable roadmap change process ([buildpacks/community/issues#292](https://github.com/buildpacks/community/issues/292)).

- [x] **Document overview of project architecture and software design that demonstrates viable cloud native use cases, as part of the project's documentation.  *This requirement may also be satisfied by completing a General Technical Review and capturing the output in the project's documentation.***

<!-- (TOC Evaluation goes here) -->

  - Satisfied via General Technical Review: [cncf/toc/pull#2047](https://github.com/cncf/toc/pull/2047)
  - Architecture-related documentation referenced in the GTR:
    - [Platform API (spec interface and architecture contract)](https://buildpacks.io/docs/reference/spec/platform-api/)
    - [Buildpack API (lifecycle/buildpack interface contract)](https://buildpacks.io/docs/reference/spec/buildpack-api/)
    - [What is the lifecycle? (phased build architecture and security boundaries)](https://buildpacks.io/docs/for-platform-operators/concepts/lifecycle/)
    - [What is a builder? (builder composition and component model)](https://buildpacks.io/docs/for-platform-operators/concepts/builder/)
    - [What is a buildpack? (detect/build behavior and transformation model)](https://buildpacks.io/docs/for-platform-operators/concepts/buildpack/)

Satisfied via the General Technical Review evidence in [cncf/toc/pull#2047](https://github.com/cncf/toc/pull/2047).

- [ ] **Document the project's release process and guidelines publicly in a [RELEASES.md](https://github.com/buildpacks/community/blob/main/RELEASES.md) or equivalent file that defines:** 

<!-- (TOC Evaluation goes here) -->

  - Gap tracking issue: [buildpacks/community/issues#295](https://github.com/buildpacks/community/issues/295) (project-wide release-process documentation gaps in top-level [RELEASES.md](https://github.com/buildpacks/community/blob/main/RELEASES.md)).

  - [x] Release expectations (scheduled or based on feature implementation)
    - Evidence: [buildpacks/community RELEASES.md](https://github.com/buildpacks/community/blob/main/RELEASES.md) documents release expectations.
  - [ ] Tagging as stable, unstable, and security related releases
    - Gap: stable/unstable guidance exists, but explicit project-wide security-release tagging guidance is not clearly documented in top-level release docs.
    - References: [buildpacks/community RELEASES.md](https://github.com/buildpacks/community/blob/main/RELEASES.md), [pack RELEASE.md](https://github.com/buildpacks/pack/blob/main/RELEASE.md), [lifecycle RELEASE.md](https://github.com/buildpacks/lifecycle/blob/main/RELEASE.md).
  - [x] Information on branch and tag strategies
    - Evidence: documented in [pack RELEASE.md](https://github.com/buildpacks/pack/blob/main/RELEASE.md), [lifecycle RELEASE.md](https://github.com/buildpacks/lifecycle/blob/main/RELEASE.md), and [spec RELEASE.md](https://github.com/buildpacks/spec/blob/main/RELEASE.md).
  - [ ] Branch and platform support and length of support
    - Gap: explicit project-wide support duration/window policy is not clearly documented in [buildpacks/community RELEASES.md](https://github.com/buildpacks/community/blob/main/RELEASES.md).
  - [x] Artifacts included in the release.
    - Evidence: release artifacts/changelogs are published in [Pack releases](https://github.com/buildpacks/pack/releases) and [Spec releases](https://github.com/buildpacks/spec/releases).

Release docs show strong component-level process detail, but top-level clarity is incomplete. Remaining gaps (security-release tagging, support-window policy, and project-wide [RELEASES.md](https://github.com/buildpacks/community/blob/main/RELEASES.md) consistency) are now tracked in [buildpacks/community/issues#295](https://github.com/buildpacks/community/issues/295).

- [x] **History of regular, quality releases.**

<!-- (TOC Evaluation goes here) -->

  - Release history start points (from GitHub Releases pages):
    - `pack`: first release [v0.0.1 (Aug 21, 2018)](https://github.com/buildpacks/pack/releases/tag/v0.0.1)
    - `lifecycle`: first release [v0.1.0 (Apr 2, 2019)](https://github.com/buildpacks/lifecycle/releases/tag/v0.1.0)
    - `spec`: early API releases visible from [Jul 16, 2020](https://github.com/buildpacks/spec/releases/tag/platform%2Fv0.3)
  - Frequency / consistency evidence:
    - `pack`: continuing releases from 2018 through 2026, including recent sequence [v0.39.0 (Nov 2025)](https://github.com/buildpacks/pack/releases/tag/v0.39.0), [v0.39.1 (Dec 2025)](https://github.com/buildpacks/pack/releases/tag/v0.39.1), [v0.40.0 (2026)](https://github.com/buildpacks/pack/releases/tag/v0.40.0)
    - `lifecycle`: frequent patch/minor cadence, e.g. [v0.20.17 (Nov 2025)](https://github.com/buildpacks/lifecycle/releases/tag/v0.20.17) through [v0.21.5 (Feb 2026)](https://github.com/buildpacks/lifecycle/releases/tag/v0.21.5)
    - `spec`: ongoing versioned API releases over multiple years, including [Platform API 0.10 (Oct 2022)](https://github.com/buildpacks/spec/releases/tag/platform%2Fv0.10), [Platform API 0.14 (Jul 2024)](https://github.com/buildpacks/spec/releases/tag/platform%2Fv0.14), [Platform API 0.15 (Dec 2025)](https://github.com/buildpacks/spec/releases/tag/platform%2F0.15)

Release history is long-lived and active across core components. Pack and lifecycle show frequent recurring releases; spec publishes versioned API releases consistently as changes are ratified.

## Security

Note: this section may be augmented by a joint-assessment performed by TAG Security and Compliance.

### Suggested

- [ ] **Achieving OpenSSF Best Practices silver or gold badge.**

<!-- (TOC Evaluation goes here) -->

Buildpacks has an OpenSSF Best Practices **passing** badge (https://www.bestpractices.dev/en/projects/4748). Silver/gold remains a non-blocking improvement target.

### Required

- [x] **Clearly defined and discoverable process to report security issues.**

<!-- (TOC Evaluation goes here) -->

Buildpacks documents a clear reporting process in [SECURITY.md](https://github.com/buildpacks/.github/blob/main/SECURITY.md) with:
- private reporting channels (GitHub Security Advisories and security@buildpacks.io),
- required report contents,
- and explicit response workflow.
- https://github.com/buildpacks/.github/blob/main/SECURITY.md
- Gap: [SECURITY.md](https://github.com/buildpacks/.github/blob/main/SECURITY.md) needed clearer report content requirements, response workflow/timelines, supported versions policy, and disclosure guidance.
- Tracking issue: https://github.com/buildpacks/community/issues/284
- Remediation merged: https://github.com/buildpacks/.github/pull/6

- [x] **Enforcing Access Control Rules to secure the code base against attacks (Example: two factor authentication enforcement, and/or use of ACL tools.)**

<!-- (TOC Evaluation goes here) -->

The project enforces access-control and repository ownership controls across Buildpacks repositories, including CODEOWNERS-based review ownership and organization/repository policy controls.
- Example CODEOWNERS usage: https://github.com/buildpacks/lifecycle/blob/main/CODEOWNERS
- Security process and disclosure governance: https://github.com/buildpacks/.github/blob/main/SECURITY.md

- [x] **Document assignment of security response roles and how reports are handled.**

<!-- (TOC Evaluation goes here) -->

[SECURITY.md](https://github.com/buildpacks/.github/blob/main/SECURITY.md) documents that the project security team (maintainers) handles reports, acknowledges reports within 72 hours, triages with assigned maintainers, coordinates fixes privately, and discloses through advisories and release notes.
- https://github.com/buildpacks/.github/blob/main/SECURITY.md
- Clarification delivered via https://github.com/buildpacks/.github/pull/6

- [x] **Document Security Self-Assessment.**

<!-- (TOC Evaluation goes here) -->

Buildpacks has a published markdown self-assessment in this CNCF-discoverable repo:
- https://github.com/cncf/toc/blob/main/projects/buildpacks/security-assessment/self-assessment.md

Related context:
- Gap: self-assessment discoverability and long-term markdown publication needed to be explicit and cross-linked.
- Tracking issue: https://github.com/buildpacks/community/issues/286
- Remediation merged (audit + self-assessment links in [SECURITY.md](https://github.com/buildpacks/.github/blob/main/SECURITY.md)): https://github.com/buildpacks/.github/pull/8
- Canonical markdown self-assessment already present in CNCF TOC repo: https://github.com/cncf/toc/blob/main/projects/buildpacks/security-assessment/self-assessment.md

- [x] **Third Party Security Review.**

<!-- (TOC Evaluation goes here) -->

Buildpacks completed a third-party security audit with OSTIF/Quarkslab and published findings publicly.
- https://ostif.org/buildpacks-audit-complete/
- https://medium.com/buildpacks/announcing-findings-from-security-audit-b4701f4e8b4b
- Audit references are now linked from [SECURITY.md](https://github.com/buildpacks/.github/blob/main/SECURITY.md) via https://github.com/buildpacks/.github/pull/8

Follow-up tracking note:
- Gap: reporting/process/security-disclosure details were incomplete in [SECURITY.md](https://github.com/buildpacks/.github/blob/main/SECURITY.md); tracked in https://github.com/buildpacks/community/issues/284 and addressed by merged PR https://github.com/buildpacks/.github/pull/6.
- Gap: explicit self-assessment/audit discoverability links were missing from [SECURITY.md](https://github.com/buildpacks/.github/blob/main/SECURITY.md); tracked in https://github.com/buildpacks/community/issues/286 and addressed by merged PR https://github.com/buildpacks/.github/pull/8.

  - [x] Moderate and low findings from the Third Party Security Review are planned/tracked for resolution as well as overall thematic findings.

    Specific tracking/remediation examples from the audit:
    - MED-1 (`Docker in-container privilege escalation`): tracked in https://github.com/buildpacks/pack/issues/2220 and implemented via merged PR https://github.com/buildpacks/pack-private/pull/29.
    - MED-2 (`permissive inter-container connectivity`): tracked in https://github.com/buildpacks/pack/issues/2219 and implemented via merged PR https://github.com/buildpacks/pack-private/pull/50 (with follow-up compatibility fix merged in https://github.com/buildpacks/pack/pull/2241).
    - LOW-4 (`data leak via cache access`): tracked in https://github.com/buildpacks/pack/issues/2224 and implemented via merged PR https://github.com/buildpacks/pack-private/pull/48.
    - LOW-1/LOW-2 (`cache-race/corrupt-cache DoS`): tracked in https://github.com/buildpacks/lifecycle/issues/1382 and related design tracking in https://github.com/buildpacks/lifecycle/issues/1383.

    Release/milestone evidence for audit remediation rollout:
    - pack 0.35.0 milestone: https://github.com/buildpacks/pack/milestone/50
    - lifecycle 0.20.0 milestone: https://github.com/buildpacks/lifecycle/milestone/41

- [x] **Achieve the Open Source Security Foundation (OpenSSF) Best Practices passing badge.**

<!-- (TOC Evaluation goes here) -->

Buildpacks has achieved the OpenSSF Best Practices passing badge:
- https://www.bestpractices.dev/en/projects/4748

## Ecosystem

### Suggested

N/A

### Required

- [x] **Publicly documented list of adopters, which may indicate their adoption level (dev/trialing, prod, etc.)**

<!-- (TOC Evaluation goes here) -->

Buildpacks maintains a public adopters list in the community repository.
- https://github.com/buildpacks/community/blob/main/ADOPTERS.md

- [x] **Used in appropriate capacity by at least 3 independent + indirect/direct adopters, (these are not required to be in the publicly documented list of adopters)**

<!-- (TOC Evaluation goes here) -->

Four adopters were interviewed (Google, Salesforce, Rapid7, 7SIGNAL). All four reported production usage at meaningful scale and described Buildpacks as core to container build and delivery workflows.


An adopter list was reviewed to verify level-appropriate usage (production use for graduation, dev/test use for incubation).

- [x] **TOC verification of adopters.**

<!-- (TOC Evaluation goes here) -->

Verification was completed through four adopter interviews and approved summaries captured in this folder.


Refer to the Adoption portion of this document.

- [x] **Clearly documented integrations and/or compatibility with other CNCF projects as well as non-CNCF projects.**

<!-- (TOC Evaluation goes here) -->

Buildpacks documentation includes integration guidance for major CNCF and non-CNCF ecosystems (for example Kubernetes, Tekton, Podman, Docker, and OCI-compatible registries/runtimes).
- https://buildpacks.io/docs/
- https://buildpacks.io/docs/for-platform-operators/how-to/integrate-ci/tekton/
- https://buildpacks.io/docs/for-app-developers/how-to/special-cases/build-on-podman/
- https://buildpacks.io/docs/for-platform-operators/how-to/integrate-ci/docker/


#### Adoption

The adopter interviews show Buildpacks is in production use at graduation maturity. Adopters report production-scale usage, measurable operational benefit, and positive maintainer/community engagement.

Common strengths across interviews:
- Consistent and reproducible source-to-image workflows at scale
- Reduced operational burden versus hand-maintained Dockerfiles
- Security and maintenance gains from rebasing, standardized base images, and SBOM-related workflows
- Good documentation and responsive maintainer/community interactions

Common improvement themes:
- Upgrade/version-alignment complexity across multiple Buildpacks components
- Migration friction for some legacy Dockerfile-heavy applications
- Continued improvement on multi-architecture support and rebase capabilities

##### Adopter 1 - Google / Cloud Platform (Serverless)

Interviewed: Jan 2026

Production usage across Cloud Run, Cloud Functions, and App Engine since 2020. Google reported Buildpacks as the standardized mechanism for source deployment, with very high build volume and strong value from open specification alignment and rebase-driven security updates.

Reference: [Buildpacks Adopter Interview - Google](./buildpacks-adopter-interview-google.md)

##### Adopter 2 - Salesforce / Enterprise Software (Internal CI)

Interviewed: Jan 2026

Production usage since 2022 in internal CI systems serving a large developer base, with sustained high daily build volume. Salesforce highlighted reproducibility, reduced manual effort, and strong utility for integration-test and configuration packaging workflows.

Reference: [Buildpacks Adopter Interview - Salesforce](./buildpacks-adopter-interview-salesforce.md)

##### Adopter 3 - Rapid7 / Cybersecurity

Interviewed: Jan 2026

Production usage since 2022 across multiple teams. Rapid7 described Buildpacks as a standard container-build path with custom buildpacks/builders where needed, citing security, rebasing, and standardization benefits, plus active community collaboration.

Reference: [Buildpacks Adopter Interview - Rapid7](./buildpacks-adopter-interview-rapid7.md)

##### Adopter 4 - 7SIGNAL / SaaS Network Monitoring

Interviewed: Jan 2026

Production usage for over three years across multiple applications. 7SIGNAL emphasized low setup overhead, low maintenance, consistent outcomes across projects, and improved security posture compared to Dockerfile-centered workflows.

Reference: [Buildpacks Adopter Interview - 7SIGNAL](./buildpacks-adopter-interview-7signalinc.md)
