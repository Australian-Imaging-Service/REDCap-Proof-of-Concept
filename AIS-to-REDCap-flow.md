**AIS/XNAT-to-REDCap flow**

✅ Imaging data is uploaded and archived in an XNAT project.

✅ XNAT Event Service detects the configured lifecycle event.

✅ XNAT Container Service launches the applicable analysis pipeline.

✅ The analysis results are stored in XNAT.

✅ A local integration component maps the approved results.

✅ It calls the External Module using its module-issued credential.

✅ The module validates the caller, project, participant, arm, event and instrument.

✅ The approved instrument data is created or updated in REDCap.

✅ The processing outcome is recorded.
