**REDCap CI/CD**

This pipeline builds, secures, and deploys the REDCap application image to the Kubernetes cluster. It assumes the approved REDCap release ZIP and any external modules to be bundled into the image are already present in the artefact repository, having passed through their own ingestion and approval processes. This pipeline consumes those artefacts as trusted, immutable inputs — verified by checksum and signature — rather than fetching or approving them itself.

<img width="1417" height="605" alt="image" src="https://github.com/user-attachments/assets/c68adbc7-ff7a-4182-9c5a-18c539fdba34" />
