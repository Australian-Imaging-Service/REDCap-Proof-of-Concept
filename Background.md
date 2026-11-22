**Background**

Research studies increasingly rely on multiple specialised platforms. REDCap may capture participant and clinical research data, AIS/XNAT manages imaging studies, and OpenSpecimen BIMS manages biospecimens. Although these platforms may support the same research activity, they operate independently, use different project and participant identifiers, and provide limited native capability to establish and manage relationships across systems. These relationships can also be many-to-many: a REDCap project may support multiple AIS or BIMS projects, while an AIS or BIMS project may receive information from multiple REDCap projects. 

For the initial implementation, a point-to-point integration approach will be adopted to reduce implementation complexity, accepting reduced robustness—particularly the difficulty of guaranteeing at-least-once message delivery—as a known trade-off.
