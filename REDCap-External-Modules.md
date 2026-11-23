**REDCap External Modules**

REDCap External Modules are extensions that add or modify REDCap functionality without changing the core REDCap application code. They can provide capabilities such as custom integrations, workflow automation, additional user-interface features, validation logic, APIs, notifications and project-specific functions.

**External Modules may be sourced in two ways:**

- **Externally sourced modules** come from third parties or the REDCap community. An admin identifies the module by its GitHub repository and release tag, and the pipeline downloads it, puts it into the folder structure REDCap expects, and scans it for vulnerabilities, hardcoded secrets, and malware. A reviewer who isn't the person who requested the module checks the results and approves it. If review fails and needs a escalation, a separate named approver, such as the Cyber Security Lead, makes that decision and writes down why. Once approved, the exact file that was reviewed gets signed and published to our artefact repository as a permanent, versioned ZIP, along with its checksum, signature, SBOM, and a record of where it came from. Nothing gets rebuilt or re-downloaded after that point, so what was reviewed is exactly what gets used.

- **Internally developed modules** are maintained in a Git repository and follow a controlled CI/CD process. A pull request to main triggers a GitHub Actions pipeline that performs checks such as SAST, SCA and secret scanning. If the defined security policy is satisfied, the change can proceed to merge and the module is packaged as a versioned ZIP and published to the artefact repository. If significant issues are detected, the pull request is blocked and requires an authorised administrator or security approver to review and approve an exception before it can proceed.

 <img width="1417" height="633" alt="image" src="https://github.com/user-attachments/assets/9979bb5b-faee-4b7e-9e62-8ae0e3984d34" />


