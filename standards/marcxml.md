---
title: MAchine Readable Cataloging record XML 
slug: marcxml
subjects:
 - arts-and-humanities
 - general
disciplines:
- P120 - Librarianship
- P121 - Library studies
specification_url: http://www.loc.gov/standards/marcxml/schema/MARC21slim.xsd
status: Maintained by The Network Development and MARC Standards Office at the Library of Congress 
website: http://www.loc.gov/standards/marcxml//
related_vocabularies:
 - name: MODS
    url: http://www.loc.gov/standards/mods/
 - name: MADS
    url: http://www.loc.gov/standards/mads/
mappings:
 - name: MODS
    url: http://www.loc.gov/standards/marcxml//
sponsors:
 - name: Library of Congress
    url: https://www.loc.gov/
 - name: Network Development and MARC Standards Office
    url: http://www.loc.gov/marc/ndmso.html
contact: Network Development and MARC Standards Office
Library of Congress
LS/NDMSO (4402)
Washington, DC 20540-4402
contact_email: ndmso@loc.gov
standard_update_date: 2009-05-21
version: Version 1.2
description: |
 <p>From Website: The Library of Congress' Network Development and MARC Standards Office is developing a framework for working with MARC data in a XML environment. This framework is intended to be flexible and extensible to allow users to work with MARC data in ways specific to their needs. The framework will contain many components such as schemas, stylesheets, and software tools developed and maintained by the Library of Congress.</p>
 
<p>The core of the MARC XML framework is a simple XML schema which contains MARC data. This base schema output can be used where full MARC records are needed or act as a "bus" to enable MARC data records to go through further transformations such as toDublin Core and/or processes such as validation. The MARC XML schema will not need to be edited to reflect minor changes to MARC21. The schema retains the semantics of MARC.
All control fields, including the leader are treated as a data string. Fields are treated as elements with the tag as an attribute and indicators treated as attributes. Subfields are treated as subelements with the subfield code as an attribute.</p>
# The following are constants: do not modify
layout: standard
type: standard
---
