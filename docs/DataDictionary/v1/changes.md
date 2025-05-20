# Changes and corrections to PREMIS data dictionary and schemas in version 2.0 

This document records corrections and changes that were approved  for version 2.0 of the <a href="http://www.oclc.org/research/projects/pmwg/premis-final.pdf">PREMIS Data Dictionary</a> and <a href="schemas.html">PREMIS schemas</a>. It does not include all stylistic changes or all changes to supporting documentation. The <a href="premis-editorial-committee.html">PREMIS Editorial Committee</a>  released the revised data dictionary on April 3, 2008. The PREMIS schema was also released as a draft for review at that time. 

## Approved changes (Data dictionary and schemas)

<ul>
  <li>Add clarification about repeatability of identifiers: objectIdentifier
    and agentIdentifier are repeatable because they may be defined and known
    outside the repository, and thus may have multiple identifiers; eventIdentifier
    and permissionStatementIdentifier are defined only inside the repository
    and should not be repeatable. </li>
  <li>Add an additional eventType suggested value for &quot;creation = the act of creating a new object&quot;</li>
  <li>Clarify difference between &quot;checksum&quot; and &quot;messageDigest&quot;</li>
  <li>Allow for use of  significantProperties   at the representation level;  consider additional structure under significantProperties. </li>
  <li>Introduce a numbering system to be used for navigation for each semantic
    unit in the data dictionary. 
    The numbering system will be grouped by  entity types: Object semantic units
    will be 1. and Event Semantic Units will be 2. If Business rules are added,
    they will be 5. The numbers can be added as comments within the Schema.</li>
  <li>Change relatedObjectSequence to optional; it is  now mandatory but  does not apply to derivative relationships.</li>
  <li>Make changes to preservationLevel. It will be optional, repeatable, and become a container with the following subunits: preservationLevelValue, preservationLevelRole, preservationLevelRationale, preservationLevelDateAssigned</li>
  <li>Change relatedEventIdentification to optional and specify that for derivative relationships it must be recorded </li>
  <li>Clarify the difference between whole/part and parent/child relationships (in suggested values under relationshipSubtype) by using &quot;hasPart&quot; and &quot;isPartOf&quot; as suggested values </li>
  <li>Revise the  data model to reflect relationships between entities more consistently with data dictionary semantic units in terms of bidirectional linking  </li>
  <li>In situations where all subunits are optional within a mandatory container, add usage notes  to specify that at least one subunit must be present</li>
  <li>Add a new optional semantic unit &quot;linkingObjectRole&quot; under linkingObjectIdentifier to disambiguate what role the object plays that is identified, e.g. &quot;source&quot; or &quot;outcome&quot; of an event</li>
  <li>Clarify definitions and examples for contentLocationType and contentLocationValue to show that file system locations as well as URLs may be recorded</li>
  <li>Make storageMedium applicable to bitstreams (but optional)</li>
  <li>Revise Rights entity to allow for wider scope of rights statements; distinguish between rights based on copyright, licenses, or statutes (based on <a href="Rights-in-the-PREMIS-Data-Model.pdf">Karen Coyle's report</a>) </li>
  <li>Under signatureInformation remove internal structure of keyInfo and handle in schema to allow for use of XML signature elements</li>
  <li>Include a discussion of how to use controlled vocabularies; the XML schemas will provide a mechanism for identifying the vocabulary used (coming after first official release of revised schema)</li>
  <li>Add note that persistentIDs are recommended, but that a particular identifier scheme is not specified </li>
  <li>Change swVersion to not repeatable at file level </li>
  <li>Change storage (container) to optional for bitstreams</li>
  <li>Clarify how objectCharacteristics apply to representations by adding a relationship subtype which specifies that a file functions also as a representation. This mechanism will also be used to specify originalName for the file that also functions as the representation</li>
  <li>Clarify the relationship between formatDesignation and formatRegistry; make format repeatable</li>
  <li>Add conventions for indicating different types of date conventions. Among other things  there is a need to specify no end date, i.e. that it is open-ended. Convention used will be &quot;OPEN&quot; in &lt;endDate&gt;. See: <a href="https://www.loc.gov/standards/datetime/">http://www.loc.gov/standards/datetime/ </a></li>
  <li>Implement a registry for controlled vocabularies (see also under schemas below). </li>
  <li>Allow for extensibility for the following PREMIS semantic units:
    <ul>
      <li>significantProperties (Object entity)</li>
      <li>objectCharacteristics (Object entity)</li>
      <li>creatingApplication (Object entity)</li>
      <li>environment (Object entity)</li>
      <li>signatureInformation (Object entity)</li>
      <li>eventOutcomeDetail (Event entity)</li>
      <li>rights (Rights entity)</li>
    </ul>
  </li>
  <li>Define a container for additional object characteristics specific to format type. Data from externally developed schemas will be used (see above under objectCharacteristics extensibility)</li>
  <li>Make storageMedium optional <br>
  </li>
</ul>
<h2>&nbsp;</h2>
<h2>Approved changes (schemas only)</h2>
<ul>
  <li>All those above under data dictionary will be changed in schemas (if applicable) </li>
  <li> relatedEventSequence  is optional in DD and mandatory in the schema; it will be changed to optional in the schema </li>
  <li>Allow for more control and extensibility in specifying object categories by allowing for validation of appropriate elements by object category (i.e. representation, file, bitstream) </li>
  <li>Implement mechanism for specifying use of controlled vocabularies. The Library of Congress as PREMIS Managing Agency will make PREMIS-developed controlled vocabularies available (and others as requested). This will be available in version 2.1, after the initial release of version 2.0 </li>
  <li>Define elements as global so that they can be reused in other XML schemas.</li>
  <li>Combine separate PREMIS schemas from version 1.1 into one schema. Since subelements object, event, agent and rights are defined globally, they may be use separately as in the previous version. </li>
  <li>Include definitions for alternate types of date expressions, including ISO 8601 basic format (without hyphens) and conventions for special types of dates (open, questionable, etc. dates) </li>
</ul>
