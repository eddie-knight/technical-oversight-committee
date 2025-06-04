name: Labs Project Application
description: Checklist to evaluate a project for FINOS Labs acceptance and ongoing maintenance requirements.
title: "[Labs Acceptance] <project-name>"
labels: ["labs-review", "acceptance-checklist"]
body:

  - type: markdown
    attributes:
      value: |
        ## Labs Project Acceptance Requirements

        Please complete the following checklist to confirm your project meets the Labs entry and ongoing maintenance requirements. For any item not yet complete, provide an explanation in the comments.

  - type: checkboxes
    id: acceptance
    attributes:
      label: Acceptance Requirements
      options:
        - label: At least one member maintainer is assigned
        - label: Project has a clear use case for the financial services industry
        - label: Development next steps are documented in the repository
        - label: Project name is not reasonably confused with any other FINOS efforts
        - label: Project is licensed under Apache v2, a Category A license, or has an approved exception from the FINOS Governing Board
        - label: Project trademark is owned by FINOS / LF (may be completed after TOC approval)

  - type: markdown
    attributes:
      value: |
        ## Ongoing Maintenance Requirements

        These must be met to remain in Labs and avoid archival.

  - type: checkboxes
    id: maintenance
    attributes:
      label: Ongoing Maintenance
      options:
        - label: All Labs acceptance requirements are still met
        - label: Public FINOS GitHub repository shows activity since the last review
        - label: Reasonable completion of any TOC-issued requests
        - label: LICENSE, NOTICE, and CONTRIBUTING files conform to FINOS standards
        - label: All community meetings follow FINOS requirements
        - label: Project README displays the appropriate FINOS Project Status Badge
        - label: Project demonstrates adherence to OSPS Baseline Level 1

  - type: textarea
    id: comments
    attributes:
      label: Comments or Exceptions
      description: Provide context, links, or justifications for any incomplete or pending checklist items.
