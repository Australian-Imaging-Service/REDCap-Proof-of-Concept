**Design overview**

✅ The proposed solution uses point-to-point integration between REDCap and external research platforms. A purpose-built REDCap External Module will be used to publish authorised REDCap data to configured destinations and expose APIs through which authorised external systems can submit data to REDCap.

✅ AIS/XNAT is used as the reference system in this design, although the same integration pattern may be applied to other approved platforms, including OpenSpecimen. The module will also manage the mapping of identifiers and data exchanged between these systems.
