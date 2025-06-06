
# Hierarchical Listing of Semantic Units

<h2>PREMIS Data Dictionary for Preservation Metadata, Version 3.0 </h2>

      
<br>
<p>The PREMIS Data Dictionary and its supporting documentation is a comprehensive,
          practical resource for implementing preservation metadata in digital
          archiving systems. The Data Dictionary is built on a data model that
          defines five entities: Intellectual Entities, Objects, Events, Rights,
          and Agents. Each semantic unit defined in the Data Dictionary is a
          property of one of the entities in the data model.        </p>
<p>This is a hierarchical listing of the semantic units included in the
          Data Dictionary. The information in parentheses following each semantic
          unit indicates whether the element is Mandatory (M) or Optional (O),
          followed by whether it is Repeatable (R) or Not repeatable (NR). Some
          semantic units in the Object section are further divided by the types
          of representation, file, and bitstream. Where not qualified, the designations
          apply to all three types. Where qualified, only the types listed are
          applicable.</p>
<h2>1. Object</h2>
<p>1.1&nbsp;&nbsp;&nbsp; objectIdentifier  (M, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.1.1&nbsp;&nbsp;&nbsp; objectIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.1.2&nbsp;&nbsp;&nbsp; objectIdentifierValue  (M, NR)<br>
          1.2&nbsp;&nbsp;&nbsp; objectCategory  (M, NR)<br>
          1.3&nbsp;&nbsp;&nbsp; preservationLevel  (O, R) [Intellectual Entity, Representation, File]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.3.1&nbsp;&nbsp;&nbsp; preservationLevelType  (O, NR) [Intellectual Entity, Representation, File]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.3.2&nbsp;&nbsp;&nbsp; preservationLevelValue  (M, NR) [Intellectual Entity, Representation, File]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.3.3&nbsp;&nbsp;&nbsp; preservationLevelRole  (O, NR) [Intellectual Entity, Representation, File]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.3.4&nbsp;&nbsp;&nbsp; preservationLevelRationale  (O, R) [Intellectual Entity, Representation, File]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.3.5&nbsp;&nbsp;&nbsp; preservationLevelDateAssigned  (O, NR) [Intellectual Entity, Representation, File]<br>
          1.4&nbsp;&nbsp;&nbsp; significantProperties (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.4.1&nbsp;&nbsp;&nbsp; significantPropertiesType (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.4.2&nbsp;&nbsp;&nbsp; significantPropertiesValue (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.4.3&nbsp;&nbsp;&nbsp; significantPropertiesExtension (O, R)<br>
          1.5&nbsp;&nbsp;&nbsp; objectCharacteristics (M, R) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.1&nbsp;&nbsp;&nbsp; compositionLevel  (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.2&nbsp;&nbsp;&nbsp; fixity (O, R) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.2.1&nbsp;&nbsp;&nbsp; messageDigestAlgorithm (M, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.2.2&nbsp;&nbsp;&nbsp; messageDigest (M, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.2.3&nbsp;&nbsp;&nbsp; messageDigestOriginator (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.3&nbsp;&nbsp;&nbsp; size (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.4&nbsp;&nbsp;&nbsp; format (M, R) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.4.1&nbsp;&nbsp;&nbsp; formatDesignation  (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.4.1.1&nbsp;&nbsp;&nbsp; formatName  (M, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.4.1.2&nbsp;&nbsp;&nbsp; formatVersion  (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.4.2&nbsp;&nbsp;&nbsp; formatRegistry  (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.4.2.1&nbsp;&nbsp;&nbsp; formatRegistryName  (M, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.4.2.2&nbsp;&nbsp;&nbsp; formatRegistryKey  (M, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.4.2.3&nbsp;&nbsp;&nbsp; formatRegistryRole  (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.4.3&nbsp;&nbsp;&nbsp; formatNote  (O, R) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.5&nbsp;&nbsp;&nbsp; creatingApplication  (O, R) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.5.1&nbsp;&nbsp;&nbsp; creatingApplicationName  (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.5.2&nbsp;&nbsp;&nbsp; creatingApplicationVersion  (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.5.3&nbsp;&nbsp;&nbsp; dateCreatedByApplication  (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.5.4&nbsp;&nbsp;&nbsp; creatingApplicationExtension  (O, R) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.6&nbsp;&nbsp;&nbsp; inhibitors  (O, R) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.6.1&nbsp;&nbsp;&nbsp; inhibitorType  (M, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.6.2&nbsp;&nbsp;&nbsp; inhibitorTarget  (O, R) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.6.3&nbsp;&nbsp;&nbsp; inhibitorKey  (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.5.7&nbsp;&nbsp;&nbsp; objectCharacteristicsExtension  (O, R) [File, Bitstream]<br>
          1.6&nbsp;&nbsp;&nbsp; originalName  (O, NR) [Intellectual Entity, Representation, File]<br>
          1.7&nbsp;&nbsp;&nbsp; storage (O,  R) [Representation, File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.7.1&nbsp;&nbsp;&nbsp; contentLocation  (O, NR) [Representation, File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.7.1.1&nbsp;&nbsp;&nbsp; contentLocationType  (M, NR) [Representation, File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.7.1.2&nbsp;&nbsp;&nbsp; contentLocationValue  (M, NR) [Representation, File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.7.2&nbsp;&nbsp;&nbsp; storageMedium  (O, NR) [Representation, File, Bitstream]<br>
          1.8&nbsp;&nbsp;&nbsp; signatureInformation (O, R) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.8.1&nbsp;&nbsp;&nbsp; signature (O, R) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.8.1.1&nbsp;&nbsp;&nbsp; signatureEncoding  (M, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.8.1.2&nbsp;&nbsp;&nbsp; signer  (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.8.1.3&nbsp;&nbsp;&nbsp; signatureMethod  (M, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.8.1.4&nbsp;&nbsp;&nbsp; signatureValue  (M, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.8.1.5&nbsp;&nbsp;&nbsp; signatureValidationRules  (M, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.8.1.6&nbsp;&nbsp;&nbsp; signatureProperties  (O, R) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.8.1.7&nbsp;&nbsp;&nbsp; keyInformation  (O, NR) [File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.8.2&nbsp;&nbsp;&nbsp; signatureInformationExtension  (O, R) [File, Bitstream]<br>
          1.9&nbsp;&nbsp;&nbsp; environmentFunction  (O, R) [Intellectual Entity of type environment]<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.9.1&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;environmentFunctionType (M, NR) [Intellectual  Entity of type environment]<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.9.2&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;environmentFunctionLevel (M, NR) [Intellectual  Entity of type environment]<br>
          1.10&nbsp; environmentDesignation  (O, R) [Intellectual Entity of type environment]<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.10.1&nbsp;&nbsp;&nbsp;&nbsp; environmentName (M, NR) [Intellectual Entity of type environment] <br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.10.2&nbsp;&nbsp;&nbsp;&nbsp; environmentVersion (O, NR) [Intellectual Entity of type environment] <br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.10.3&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;environmentOrigin (O, NR) [Intellectual  Entity of type environment] <br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.10.4&nbsp;&nbsp;&nbsp;&nbsp; environmentDesignationNote (O, R) [Intellectual Entity of type  environment] <br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.10.5&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;environmentDesignationExtension (O,  R) [Intellectual Entity of type environment] <br>
          1.11&nbsp; environmentRegistry (O, R) [Intellectual  Entity of type environment]<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.11.1&nbsp;&nbsp;&nbsp;&nbsp; environmentRegistryName (M, NR) [Intellectual  Entity of type environment] <br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.11.2&nbsp;&nbsp;&nbsp;&nbsp; environmentRegistryKey (M, NR) [Intellectual  Entity of type environment] <br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1.11.3&nbsp;&nbsp;&nbsp;&nbsp; environmentRegistryRole (O, NR) [Intellectual  Entity of type environment] <br>
          1.12&nbsp; environmentExtension  (O, R) [Intellectual Entity of type environment]<br>
          1.13&nbsp; relationship  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.1&nbsp; relationshipType (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.2&nbsp; relationshipSubType (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.3&nbsp; relatedObjectIdentifier  (M, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.3.1&nbsp; relatedObjectIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.3.2&nbsp; relatedObjectIdentifierValue  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.3.3&nbsp; relatedObjectSequence  (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.4&nbsp; relatedEventIdentifier  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.4.1&nbsp; relatedEventIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.4.2&nbsp; relatedEventIdentifierValue  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.4.3&nbsp; relatedEventSequence  (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.5&nbsp; relatedEnvironmentPurpose  (O, R) [Representation, File, Bitstream]<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.13.6&nbsp; relatedEnvironmentCharacteristic  (O, NR) [Representation, File, Bitstream]<br>
          1.14&nbsp; linkingEventIdentifier  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.14.1&nbsp; linkingEventIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.14.2&nbsp; linkingEventIdentifierValue  (M, NR)<br>
          1.15&nbsp; linkingRightsStatementIdentifier  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.15.1&nbsp; linkingRightsStatementIdentifierType  (M, NR)<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;1.15.2&nbsp; linkingRightsStatementIdentifierValue  (M, NR)</p>
<h2>Event</h2>
<p>2.1&nbsp;&nbsp;&nbsp; eventIdentifier (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.1.1&nbsp;&nbsp;&nbsp; eventIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.1.2&nbsp;&nbsp;&nbsp; eventIdentifierValue  (M, NR)<br>
          2.2&nbsp;&nbsp;&nbsp; eventType (M,  NR)<br>
          2.3&nbsp;&nbsp;&nbsp; eventDateTime  (M, NR)<br>
          2.4&nbsp;&nbsp;&nbsp; eventDetailInformation  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.4.1&nbsp;&nbsp;&nbsp; eventDetail (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.4.2&nbsp;&nbsp;&nbsp; eventDetailExtension (O, R)<br>
          2.5&nbsp;&nbsp;&nbsp; eventOutcomeInformation  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.5.1&nbsp;&nbsp;&nbsp; eventOutcome (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.5.2&nbsp;&nbsp;&nbsp; eventOutcomeDetail (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.5.2.1&nbsp;&nbsp;&nbsp; eventOutcomeDetailNote  (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.5.2.2&nbsp;&nbsp;&nbsp; eventOutcomeDetailExtension  (O, R)<br>
          2.6&nbsp;&nbsp;&nbsp; linkingAgentIdentifier  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.6.1&nbsp;&nbsp;&nbsp; linkingAgentIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.6.2&nbsp;&nbsp;&nbsp; linkingAgentIdentifierValue  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.6.3&nbsp;&nbsp;&nbsp; linkingAgentRole  (O, R)<br>
          2.7&nbsp;&nbsp;&nbsp; linkingObjectIdentifier  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.7.1&nbsp;&nbsp;&nbsp; linkingObjectIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.7.2&nbsp;&nbsp;&nbsp; linkingObjectIdentifierValue  (M, NR)<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;2.7.3&nbsp;&nbsp;&nbsp; linkingObjectRole  (O, R)</p>
<h2>Agent</h2>
<p>3.1&nbsp;&nbsp;&nbsp; agentIdentifier  (M, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.1.1&nbsp;&nbsp;&nbsp; agentIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.1.2&nbsp;&nbsp;&nbsp; agentIdentifierValue  (M, NR)<br>
          3.2&nbsp;&nbsp;&nbsp; agentName (O,  R)<br>
          3.3&nbsp;&nbsp;&nbsp; agentType (O,  NR)<br>
          3.4&nbsp;&nbsp;&nbsp; agentVersion  (O, NR)<br>
          3.5&nbsp;&nbsp;&nbsp; agentNote (O,  R)<br>
          3.6&nbsp;&nbsp;&nbsp; agentExtension  (O, R)<br>
          3.7&nbsp;&nbsp;&nbsp; linkingEventIdentifier  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.7.1&nbsp;&nbsp;&nbsp; linkingEventIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.7.2&nbsp;&nbsp;&nbsp; linkingEventIdentifierValue  (M, NR)<br>
          3.8&nbsp;&nbsp;&nbsp; linkingRightsStatementIdentifier  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.8.1&nbsp;&nbsp;&nbsp; linkingRightsStatementIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.8.2&nbsp;&nbsp;&nbsp; linkingRightsStatementIdentifierValue  (M, NR)<br>
          3.9&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; linkingEnvironmentIdentifier (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.9.1&nbsp;&nbsp;&nbsp;&nbsp; linkingEnvironmentIdentifierType (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.9.2&nbsp;&nbsp;&nbsp;&nbsp; linkingEnvironmentIdentifierValue (M, NR)<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;3.9.3&nbsp;&nbsp;&nbsp;&nbsp; linkingEnvironmentRole (O, R)</p>
<h2>Rights</h2>
<p>4.1&nbsp;&nbsp;&nbsp; rightsStatement  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.1&nbsp;&nbsp;&nbsp; rightsStatementIdentifier  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.1.1&nbsp;&nbsp;&nbsp; rightsStatementIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.1.2&nbsp;&nbsp;&nbsp; rightsStatementIdentifierValue  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.2&nbsp;&nbsp;&nbsp; rightsBasis  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3&nbsp;&nbsp;&nbsp; copyrightInformation  (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3.1&nbsp;&nbsp;&nbsp; copyrightStatus  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3.2&nbsp;&nbsp;&nbsp; copyrightJurisdiction  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&#12288;4.1.3.3&nbsp;&nbsp;&nbsp; copyrightStatusDeterminationDate  (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3.4&nbsp;&nbsp;&nbsp; copyrightNote (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3.5&nbsp;&nbsp;&nbsp; copyrightDocumentationIdentifier (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3.5.1&nbsp;&nbsp;&nbsp;&nbsp; copyrightDocumentationIdentifierType (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3.5.2&nbsp;&nbsp;&nbsp;&nbsp; copyrightDocumentationIdentifierValue (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3.5.3&nbsp;&nbsp;&nbsp;&nbsp; copyrightDocumentationRole (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3.6&nbsp;&nbsp;&nbsp; copyrightApplicableDates (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3.6.1&nbsp;&nbsp;&nbsp;&nbsp; startDate (O, NR)<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.3.6.2&nbsp;&nbsp;&nbsp;&nbsp; endDate (O, NR)<br>
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4&nbsp;&nbsp; licenseInformation (O, NR) <br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4.1&nbsp;&nbsp;&nbsp; licenseDocumentationIdentifier (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4.1.1&nbsp;&nbsp;&nbsp; licenseDocumentationIdentifierType (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4.1.2&nbsp;&nbsp;&nbsp; licenseDocumentationIdentifierValue (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4.1.3&nbsp;&nbsp;&nbsp; licenseDocumentationRole (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4.2&nbsp;&nbsp;&nbsp; licenseTerms (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4.3&nbsp;&nbsp;&nbsp; licenseNote (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4.4&nbsp;&nbsp;&nbsp; licenseApplicableDates (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4.4.1&nbsp;&nbsp;&nbsp; startDate (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.4.4.2&nbsp;&nbsp;&nbsp; endDate (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5&nbsp; statuteInformation (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5.1&nbsp;&nbsp;&nbsp; statuteJurisdiction (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5.2&nbsp;&nbsp;&nbsp; statuteCitation (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5.3&nbsp;&nbsp;&nbsp; statuteInformationDeterminationDate (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5.4&nbsp;&nbsp;&nbsp; statuteNote (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5.5&nbsp;&nbsp;&nbsp; statuteDocumentationIdentifier  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5.5.1&nbsp;&nbsp;&nbsp; statuteDocumentationIdentifierType (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5.5.2&nbsp;&nbsp;&nbsp; statuteDocumentationIdentifierValue (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5.5.3&nbsp;&nbsp;&nbsp; statuteDocumentationRole (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5.6&nbsp;&nbsp;&nbsp; statuteApplicableDates (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5.6.1&nbsp;&nbsp;&nbsp; startDate (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.5.6.2&nbsp;&nbsp;&nbsp; endDate (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.6&nbsp; otherRightsInformation (O, NR)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4.1.6.1&nbsp;&nbsp;&nbsp; otherRightsDocumentationIdentifier (O, R)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4.1.6.1.1&nbsp;&nbsp;&nbsp; otherRightsDocumentationIdentifierType (M,  NR)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4.1.6.1.2&nbsp;&nbsp;&nbsp; otherRightsDocumentationIdentifierValue (M,  NR)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4.1.6.1.3&nbsp;&nbsp;&nbsp; otherRightsDocumentationRole (O, NR)&nbsp;&nbsp;&nbsp; <br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4.1.6.2&nbsp;&nbsp;&nbsp; otherRightsBasis (M, NR)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.6.3&nbsp;&nbsp;&nbsp; otherRightsApplicableDates (O, NR)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;4.1.6.3.1&nbsp;&nbsp;&nbsp; startDate  (O, NR)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4.1.6.3.2&nbsp;&nbsp;&nbsp; endDate (O, NR)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.6.4&nbsp;&nbsp;&nbsp; otherRightsNote (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.7&nbsp; rightsGranted  (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.7.1&nbsp;&nbsp;&nbsp; act (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.7.2&nbsp;&nbsp;&nbsp; restriction (O, R)<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.7.3&nbsp;&nbsp;&nbsp; termOfGrant  (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.7.3.1&nbsp;&nbsp;&nbsp; startDate  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.7.3.2&nbsp;&nbsp;&nbsp; endDate (O, NR)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4.1.7.4&nbsp;&nbsp;&nbsp; termOfRestriction  (O, NR)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4.1.7.4.1&nbsp;&nbsp;&nbsp; startDate (M, NR)<br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 4.1.7.4.2&nbsp;&nbsp;&nbsp; endDate (O, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.7.5&nbsp;&nbsp;&nbsp; rightsGrantedNote (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.8&nbsp; linkingObjectIdentifier (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.8.1&nbsp;&nbsp;&nbsp; linkingObjectIdentifierType (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.8.2&nbsp;&nbsp;&nbsp; linkingObjectIdentifierValue (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.8.3&nbsp;&nbsp;&nbsp; linkingObjectRole (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.9&nbsp; linkingAgentIdentifier (O, R)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.9.1&nbsp;&nbsp;&nbsp; linkingAgentIdentifierType  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.9.2&nbsp;&nbsp;&nbsp; linkingAgentIdentifierValue  (M, NR)<br>
          &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;4.1.9.3&nbsp;&nbsp;&nbsp; linkingAgentRole  (O, R)<br>
        4.2&nbsp;&nbsp;&nbsp; rightsExtension  (O, R)</p>

