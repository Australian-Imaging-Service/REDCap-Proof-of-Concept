**REDCap-to-AIS/XNAT flow**

✅ Publication is initiated automatically following an eligible instrument save or manually when an authorised user selects Publish.

✅ The module identifies the applicable destination and publication definition.

✅ It validates the user, record, arm, event, instrument, release conditions and mandatory data.

✅ The module creates a persistent publication request.

✅ It authenticates to XNAT and obtains a session token.

✅ It maps the REDCap data to the configured XNAT API contract.

✅ It creates or updates the configured XNAT subject, session or other object.

✅ The publication status and outcome are recorded.
