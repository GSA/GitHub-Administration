---
name: gsa-system
escription: Github Team Request
title: [system]() - [github-team]()
labels: "g: accepted, i: github-team"
assignees: "@tts-admins"
labels: ["bug", "triage"]
projects: ["gsa-tts/1"]
assignees:
  - tts-admins
  - tts-system-owners
  - tts-website-managers
  - tts-ISSO
  - tts-ISSM
body:
  - type: markdown
    attributes:
      value: |
        Team
  - type: input
    id: contact
    attributes:
      label: Contact
      description: GSA Email
      placeholder: email@gsa.gov
    validations:
      required: false
  - type: textarea
    id: what-happened
    attributes:
      label: What happened?
      description: Also tell us, what did you expect to happen?
      placeholder: Tell us what you see!
      value: "A bug happened!"
    validations:
      required: true
  - type: system-id
    id: version
    attributes:
      label: Version
      description: What version of our software are you running?
      options:
        - analytics.usa.gov
        - Api.Data.gov
        - Challenge.gov
        - Data.gov
        - Federal Audit Clearinghouse (FAC)
        - GSA Implementation of Genesys
        - GSA Implementation of Zendesk
        - Identity Verification API (IDVA)
        - lnteragency Suspension and Debarment Committee (ISDC)
        - Made in America (MiAO)
        - Search.gov
        - Site Scanner
        - System of Records Notice (SORN) Dashboard
        - Tock
        - Touchpoints (TP)
        - TTS Pages
        - US Notify
        - USA.GOV 
        - LOGIN.GOV
      default: tts.gsa.gov
    validations:
      required: true
  - type: dropdown
    id: browsers
    attributes:
      label: What browsers are you seeing the problem on?
      multiple: true
      options:
        - analytics.usa.gov
        - Api.Data.gov
        - Challenge.gov
        - Data.gov
        - Federal Audit Clearinghouse (FAC)
        - GSA Implementation of Genesys
        - GSA Implementation of Zendesk
        - Identity Verification API (IDVA)
        - lnteragency Suspension and Debarment Committee (ISDC)
        - Made in America (MiAO)
        - Search.gov
        - Site Scanner
        - System of Records Notice (SORN) Dashboard
        - Tock
        - Touchpoints (TP)
        - TTS Pages
        - US Notify
        - USA.GOV 
        - LOGIN.GOV
  - type: textarea
    id: logs
    attributes:
      label: Supervisor
      description: Supervisor
      render: shell
  - type: checkboxes
    id: terms
    attributes:
      label: Code of Conduct
      description: By submitting this issue, you agree to follow our [Code of Conduct](https://example.com)
      options:
        - label: I agree to follow this project's Code of Conduct
          required: true
    attributes:
      label: Code of Conduct
      description: By submitting this issue, you agree to follow our [Code of Conduct](https://example.com)
      options:
        - label: I agree to follow this project's Code of Conduct
          required: true          
```
---
