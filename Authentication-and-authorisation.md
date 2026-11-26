**Authentication and authorisation**

The External Module will manage the credentials required for both integration directions.

**Outbound access to XNAT**
For XNAT destinations:

- A dedicated XNAT user will be created.

- The user will be granted access only to the required XNAT projects.

- The username and password will be stored inline and encrypted by the module.

- The module will use the credentials to obtain a short-lived XNAT session token before calling XNAT APIs.

- Each destination will have a separate credential configuration.

**Inbound access to REDCap**
- The module will issue a separate client credential to each authorised external system. Each credential will be associated with explicit access grants for the relevant REDCap project, arm, event, instrument and operation.

- Credentials must support:

- Encryption at rest.

- Expiry and rotation.

- Immediate revocation.

- Masking in the user interface and logs.

TLS-protected transmission.

Credentials must not be embedded in source code or job definitions.
