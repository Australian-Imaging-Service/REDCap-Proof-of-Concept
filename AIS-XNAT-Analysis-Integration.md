**AIS/XNAT analysis and integration**

Each federated AIS/XNAT instance may operate a locally deployed analysis and integration workflow.

XNAT Event Service can detect configured imaging lifecycle events, such as an imaging session being archived, and trigger an analysis pipeline through XNAT Container Service. Following successful analysis, a local integration component maps the approved results and submits them to the External Module’s inbound API.

**The workflow will:**

✅ Associate REDCap participants and visits with XNAT subjects and imaging sessions.

✅ Run configured image-analysis pipelines.

✅ Store analysis outputs in XNAT.

✅ Publish approved results to REDCap.

✅ Record processing outcomes and errors.

✅ Retry failed submissions according to the local retry policy.
